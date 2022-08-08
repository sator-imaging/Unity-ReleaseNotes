# Unity 2019.1

https://unity3d.com/unity/whats-new/2019.1.0

## Improvements



*   2D: Added GridPaintSortingAttribute to allow users to specify the sorting of GameObjects listed in the Active Tilemaps list of the Tile Palette
    
*   Android: Add keystores dedicated location option
    
*   Android: Added **Symlink Sources** in the **Build Settings** window. This enables Java and Kotlin files to be directly referenced from Unity projects in an exported Gradle project.
    
*   Android: Added a check for Vulkan device compatibility on Build and Run
    
*   Android: Added Vulkan renderer compatibility to the Unity video player
    
*   Android: Disabled various Adreno Vulkan driver workarounds for latest drivers
    
*   Android: Enumerated all Android audio input device options, including the lowest-latency option, which can be selected via the name **Android voice recognition input**
    
*   Android: Implemented Native Systrace profiling support
    
*   Android: Improved IL2CPP player startup by ~200ms for second and later launches.
    
*   Android: Made the number of worker threads adjust dynamically according to the number of online cores.
    
*   Android: Made the Proguard mapping file save at the same location after building the APK
    
*   Android: More devices can use OpenSL instead of AudioTrack.This reduces audio input and output latency.
    
*   Animation: Added Experimental methods to AnimationPlay.
    
*   Animation: Added property Avatar.humanDescription.
    
*   Animation: Aligned all Animator StateMachine nodes on the grid.
    
*   Animation: Changed default StateMachine node width so that all nodes align vertically.
    
*   Animation: Implemented shift-click and right-click context menu to add properties in animation window without closing popup window.
    
*   Animation: Improved performance for AvatarBuilder.
    
*   Animation: Unity now adds `TransformStreamHandle` bound to the Transform dynamically at run time. This improves support for animation jobs.
    
*   Animation: Upgraded the animation window preview/playback engine to use the Playable API.
    
*   Asset Import: Added support for cameras in Sketchup Importer.
    
*   Asset Import: Extended the **Optimize Mesh** option on Model Asset import settings, to allow you to independently control optimization of Vertex Order and Polygon Order, rather than using the same flag for both. NOTE: Performance improvements to the underlying Mesh optimization code might cause Unity to generate vertices in a different order than in previous Unity versions. If you rely on vertex ordering in the optimized Mesh data (such as for vertex painting), be aware that you may need to re-generate this data.
    
*   Asset Import: Improved performance of DXT1/BC1 and DXT5/BC3 Texture compression This does not affect compression quality, but it does probably produce subtly different compression results.
    
*   Asset Pipeline: Scriptable objects that are loaded before a refresh/import, will after a refresh/import be reloaded, if the underlying asset had been modified before the refresh/import. This means that after the refresh/import scriptables objects will have the modified values from modified assets. Before this change, the scriptable object would get "null" value (when using operator==) after the refresh/import.
    
*   Compute: \* Added new functionality to allow Unity to use more of the scripting `CommandBuffer` utility functions with command buffers executed on async compute (such as getting temporary render targets).
    
    *   Added the concept of execution flags to `CommandBuffer` to describe how they should execute and allow for better error handling when those command buffers are built in script. This allows for generating exceptions when adding commands not valid for async compute.
    *   Added in-Editor detection for potential GPU deadlock cases where you creates a GPU fence in one command buffer but then never execute that command buffer.
*   Editor: Added a confirmation prompt when you delete a Shortcut Profile through the Shortcut Manager.
    
*   Editor: Added a keyboard shortcut for the submit button on the changeset submission window, and for some commonly used VCS operations. (1069130)
    
*   Editor: Added Field Of View axis selection drop-down in Camera Inspector.
    
*   Editor: Added **Clear on Build** option in Console.
    
*   Editor: Assembly Definition File inspector: Assembly Definition References, Assembly References and Define Constraints lists are now reorderable when editing a single Assembly Definition File.
    
*   Editor: Improved detecting of Visual Studio for Mac detecting when "Visual Studio.app" filename contains suffixes.
    
*   Editor: Improved performance of the Model Importer Inspector Material remapping section.
    
*   Editor: Improved performance when interacting with Model Inspector with some large Meshes.
    
*   Editor: Improved the performance of the UIElements renderer.
    
*   Editor: Made columns resizable in the Shortcuts Manager Command list.
    
*   Editor: Metal: Added Texture type validation to built-in Metal API validation feature.
    
*   Editor: Moved Camera Easing options to Camera Settings in SceneView from Preferences
    
*   Editor: Reworked Android keystore and key creation UI.
    
*   GI: Added support for shadow mask for rectangular area lights in the progressive lightmappers (available via HDRP).
    
*   GI: Added support for user defined range for area lights.
    
*   GI: Enabled the GPU lightmapper (preview) for macOS and Linux.
    
*   GI: GPU lightmapper now dumps a memory report to Editor.log when it falls back to CPU lightmapper.
    
*   GI: Lightprobe Gizmos are now affected by post-processing.
    
*   GI: Optimized baking of low occupancy lightmaps when using the GPU Lightmapper.
    
*   Graphics: Added filtering for sorting layers to the ScriptableRenderContext.
    
*   Graphics: Added fix to remove stalling on the render thread when loading large Textures.
    
*   Graphics: Added mixed area lights to cull results. This enables mixed rectangular lights in HDRP.
    
*   Graphics: Added Rendering.GraphicsSettings.realtimeDirectRectangularAreaLights to Scriptable Render Pipelines. This provides direct realtime area lighting.
    
*   Graphics: Added SRP hooks for detail rendering Shaders.
    
*   Graphics: Added support for Dynamic Resolution Scaling to the Lightweight Render Pipeline.
    
*   Graphics: Changed the Motion Vector behavior when the exclude motion vector flag is on: 1 - Motion Vector no longer skips nodes that only have Camera Motion 2 - Motion Vector now only skips submeshes with an explicit motion vector pass
    
*   Graphics: Emabled import and skinning of models with up to 32 bone weights for each vertex.
    
*   Graphics: Frame debugger now displays Shader properties for compute Shader dispatches.
    
*   Graphics: GraphicsFences are now available on Vulkan, Metal, D3D11, OpenGL, and OpenGL ES rendering backends.
    
*   Graphics: Made changes so that mesh creation is performed for Terrain details (such as grass) on parallel threads.
    
*   Graphics: Metal/iOS: Fixed Dynamic Resolution render surfaces to use heap allocation with aliasing to improve performance and memory usage.
    
*   Graphics: Metal/macOS: Moved immutable buffers and most Textures from using managed storage into private memory storage, to improve performance and CPU memory utilization.
    
*   Graphics: Metal: Applied a second iteration on the Metal heap allocation management to make it more fine-grained.
    
*   Graphics: Metal: Unity now defers creation of command buffers and render encoders until it actually needs them.
    
*   Graphics: Moved creation of Textures during async load on PC DX11 and Mac Metal off render thread into a job, to minimise problems during load.
    
*   Graphics: Not evaluating the light rectangles for oblique projection matrices
    
*   Graphics: Replaced Shader selection dropdown in Material Asset editor with a searchable drop-down.
    
*   Graphics: Revamped the DrawProcedural script API:
    
    *   DrawProceduralNow replaces the existing API, because it submits draw calls immediately. The new DrawProcedural API submits calls to color, shadows, reflections etc. This now matches the DrawMesh/DrawMeshNow API.
    *   Added overloads of DrawProcedural that take an Index Buffer
*   Graphics: Unity now supports Texture Mipmap streaming in Edit Mode when **Texture Streaming** is enabled in the Editor Settings.
    
*   Graphics: Updated the ASTC texture compressor with faster multi-core compression.
    
*   Graphics: `Graphics.Blit` and `CommandBuffer.Blit` methods now support blitting to and from Texture arrays.
    
*   IL2CPP: Improve run time performance when script debugging is enabled.
    
*   IL2CPP: Improved the performance of code generated by IL2CPP by up to 20%.
    
*   IL2CPP: Setting IL2CPP compiler config to "Master" will now enable Link Time Optimization on Mac, Android and WebGL
    
*   iOS: Added Access WiFi Capability to the Xcode API (availabe from iOS 12/Xcode 10)
    
*   iOS: Added device generation enums for the 2018 iPad Pro
    
*   iOS: Added launch screen image fields for iPhone XS and XS Max.
    
*   iOS: Added support for the iPhone XS/XS Max (DPI and device detection)
    
*   iOS: Refactored iOS device generation parsing
    
*   Mobile: Added support for RGBM and native HDR lightmaps
    
*   OSX: Made V-sync handling in macOS standalone players more stable.
    
*   Package Manager: _Editor.log_ now logs project load time.
    
*   Package Manager: Added _enablePackageManagerTraces_ command argument functionality, so you can use it to increase the logging level of the UPM process (and increase the verbosity of the upm.log file).
    
*   Package Manager: Introducing scoped registry feature. This empower users to host their own package in a local private registry. This is experimental. The package manager UI was not updated for this feature.
    
*   Package Manager: Released Package Manager UI v2.1.0-preview-1:
    
    *   Support maximize/minimize
    *   You can now save the PackageManager UI as a maximized window in your Editor layout
    *   Keep track of selected built-in package
    *   Keep track of last selected filter
    *   Fixed UI layout
*   Package Manager: Removed reference to "package" or "package manager" in the extension manager logs to avoid confusion with the new Package Manager system.
    
*   Package Manager: The Package Manager now displays dependent packages and corresponding assemblies in Object Picker.
    
*   Particles: Added a new mode to the Texture Sheet Animation Module that allows animations to be specific to each mesh a particle is using.
    
*   Particles: Added missing script API for External Forces influencers list.
    
*   Particles: Exposed missing External Forces module properties to script API.
    
*   Particles: Exposed particle mesh indices to script, so you can get and set which mesh each particle is using.
    
*   Particles: Exposed particle mesh indices to shaders, so you know which mesh each particle is using.
    
*   Physics: Added "Collision.contactCount" to retrieve the number of contacts.
    
*   Physics: Added "Collision.GetContact(index)" to retrieve a specific contact.
    
*   Physics: Added "Collision.GetContacts(array)" to retrieve all contacts.
    
*   Physics: Added an _Info_ section to the Rigidbody Inspector view that let's you examine the current velocities, centre of mass and inertia tensor of the Rigidbody.
    
*   Physics: Added an overload of `Rigidbody2D.MoveRotation` that accepts a Quaternion.
    
*   Physics: OnCollisionEnter, OnCollisionStay & OnCollisionExit no longer create any GC allocations.
    
*   Physics: OnCollisionEnter2D, OnCollisionStay2D & OnCollisionExit2D no longer create any GC allocations.
    
*   Physics: The Inspector _Info_ sections for the Rigidbody2D and Collider2D components now remain expanded when entering and exiting Play mode or moving between components.
    
*   Plugins: Preloading is now supported for any native plug-in. Added PluginImporter.isPreloaded.
    
*   Plugins: When you double-click a plug-in in your Unity project, an associated IDE now opens.
    
*   Prefabs: Added method PrefabUtility.HasPrefabInstanceAnyOverrides to quickly check if there's any override on a Prefab instance.
    
*   Prefabs: Show a "Auto Saving..." badge next to the 'Auto Save' toggle button when saving duration is over 1 second.
    
*   Prefabs: You can now edit the root GameObject of a Prefab directly from the Project browser, without going into Prefab Mode. This supports multi-GameObject editing as well. ([1120805](https://issuetracker.unity3d.com/issues/editing-prefabs-directly-in-the-project-browser-is-no-longer-possible), 1120807)
    
*   Profiler: Added "Semaphore.WaitForSignal" profiler marker.
    
*   Profiler: Added Mono.JIT and Mono.DomainUnload profiler markers.
    
*   Profiler: Added profiler markers for static constructors.
    
*   Profiler: Enabled automatic scripting threads profiling for ILC2PP.
    
*   Profiler: Increased minimum memory usage for profiler to 4MB in Players and 64MB in the Editor.
    
*   Profiler: The Unity Profiler now shows the amount of time until the next frame consistently accross all player platforms, regardless of how V-sync is implemented.
    
*   ps4: Added `PS4Input.touchpadMouseSensitivity` to provide sensitivity support for touchpad pointer emulation.
    
*   Scripting: Added ability to create `NativeArrays` of bool and char and `types` containing bool and char. (1127499, 1129523)
    
*   Scripting: Added support for Visual Studio 2019 code editor.
    
*   Scripting Upgrade: Support C# 7.3 when targeting .NET 4.x Equivalent Scripting Runtime.
    
*   Shaders: Defined `UNITY_SEPARATE_TEXTURE_SAMPLER` in `HlslSupport.cginc` for platforms capable of separate texture and sampler objects.
    
*   Shaders: Improve shader debugging. Unity now disables the optimiser when it generates debug shaders (i.e. #pragma enable\_d3d11\_debug\_symbols).
    
*   Shaders: Moved 38 built-in keywords to local keywords. The Shaders inspector now displays global/local keywords by shader.
    
*   Shaders: Shaders can now include files from packages directly like this: #include "Packages/packagename/IncludeFile.cginc"
    
*   Terrain: Added a direction bias to the Terrain smoothing Brush for increasing and decreasing blur.
    
*   Terrain: Added hotkeys to adjust Terrain tool brush size and opacity.
    
*   Terrain: Made changes to allow the setting of `shadowCastingMode` on Terrain.
    
*   Timeline: Added Volume, Pan and Spatial Blend controls to Audio Tracks, and volume controls to Audio Track Clips.
    
*   Timeline: Improved performance and reduced allocations when playing a Timeline
    
*   Timeline: Made performance improvements to the Timeline Editor Window display.
    
*   UI: Adding ability to modify the ui Dropdowns alpha fade when showing and hiding.
    
*   UI: Adding the ability to to use Sprite Tight mesh inside Unity UI
    
*   UI: Removing option for spritePacking tag in TextureImporter (sprites) when not using the legacy packing mode.
    
*   Universal Windows Platform: Added support for building player with Visual Studio 2019.
    
*   Universal Windows Platform: Added `ExecutableOnly` build type, which allows you to build without creating a Visual Studio project. This enables quicker iteration when using **Build & Run**. See documentation for `UnityEditor.WSAUWPBuildType` for more information
    
*   Video: Improved the platform strings documentation for the Set, Get, and ClearTargetSettings methods, in the VideoClipImporter class.
    
*   Web: Added support to write to file in append mode in `DownloadHandlerFile`.
    
*   Web: UnityWebRequest now reports Content-Length to `DownloadHandlerScript` as 64-bit. 32-bit method is now deprecated. ([1092447](https://issuetracker.unity3d.com/issues/scripting-downloadhandler-dot-receivecontentlength-2gb-integer-overflow))
    
*   WebGL: Added multi-threading compatibility check.
    
*   WebGL: Added `Quit()` function support to the Unity instance.
    
*   WebGL: Added `UnityLoader.instantiateAsync()`, which returns a JavaScript `Promise`.
    
*   XR: Enable depthBufferSharing by default for Windows Mixed Reality.
    
*   XR: Fixed linear color space on Oculus Go and Quest. For Gear VR, driver issues might prevent linear color space from working with S7 Adreno phones on Android 7.0.
    
*   XR: Fixed wireframe shader in single-pass instancing stereo rendering mode.
    
*   XR: Update Vuforia to version 7.5.20
    
*   XR: Updated Google VR to version 1.18.0.
    
*   XR: Updated Oculus's minimum supported version to 1.28.0.
    
*   XR: Updated Vuforia to version 8.0.10.
    
*   XR: Updated Vuforia to version 8.1.7.
    
*   XR: UpdateVuforia to version 7.5.26
    
*   XR: XR LWRP improvements:
    
    1.  Implemented single-pass double wide rendering as a stereo rendering method fallback for Android devices that do not support single-pass instancing or multi-view.
    2.  Made stereo multi-pass rendering unselectable from the Player Settings when an SRP is in use.
    3.  Unity now automatically selects Single-Pass stereo rendering if multi-pass was previously selected before using an SRP.
    4.  Fixed Android y-flip issues.
    5.  Fixed shadow rendering on all Android platforms when using multi-view stereo rendering.
    6.  Removed the VR watermark on head-mounted displays.
    7.  Removed OpenGL invalid state errors from Android Debug Bridge (ADB) logs.