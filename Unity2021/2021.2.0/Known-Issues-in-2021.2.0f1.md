# Unity 2021.2.0

https://unity3d.com/unity/whats-new/2021.2.0

## Known Issues in 2021.2.0f1

- [Features](#features)
- [Improvements](#improvements)
- [API Changes](#api-changes)
- [Changes](#changes)
- [Fixes](#fixes)


*   Android: Sometimes text is not rendered when using OpengLES3 on a Xiaomi Redmi9A device. ([1347186](https://issuetracker.unity3d.com/issues/android-the-text-is-missing-on-a-xiaomi-redmi9a-device))
    
*   Android: \* Devices might wake up from sleep when in split screen mode.  
    
    *   Chrome OS devices that support tablet mode might not pause apps when they are no longer visible.  
        
    *   Some Android devices may experience delayed resolution updates after resizing a window.  
        
    *   Minimum window size might not be respected properly on all Android devices.
*   Asset Bundles: The build of AssetBundles can be slow when there is a very large filecount. (Z58059\](https://issuetracker.unity3d.com/issues/building-process-of-the-assetbundles-is-slow-when-the-file-count-is-huge))
    
*   Asset Import Pipeline: There is a ArtifactInfo.Internal\_Destroy exception thrown when in Play mode while using Rider debugger. ([1359723](https://issuetracker.unity3d.com/issues/artifactinfo-dot-internal-destroy-exception-thrown-when-in-play-mode-while-using-rider-debugger))
    
*   Asset Import Pipeline: There is a crash in OnDemandScheduler::SetStandbyWorkerCount when opening a project with a symbolic link in it. ([1370389](https://issuetracker.unity3d.com/issues/crash-on-ondemandscheduler-setstandbyworkercount-when-opening-a-project-with-a-symbolic-link-in-it))
    
*   Global Illumination: Scene gets brighter in Standalone player if it was open in the Editor at build time. ([1375015](https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time))
    
*   Global Illumination: Progressive Lightmapper falls back to CPU if only light color was changed. ([1356714](https://issuetracker.unity3d.com/issues/gpu-plm-switch-light-color-only-and-rebake-causes-fallback))
    
*   IL2CPP: System.Runtime.Serialization.Formatters.BinaryFormatter doesn't work when Project is built with IL2CPP Scripting Backend. ([1374185](https://issuetracker.unity3d.com/issues/il2cpp-system-dot-runtime-dot-serialization-dot-formatters-dot-binaryformatter-doesnt-work-when-project-is-build-with-il2cpp-scripting-backend))
    
*   Recent Mac Metal editor change delayed frame updates by 1, affecting selection feedback, keyboard inout and undo/redo. ([1375664](https://issuetracker.unity3d.com/issues/the-first-keyboard-input-is-ignored-and-stored-for-later-when-renaming-assets-causing-all-keyboard-inputs-to-become-mixed))
    
*   Input: Touch Input doesn't work in Play Mode when running an Editor on a Touchscreen device. ([1341159](https://issuetracker.unity3d.com/issues/touch-input-doesnt-work-in-play-mode-when-running-an-editor-on-a-touchscreen-device))
    
*   Mono: Microsoft.Extensions.Logging Nuget Package causes errors in console when built into UWP with .NET Standard 2.1. ([1373389](https://issuetracker.unity3d.com/issues/microsoft-dot-extensions-dot-logging-nuget-package-causes-errors-in-console-when-built-into-uwp-with-net-standard-2-dot-1))
    
*   Mono: NullReferenceException can cause a freeze when thrown in the Player. ([1364311](https://issuetracker.unity3d.com/issues/nullreferenceexception-causes-freeze-when-thrown-in-the-built-project))
    
*   Profiling: GUIStyle errors are thrown when entering Play mode with docked Profiler and the "Maximize On Play" option Enabled. ([1364443](https://issuetracker.unity3d.com/issues/guistyle-errors-are-thrown-when-entering-play-mode-with-docked-profiler-and-the-maximize-on-play-option-enabled))
    
*   Profiling: Profiler's timeline view loses context frames when frames go out of Frame Count bounds. ([1367470](https://issuetracker.unity3d.com/issues/timeline-view-looses-context-frames-when-frames-go-out-of-frame-count-bounds))
    
*   Scene Management: Instantiated FBX through code throws error after leaving Play Mode. ([1363573](https://issuetracker.unity3d.com/issues/instantiated-fbx-through-code-throws-error-after-leaving-play-mode))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Shader System: Shaders are ignored when executing Build Asset Bundles method from console with -nographics argument ([1369645](https://issuetracker.unity3d.com/issues/shaders-are-ignored-when-executing-build-asset-bundles-method-from-console-with-nographics-argument))
    
*   uGUI: Performance regression when loading or unloading a large Scene. ([1375646](https://issuetracker.unity3d.com/issues/poor-performance-when-loading-or-unloading-a-large-scene-1))
    
*   Vulkan: GameObjects textures are seemingly random and change colours depending on the Scene's Camera pos. ([1337772](https://issuetracker.unity3d.com/issues/vulkan-editor-the-scenes-gameobjects-textures-are-seemingly-random-and-change-colours-depending-on-the-scenes-camera-pos))
    
*   XR SDK: \[XR\]\[Linux\] Scene View doesn't render when opening new AR or VR Template project or pressing "Show Tutorials". ([1362435](https://issuetracker.unity3d.com/issues/xr-linux-scene-view-doesnt-render-when-opening-new-ar-or-vr-template-project-or-pressing-show-tutorials))
    

### Features

*   2D: Added a new template to allow users to start a new project with 2D Renderer set up.
    
*   2D: Added support for users to create and define scriptable tools for the _Tile Palette_ window.
    
*   Android: Added a default texture compression format option to **Player Settings**.
    
*   Android: Added support for building and running Android apps on Chrome OS devices with x86 and x86-64 CPUs.
    
*   Android: Added support on Android for split-screen, pop-up and freeform windows.
    
*   Android: Changed so users can now include custom asset packs into the build by adding assets to the directory ending with '.androidpack'.
    
*   Android: When building Android App Bundle with Split App Binary enabled, Unity will create asset packs.
    
*   Asset Import: Added an artifact file dependency system to the AssetImportContext. For more information, see AssetImportContext.GetArtifactFilePath and AssetImportContext.GetOutputArtifactFilePath.
    
*   Asset Pipeline: Added **ArtifactDifference Reporting** messages to the **Artifact Browser**.
    
*   Asset Pipeline: Added Accelerator authentication support using Unity ID.
    
*   Asset Pipeline: Added Import Activity Window. This allows you to look at import times, previous revisions, list dependencies, see importers used and import duration over time.
    
*   Asset Pipeline: Support for importing models and textures in parallel in external processes (off by default, enable in Project Settings ->; Editor ->; Refresh.
    
*   Burst: Added a new optimization mode, `Balanced`. This is now the default optimization mode, and trades off slightly lower maximum performance for much faster compile times.
    
*   Burst: Added an `OptimizeFor` option to `[BurstCompile]`, allowing users to specify whether they want to prioritize runtime speed, runtime size, or compilation time.
    
*   Burst: Added Embedded Linux as a new target platform for Burst.
    
*   Burst: Added Embedded Linux toolchain resolution mechanism.
    
*   Burst: Added experimental half precision floating point type f16.
    
*   Burst: Added experimental support for Arm Neon intrinsics half precision floating point.
    
*   Burst: Added experimental support to the Burst compiler package for some ArmV8.2A intrinsics (dotprod, crypto, RDMA).
    
*   Burst: Added source location metadata into hash cache.
    
*   Burst: Added support for basic vld1 ARM Neon intrinsics.
    
*   Burst: Added support for calling Burst code directly from C# without using function pointers.
    
*   Burst: Added support for creating profiler markers from Burst code.
    
*   Burst: Added support for having `[return: MarshalAs(UnmanagedType.U1)]` or `[return: MarshalAs(UnmanagedType.I1)]` on external functions with a `bool` return type.
    
*   Burst: Added support for new intrinsics.
    
*   Burst: Added support for the C# 8.0 construct `default(T) is null`
    
*   Burst: Added support for the latest LLVM 11 code generation benefits to the Burst compiler package.
    
*   Burst: Added the option to call BurstCompiler.CompileFunctionPointer() in Burst code.
    
*   Burst: Added warnings about delegates being used by `BurstCompiler.CompileFunctionPointer` that are not decorated as expected. In most cases, Burst will automatically add the C-declaration attribute in IL Post Processing, but if the usage of CompileFunctionPointer is abstracted away behind an open generic implementation, then Burst will not be able to automatically correct the delegate declaration, and thus this warning will be displayed.
    
*   Burst: Added workarounds for issues where Windows Native Debuggers restrict the number of messages and DLLs that can be sent to the debugger when attaching.
    
*   Burst: Apple silicon support.
    
*   Burst: Assemblies are now allowed to have an `[assembly: BurstCompile()]` attribute which allows you to specify compile options that apply assembly wide. For example, `[assembly: BurstCompile(OptimizeFor = OptimizeFor.FastCompilation)]`.
    
*   Burst: Burst 1.6 release cycle is for 2021.2.
    
*   Burst: Exceptions thrown from Burst can now contain a callstack.
    
*   Burst: Made it possible to get a pointer to UTF-8 encoded string literal data in HPC# code via StringLiteral.UTF8().
    
*   Burst: The Burst compiler package now fully supports ARMv7 and ARMv8-A Neon intrinsics.
    
*   Burst: To support modding, added support for loading additional burst compiled libraries in Play mode and standalone builds.
    
*   Burst: Unity now automatically adds the `[UnmanagedFunctionPointer(CallingConvention.Cdecl)]` attribute to any delegates that are used for `BurstCompiler.CompileFunctionPointer&lt;&gt;()`. An error occurs if a delegate has the attribute but is not `Cdecl`.
    
*   Core: Added Screen.mainWindowPosition, Screen.mainWindowDisplayInfo, Screen.GetDisplayLayout() and Screen.MoveMainWindowTo() APIs. See Scripting API documentation for more information.
    
*   Editor: Added a **Diagnostics** section to the **Preferences** window to help with remote troubleshooting. You shouldn't interact with this section unless instructed to by Unity Support.
    
*   Editor: Added support for two new menu states, "disabled" and "checked", in Unity Search.
    
*   Graphics: Added _Graphics Buffer Support_ in VFX Graph.
    
*   Graphics: Added a new tool to set the bounds of a VFX Graph system.
    
*   Graphics: Added anisotropic filtering to the built-in inline samplers.
    
*   Graphics: Added support for DX12 on Hololens with OpenXR.
    
*   Graphics: Added support of direct link event.
    
*   IL2CPP: Added new option for "IL2CPP Code Generation" which enables faster and smaller builds by using better sharing of generics code and additional runtime overhead.
    
*   Input System: Released 1.1 of the Input System package with fixes and improvements. Details at https://github.com/Unity-Technologies/InputSystem/blob/develop/Packages/com.unity.inputsystem/CHANGELOG.md.
    
*   License: Introduced licensingIpc Editor CLI.
    
*   macOS: Added deep linking support.
    
*   Mobile: Adapted the scaler profiles so you can easily define and change Adaptive Performance Scalers with predefined profiles.
    
*   Mobile: Added a new adaptive view distance scaler to change the Camera.main view distance automatically.
    
*   Mobile: Added boost mode for Samsung devices. This increases CPU and GPU performance for short periods of time.
    
*   Mobile: Added Boost mode to boost the CPU and GPU for short periods of time.
    
*   Mobile: Added predefined scalar profiles that you can use to easily define and change Adaptive Performance scalers.
    
*   Mobile: Added Startup Boost mode which enables boost mode during engine startup.
    
*   Mobile: Added the ability to enable boost mode during engine startup. This increases CPU and GPU performance for a short period of time as the application starts.
    
*   Mobile: Added the ability to request information about which and how many cores are available on the device.
    
*   Mobile: Added the Adaptive Performance feature API. This checks which Adaptive Performance features are available on the current platform.
    
*   Mobile: Added the Adaptive view distance scaler. This scaler changes the Camera.main view distance automatically.
    
*   Mobile: Added the Feature API to check which Adaptive Performance feature is available on the current platform.
    
*   Mobile: Integrated Adaptive Performance into the Unity Profiler.
    
*   Mobile: Integrated the Profiler so you can Profile Adaptive Performance easily from the Unity Profiler.
    
*   Mobile: Requested cluster info to have details on which and how many cores are available on the device.
    
*   Mono: Enabled Brotli compression for Windows with the Mono runtime.
    
*   Mono: Upgraded to a recent version of Mono (~6.12), which brings most bug fixes from the upstream Mono project.
    
*   Package: (Recorder) Added support for recording accumulation, for motion blur and path tracer (HDRP).
    
*   Package: (Recorder) Integrated the AOV Recorder into the Recorder package.
    
*   Package: Added support for macOS arm64.
    
*   Package Manager: Added new UI support for features in the Package Manager window. Added an initial list of features.
    
*   Package Manager: Added option in the popup window, when _Install_ for a Full Project Asset is clicked, to install the Asset into a new, temporary project.
    
*   Package Manager: Added the ability to install a package from a browser hyperlink, including experimental packages.
    
*   Package Manager: Added UI support for feature sets in the Package Manager window:  
    
    *   Added a Lock/Unlock mechanism on packages that are part of a feature set.  
        
    *   Reset a feature set dependencies to their default versions when the feature set was customized.  
        
    *   Added a warning message if a feature set dependencies are already installed with a different version before installing it.  
        
    *   Added a visual cue on feature sets when the dependency versions change.  
        
    *   Added feature set information to the Inspector.  
        
    *   Added analytics on feature sets.
*   Package Manager: Changed account menu in the top bar of the editor to show your initials instead of full name.
    
*   Package Manager: Changed the Package Manager window so that when users choose to continue from the UPM dialog warning that shows an entitlement error, then launch the Editor, the Package Manager window immediately opens to the first package with an entitlement error.
    
*   Package Manager: Swapped the advanced settings panel and the scoped registries management panel in project settings.
    
*   Package Manager: The Package Manager now supports packages with entitlements (subscription-based licensing).
    
*   Particles: Added a mesh weighting field to the list of meshes in a **Particle System** component, to control how likely Unity is to assign each mesh to a particle.
    
*   Physics: Added a new CustomCollider2D that allows custom 2D physics shapes to be used with a fully customizable and featured 2D Collider.
    
*   Physics: Added an **Enable All** and **Disable All** button to the Physics Project Settings' **Layer Collision Matrix**, which allows enabling or disabling all layer collisions.
    
*   Physics: Added Physics Profiler counters to the list of available counters in the Profiler Module editor window.
    
*   Physics: Added the ability to read low-level 2D physics shapes (PhysicsShape2D) from any 2D Collider into a new shape container (PhysicsShapeGroup2D).
    
*   Physics: Exposed a set of functions to enable you to modify the contact properties of a collision before the solver receives them.
    
*   Profiler: Added ProfilerModule API to extend the Profiler window with custom modules.
    
*   Profiler: Added the _File Access Profiler_ and _Asset Loading Profiler_ modules to the Unity Profiler.
    
*   Profiler: The connection drop down has been revamped into a tree view that groups player connections int0 three main categories. Local, any player that is running local to the machine, this includes devices connected via cable. Remote any player that is running anywhere else on the network that is reachable. Direct connection, this is for connecting directly via IP address or any player that has automatically connected. There options are further searchable using the new search bar.  
    Any connections to players which exist from before this feature will still appear though they will appear under the category of "Connection Without Id".  
    Further to this there no exists an option that can be used to supply a custom connection name for the profiler which will make it easier for the user to find their desired connection. This is set through the Preferences->;Anaylsis option or via the command line "-connection-id" when launching a player from the command line.
    
*   Scene/Game View: Added support for component tools to the **EditorToolContext**.
    
*   Scene/Game View: Introduced new Overlays feature. Tools and contextual views are now available directly in the Scene View, and are completely customizable.
    
*   Search: Added a new explicit provider to search performance metrics.
    
*   Search: Added new extended search picker workflow and API.
    
*   Search: Added search expression language to evaluate multiple search queries and apply set operations, transformation or other user defined operations.
    
*   Search: Added search table support to build advanced reports using complex search expressions.
    
*   Shaders: Added support for specifying package requirements for SubShaders and Passes to ShaderLab.
    
*   Shaders: Introduced keyword space separation.  
    Shaders, compute shaders and materials now operate in separate local keyword spaces. All keywords declared in a shader or in a compute shader using any of the multi\_compile\* or shader\_feature\* directives are local. Material and Compute Shader classes now operate with local keywords only.  
    Global keyword space contains global keywords. Global keywords are converted to local keyword space of a shader or compute shader prior to rendering. When a shader or a compute shader declares a keyword that has the same name as a global keyword, turning this global keyword on or off will affect variant selection.
    
*   Terrain: Added a new instancing mode for Terrain details, which uses the material specified on the prototype prefab to render detail objects with instanced draws.
    
*   UI: Added preference to enable or disable extended Dynamic Hints.
    
*   UI Toolkit: Added a context action in the UI Builder Hierarchy to export an element to a UXML file.
    
*   UI Toolkit: Added a contextual action to unpack a template in a document in the UI Builder.
    
*   UI Toolkit: Added contextual actions to unpack a template completely in UI Builder.
    
*   UI Toolkit: Added runtime access to the PanelSettings object and the UIDocument component. Runtime UIToolkit rendering no longer requires the UIToolkit package.
    
*   UI Toolkit: Added support for negative transform scaling on x and y axes, enabling mirroring to be performed. When crossing zero, the geometry will be regenerated to flip the winding.
    
*   UI Toolkit: Added support for rendering antialiased vector shapes without MSAA in UI Toolkit.
    
*   UI Toolkit: Added support for up to 7 levels of stencil-based masking.
    
*   UI Toolkit: Added the DynamicColor usage hint that allows border/background/text color to change dynamically without having to regenerate the geometry.
    
*   UI Toolkit: Added transform-origin, rotate, scale and translate to the supported properties by UI Toolkit.
    
*   UI Toolkit: Added Transitions properties to the UI Toolkit.
    
*   UI Toolkit: Attribute overrides can be added, edited and removed in a template instance using UI Builder.
    
*   UI Toolkit: ListView now supports dynamic item height as a virtualization method. For more information, see ListView and CollectionVirtualizationMethod.
    
*   UI Toolkit: Updated the UIElementsGenerator tool to the latest version.
    
*   Version Control: Added auto sign in when logged into Unity account.
    
*   Version Control: Added workspace migration from Collab to Plastic which can be done with or without Plastic installed.  
    Added notification status icons.  
    Added light and dark mode versions of the avatar icon.
    
*   Version Control: Improvements to Plastic SCM:  
    
    *   Added support for inviting other members. This option is available from the gear / settings icon.  
        
    *   Added support for signing in with Cloud Edition. This is available during the onboarding screen if you have never signed in.  
        
    *   Added support for turning off Plastic in their project. This option removes the Plastic metadata from your directory. This option is available under Assets >; Plastic SCM >; Turn off Plastic SCM  
        
    *   Added notification on the Plastic SCM tab title to indicate incoming changes. Users will no longer need to have the Plastic SCM window visible to know there are incoming changes.  
        
    *   Auto configuration of SSO  
        
    *   Added date column in incoming changes
*   WebGL: Added support for compressed audio in WebGL.
    
*   WebGL: Added the _Debug Symbols_ player setting to create release builds with embedded function symbols for improved profiling and error stack traces.
    
*   WebGL: Added the texture subtarget build setting to WebGL.
    
*   WebGL: Enabled ETC/ETC2/ASTC/BC4/BC5/BC6/BC7 compressed texture formats for WebGL in editor, build and runtime.
    
*   XR: Added support for controller late latching, which can reduce latency between rendering and tracked input (head and hand-held controller) in XR. Can be used with the Mesh Renderer and the Skinned Mesh Renderer.
    
*   XR: Reduced render latency in URP with Late Latching.
    

### Improvements

*   2D: Added folder support for SpriteAtlas V2 in 2D.
    
*   2D: Cached internal reflection to speed up Sprite editing data access.
    
*   2D: Improved performance for setting multiple Tiles on a Tilemap.
    
*   2D: Improved performance of RuleTile caching.
    
*   2D: Improved performance when importing large number of textures.
    
*   2D: Improved the placement of Tiles generated from Sprites with Textures sliced using the Isometric Slicing option in the Sprite Editor.
    
*   2D: Prereleased the SpriteShape and PSDImporter package
    
*   2D: Updated icons for the Tile Palette Rotate and Flip tools.
    
*   2D: Updated the 2D template to use the latest verified 2D packages.
    
*   2D: Updated the 2D URP template starting folder structure for better clarification of usage.
    
*   2D: Updated the Skinning Editor tooltips text.
    
*   AI: Added the `RasterizeModifierBox` profiler marker for the NavMesh builder step that processes ModifierBox sources.
    
*   Android: Added a new Android/Chrome OS player setting, "Chrome OS Input Emulation". If un-checked, this option disables Chrome OS's default behavior of converting mouse and touchpad events into touchscreen events. This allows an app to implement more complete support for these input devices. Also, fixed a bug with Android/Chrome OS touchpad scrolling.
    
*   Android: Added boot-config/command-line switch `platform-android-cpucapacity-threshold`. This specifies which CPU cores to treat as big cores. The cpu capacity is a value in the range between 0 and 1024. A capacity value of 870 yields the same behavior as before the fix for case 1349057.
    
*   Android: Added support for custom cursors to Android to support Player Settings and C# functions on Android version 7.0 and later.
    
*   Android: Allow low-level configuration of Unity threads (priority, affinity)
    
*   Android: Changed the device scanning operation of the Android Extension to be async when receiving an USB device changed event. ([1349380](https://issuetracker.unity3d.com/issues/opening-project-which-doesnt-target-android-stall-for-a-few-seconds-with-scanning-for-usb-devices))
    
*   Android: If a hardware keyboard is available, Unity now uses it within UI systems, instead of always bringing up a virtual, on-screen keyboard.
    
*   Android: Made a large part of the Android Build Pipeline incremental which means sequential builds with zero changes are now much faster. That also means Unity no longer creates builds from scratch, but instead updates the files which dependencies have changed. If you use the IPostGenerateGradleAndroidProject callback, note that it might be operating on files which were modified by IPostGenerateGradleAndroidProject from a previous build.
    
*   Android: Unity gradle projects now have a new entry in gradle.properties, unityTemplateVersion. Unity increments this property whenever Unity gradle template files change. That way if you build on top of the old folder and the unityTemplateVersion is different, Unity throws an error, saying that you need to update your gradle files or build to an empty folder.
    
*   Android: When generating manifest files, there are new files in Library\\Bee\\artifacts\\Android\\Manifest, LibraryManifestDiag.txt, LauncherManifestDiag.txt. They contain information about why a specific permission is added to manifest.
    
*   Asset Bundles: Added profile marker for CRC checks.
    
*   Asset Import: Documented the `MonoImporter` class.
    
*   Asset Import: Improved FBX model importing speed.
    
*   Asset Import: Improved import performance of ASCII FBX files.
    
*   Asset Import: Improved import performance of FBX files.
    
*   Asset Import: Improved import speed for FBX files that use the ASCII file format.
    
*   Asset Import: Improved import speed for model files containing more than 1 mesh.
    
*   Asset Import: Improved import speed of FBX models by skipping unused data.
    
*   Asset Import: Improved import speed of models that contain multiple meshes.
    
*   Asset Import: Improved import speed of Sketchup models.
    
*   Asset Import: Improved model import speed by multithreading mesh triangulation.
    
*   Asset Import: Improved model import times for models that contain animations.
    
*   Asset Import: Improved Model Importer material tab display performance. (1295743)
    
*   Asset Import: Improved model importing performance for files that contain lots of curves.
    
*   Asset Import: Improved the model import times slightly for models that contain animations.
    
*   Asset Import: Increased the speed of Asset Import when using mikktspace tangent generation on meshes containing degenerate triangles.
    
*   Asset Import: Optimized the texture import mipmap calculation when using Kaiser filtering. For example, importing 16GB of textures with mostly Kaiser mip filters is reduced from 127 seconds to 109 seconds.
    
*   Asset Import: Reduced peak memory usage during Model Importing.
    
*   Asset Import: Updated Sketchup SDK to version 2020.2.
    
*   Asset Pipeline: Added a new UI in the AssetImporter inspectors that display all AssetPostprocessors methods that were used in the last import of the selected asset.
    
*   Asset Pipeline: Added summary in the editor log about what happened during a refresh (import).
    
*   Asset Pipeline: Added warnings and an _Automatic Fix_ button where main object names do not match the corresponding filename.
    
*   Asset Pipeline: Improved directory enumeration by multi-threading it.
    
*   Asset Pipeline: Improved project startup times. Projects with 900,000 files will load at least 30 seconds faster.
    
*   Asset Pipeline: Improved speed of Editor startup by fixing Asset handling related code.
    
*   Asset Pipeline: Improved startup performance for 900,000 file project by 18 seconds.
    
*   Asset Pipeline: Improved upload and download path.
    
*   Asset Pipeline: Optimized the UnityEngine.Hash128.ToString method.
    
*   Asset Pipeline: The Asset Pipeline no longer displays a warning when it is not possible to move import worker log files.
    
*   Asset Pipeline: Unity prefetches Asset Databases to improve Editor startup time and reduce cost of page faults.
    
*   Audio: Added a new _Attenuation_ transition type to AudioMixer so that it can perform equal power panning for group attenuations when transitioning between snapshots. (1322673)
    
*   Audio: Added voice priority display in the audio pane of profiler.
    
*   Audio: Added VU metering information from audio mixer groups in the audio pane of profiler to make it easier to compare it against volume and audibility levels.
    
*   Audio: Improved the way Unity displays audio mixers inside the Audio Profiler window when the Groups and Channels and Groups view modes are enabled.  
    Previously, Unity applied the column-based sorting from the Channels view mode to the other view modes, which resulted in inconsistent sorting of channels and groups below mixers, and in mixers changing their order dynamically. This made the Audio Profiler window hard to read.  
    Unity now shows the names of the mixers in the Profiler where it previously only showed the ambiguous Master groups of the mixers below the Audio Listener group.  
    The triangle shape after the titles of the column headers in the Detailed and Clip views was changed to an arrow that more clearly indicates the sorting order. The arrow is now placed before the title instead of after it to avoid cutting the title off when you resize the columns manually.
    
*   Audio: Target mixer groups are now displayed in the audio profiler.
    
*   Bug Reporter: The Crash Handler window now includes the following UI changes:  
    
    *   _Stack trace_ field  
        
    *   _Go to crash logs_ button  
        
    *   _Report a Bug..._ button  
        
    *   _Open Unity Hub_ button  
        Note that clicking the _Open Unity Hub_ button restarts the Editor.
*   Build Pipeline: "Scripts Only Build" is now automatic for platforms using the new incremental build pipeline. The checkbox is removed for such platforms, and Unity will automatically detect if it can do a Scripts Only Build based on which changes there are in the project.
    
*   Build Pipeline: Changed Linux so that it uses the incremental player build pipeline.
    
*   Build Pipeline: Improved linking speed for big projects
    
*   Build Pipeline: Improved the performance of the build pipeline by giving concurrent shader cache folders read access.
    
*   Build Pipeline: MacOS Standalone player builds now use the new incremental build pipeline, which allows faster subsequent player builds by only rebuilding parts which have changed.
    
*   Build Pipeline: Modified Windows Standalone player builds so that they only rebuild parts that have changed since the previous build to improve build speed.
    
*   Build Pipeline: Removed prompt to save an untitled scene if it is not included in the build.
    
*   Build Pipeline: WebGL now uses the incremental Player build pipeline.
    
*   Burst: Automatically add \[UnmanagedFunctionPointer(CallingConvention.Cdecl)\] to any delegates that are used for BurstCompiler.CompileFunctionPointer<;>;() or error if the delegate has the attribute and it is not Cdecl.
    
*   Burst: Improved codegen.
    
*   Core: Modified the Dynamic Heap Allocator to reduce the time it takes to intantiate chunks in a Build. ([1272168](https://issuetracker.unity3d.com/issues/slower-performance-of-instantiate-when-using-it-in-a-build-compared-to-the-editor))
    
*   Core: Reduced the number of memory alllocations and improved the tracking of core allocations.
    
*   Documentation: Added a pop-up to Obsolete API labels in the Script Reference, explaining why something is obsolete, and pointing to the new API where possible.
    
*   Documentation: Improved documentation for GeometryUtility.TestPlanesAABB to explain false positives.
    
*   DX12: \*Binded dynamic lightmaps resources (Enlighten) to ray tracing shaders: `unity_DynamicLightmap`, `unity_DynamicDirectionality` and `unity_DynamicLightmapST`. \*Enabled `DYNAMICLIGHTMAP_ON` shader keyword for when these resources are used by Renderers.
    
*   DX12: Added the ability to set D3D12\_RAYTRACING\_GEOMETRY\_FLAG\_NO\_DUPLICATE\_ANYHIT\_INVOCATION flag when adding Renderers to a RayTracingAccelerationStructure. This will allow implementation of robust colored ray traced shadows.
    
*   DX12: Optimized uniform setup in ray tracing shaders, and added a special case for the `UnityPerMaterial` cbuffer.
    
*   Editor: Added a context menu to the Console window which has an option to use monospace font. (1276112)
    
*   Editor: Added ability to reorder UnityEvent callbacks.
    
*   Editor: Added missing USB device detection and reporting for Linux Editors.
    
*   Editor: Added new devices to the Device Simulator:  
    
    *   Apple iPad Air 2  
        
    *   Apple iPad Air (4th generation)  
        
    *   Apple iPhone 12 mini  
        
    *   Apple iPhone 12  
        
    *   Apple iPhone 12 Pro  
        
    *   Apple iPhone 12 Pro Max  
        
    *   Apple iPhone SE (2nd generation)  
        
    *   Google Pixel 5  
        
    *   Huawei P40 Pro  
        
    *   OnePlus 7 Pro  
        
    *   Samsung Galaxy Z Fold2 5G  
        
    *   Samsung Galaxy Note10  
        
    *   Samsung Galaxy Note10+ 5G  
        
    *   Samsung Galaxy Note20 Ultra 5G  
        
    *   Samsung Galaxy S8  
        
    *   Samsung Galaxy S9  
        
    *   vivo NEX 3 5G  
        
    *   Xiaomi Mi A3.
*   Editor: Added new features for Menu Items in the context of Editor Modes.
    
*   Editor: Added Open in Property Editor menu item to the Inspector's kebab menu. (1334342)
    
*   Editor: Added profiler markers around test setup, teardown, and execution.
    
*   Editor: Added Texture import overrides to the Build Settings window so you can reduce imported texture size and change the compression settings to speed up asset imports and platform switches.
    
*   Editor: Added the **Play Unfocused** option to the Game view, to stop the Game view from focusing when entering Play mode. Also added an option to **Edit** &gt; **Preferences** &gt; **General** to enable or disable automatically creating a Game view on entering Play mode.
    
*   Editor: Added the ability to cut, copy, and paste Assets in ProjectWindow. (1264821)
    
*   Editor: Added the ability to search Settings by their properties.
    
*   Editor: Added the option to constrain scale proportions to the Transform component. You can set this option as default in Editor preferences.
    
*   Editor: Added the renderer type to the UpdateRendererBoundingVolumes profile marker tooltip.
    
*   Editor: Allowed the importing of LOD meshes with indices that have preceding zeroes. By specifying a range, e.g., LOD1-3 will assign the mesh to all LOD levels in the range.
    
*   Editor: Avoid stall entering playmode if a scene contains sequential GameObject file ID hints. ([1308128](https://issuetracker.unity3d.com/issues/entering-play-mode-takes-upwards-of-1-hour-when-auto-generating-high-amounts-of-objects))
    
*   Editor: Cached the translation results, reducing GC pressure.
    
*   Editor: Changed the popup menu behaviour to only trigger a `GUI.changed` event if it has changed.
    
*   Editor: If the assembly containing code that is stalling the editor is available, it's now displayed in the popup progress bar.
    
*   Editor: Improved Gizmos performance in Editor.
    
*   Editor: Improved import times of SketchUp models (\*.skp).
    
*   Editor: Improved loading times for scenes with lots of GameObjects at the top level in the Hierarchy.
    
*   Editor: Improved mac editor process guard in order to catch all types of exceptions and early handle cases before shutting down.
    
*   Editor: Improved model importing performance.
    
*   Editor: Improved performance importing models with Blendshapes if the Import Blendshapes setting is unchecked.
    
*   Editor: Improved the Frame Debugger, so you can clear display color, depth, and stencil values. The compute shader displays the display shader name, keywords, and thread group size. Indirect draws display shader and property information. The Mesh preview now displays correctly on HDRP. Displays SRP Batcher draws with the names of meshes they render.
    
*   Editor: Improved the performance of the model importer by multi-threading the mesh triangulation step.
    
*   Editor: Improving UTF documentation (DSTR-120).
    
*   Editor: Increased speed of filtering operations when you only run a subset of tests.
    
*   Editor: Inspector number fields support more math expressions now: functions (`sqrt`, `sin`, `cos`, `tan`, `floor`, `ceil`, `round`), distribution over multi-selection (`L`, `R`) and can refer to current value to change it across multi-selection (`+=3`, `*=2`).
    
*   Editor: Now shaders will have SHADER\_API\_(DESKTOP|MOBILE) define set according to the target build platform.
    
*   Editor: Optimized BC7 ("high quality" compression setting on PC/Console platforms) texture compression. Performance is 2-3 times faster. This optimization uses a new texture compressor (bc7e). An option is available in Editor Settings to switch to the old one (ISPC) if needed.
    
*   Editor: Optimized drag selection in Editor scenes.
    
*   Editor: Reduced the per-test overhead of running tests in the editor.
    
*   Editor: Reduced the time taken to rebuild the test tree and to scan for assets a test created but did not delete.
    
*   Editor: Removed the Enable Code Coverage option from Preferences/General, and moved it into the Code Coverage package.
    
*   Editor: Reorganized Quality Project Settings, to make it clearer which options are relevant to which parts of Unity. (1307483)
    
*   Editor: The Frame Selected command now ignores Audio Source and Reverb Zone components.
    
*   Editor: The Texture Import Settings window indicates which platforms have override settings. The window shows this with a blue line on the platform tabs.
    
*   Editor: UI polish of Build Settings window (improved logical sort of installed platforms).
    
*   Editor: Updated ASTC texture compressor to improve compression time by about 10%.
    
*   Editor: Updated ASTC texture compressor to reduce compression time.
    
*   Editor: Updated the Inspector property context menu 'Revert to Prefab' to work with multiple selected objects.
    
*   Editor: Updated the Renderer component so that you can click on a Material inside the Renderer component to highlight the Sub Meshes with that Material in the Scene View.
    
*   Editor: Updated the target window of a Dynamic Hint to be focused before displaying the Dynamic Hint, if available.
    
*   Editor: You can now drag multiple GameObjects to the Project Window to create multiple prefabs at once.
    
*   Editor: `Create Empty Parent` now matches the 'selection rect' for Rect Transforms.
    
*   GI: Added support for asynchronous environment sky updates to Enlighten Realtime Global Illumination to reduce the likelihood of frame hitches when the sky changes.
    
*   GI: Added support for rectangular area lights to Enlighten Realtime Global Illumination.
    
*   GI: Clarified the Indirect Bounce Shadow warning in the **Light Inspector** to indicate that Enlighten Realtime Global Illumination only supports this feature for Directional lights.
    
*   GI: Ensured that analytics data about cancelled bakes are logged when the Editor closes while baking lighting. ([1354238](https://issuetracker.unity3d.com/issues/fatal-error-when-closing-the-editor-while-generating-lighting))
    
*   GI: Extended support for the Lit Clustering Scene View exposure control so that it is available for lightmaps created with Enlighten Baked Global Illumination.
    
*   GI: Hid the **Show Inactive Objects** and **Isolate Selection** checkboxes on the Static Emissives tabs of the Light Explorer because these options are not applicable to materials. ([1331750](https://issuetracker.unity3d.com/issues/show-inactive-objects-and-isolate-selection-checkboxes-are-shown-static-emissives-tab-of-light-explorer-but-are-pointless))
    
*   GI: Improved clarity in the GI Profiler by indicating whether the project's render pipeline supports Enlighten Realtime Global Illumination.
    
*   GI: Improved performance by running GICache trimming jobs every 30 seconds. ([1289849](https://issuetracker.unity3d.com/issues/gicache-over-max-size-is-not-reduced-and-warnings-are-spammed-in-the-console))
    
*   GI: Improved usability by including memory-related logs in the Editor log.
    
*   GI: Lightmap analytics events now include bakes that fell back from GPU to CPU Lightmapper.
    
*   GI: Reduced ringing in lightmaps filtered with Intel Open Image Denoise.
    
*   GI: Removed the **Compress Lightmaps** option and replaced it with a configurable **Lightmap Compression** setting in the Lighting Settings Asset. ([1230918](https://issuetracker.unity3d.com/issues/lightmap-encoding-quality-settings-do-not-apply-to-baked-lightmap-textures))
    
*   GI: Removed unnecessary thread logging for Enlighten Realtime Global Illumination to improve performance.
    
*   GI: Upgraded Radeon Denoiser support to to version 1.7.0 in order to improve results generated in HDR mode.
    
*   Graphics: Added an error message that appears when a custom render texture uses a Material with an invalid or unsupported shader. (1304355)
    
*   Graphics: Added ASTC texture format support for single channel textures.
    
*   Graphics: Added support for async readback when using OpenGL ES 3.0 (and later) and GL core.
    
*   Graphics: Added support for Color and Depth Load/Store actions to the Frame Debugger.
    
*   Graphics: Added support for `VFX.CameraBuffersFallback` preferences. Select from one of 3 options:  
    
    *   **None**: Use no fallback and keep outdated buffer info from the last rendered frame.  
        
    *   **Prefer Main Camera** (Default): Use the buffer from the Main camera when available, and the Scene camera otherwise.  
        
    *   **Prefer Scene Camera**: Use the buffer from the Scene camera when available, even if the Main camera is being rendered.
*   Graphics: Added the _2D Lights_ tab to the Light Explorer window.
    
*   Graphics: Added the ability to remove shader Passes that contain ray tracing shaders (for example, `ClosestHit`, `AnyHit`) when ray tracing is not supported by the system or graphics API.
    
*   Graphics: Added two new functions in RayTracingAccelerationStructure - UpdateInstanceID and GetInstanceCount. The ray tracing instance ID can be accessed in HLSL code using InstanceID() intrinsic.
    
*   Graphics: Changed Renderer components so that you can use `.bounds` and `.localBounds` setter APIs to set custom world space or local space bounds.
    
*   Graphics: Changed the default specular reflection to use a RenderTexture with dimensions CUBE (instead of a Cubemap). (1281013)
    
*   Graphics: Changed the gear icon for the more menu on the Asset Settings Provider.
    
*   Graphics: Enhanced the error reporting from the command buffer in order to improve GPU-side (Metal) error logging.
    
*   Graphics: Fixed comments in shader examples from CommandBuffer.SetRayTracingShaderPass and RayTracingShader.SetShaderPass that point to incorrect functions.
    
*   Graphics: Improved ASTC decompression performance.
    
*   Graphics: Improved error logging for the `CopyTexture` function.
    
*   Graphics: Improved the application of outstanding pending changes to RendererScene after a camera render.
    
*   Graphics: Optimized render sorting to speed up performance.
    
*   Graphics: Optimized `Material.FindPass`. The improved speed depends on how many passes the Material has.
    
*   Graphics: Removed the redundant calls that Unity made when it set shader program parameters.
    
*   Graphics: Set up unity\_MotionVectorsParams built-in shader variable in Ray Tracing shaders.
    
*   Graphics: Split texture postprocessor re-imports by texture type to reduce the amount of re-imports when changing a texture postprocessor script.
    
*   Graphics: Unity can now preload shaders after it loads the first Scene, and can distribute the preloading process across multiple frames.
    
*   Graphics: Unity now opens the _Render Pipeline Asset_ dialog when changing asset for Quality Settings and Graphics Settings (_Project Settings >; Quality, Project Settings >; Graphics_) notifying that this may take a significant amount of time. You can choose to Continue or Cancel.
    
*   Graphics: VFX : Optimization while sending event to a VisualEffect by script.
    
*   Graphics: Virtual Texturing is now more robust when switching between color spaces.
    
*   Graphics: You can now access Mesh and SkinnedMeshRenderer geometry data from Compute Shaders similar to `Mesh.GetVertexBuffer` and `SkinnedMeshRenderer.GetVertexBuffer`.
    
*   IL2CPP: Added an intrinsic for Span get\_Item/indexer to improve Span Indexer performance when accessing a large number of Span items.
    
*   IL2CPP: Added full support for System.Reflection.MemberInfo.GetCustomAttributesData.
    
*   IL2CPP: Added optimizations to Enum.HasFlag.
    
*   IL2CPP: Changed IL2CPP's internal build system to use bee on Android to prepare for improved player build performance.
    
*   IL2CPP: Changed il2cpp's internal buildsystem on Windows & Mac to prepare for improved player build performance.
    
*   IL2CPP: Corrected the source file hash so that a managed debugger can determine when a source file has changed and provide a proper warning.
    
*   IL2CPP: Improved the performance for invoking delegates.
    
*   IL2CPP: Improved the performance of IL2CPP conversion by using a new data model.
    
*   IL2CPP: Reduced executable size by reducing generic metadata output.
    
*   IL2CPP: Reduced the number of internal metadata allocations that relate to array method naming.
    
*   IL2CPP: Switch IL2CPP densehash map and set to sparsehash map and set for lower runtime memory usage.
    
*   IL2CPP: Updated IL2CPP to run on .NET 5.
    
*   IL2CPP: Updated IL2CPP to use the new bee distribution format.
    
*   IMGUI: Improved overall layout and repaint performance.
    
*   Input: Added _Use Physical Keys_ setting in the Input Manager to map Input.KeyCode to physical keys.
    
*   iOS: Changed depth RenderSurfaces to have private storageMode. (1339864)
    
*   iOS: Changed how plug-ins handle the wrong CPU type when creating an XCode project. CPU types that aren't supported are now ignored.
    
*   iOS: The generated Xcode project now uses the new build system.
    
*   Kernel: Added Memory Settings to the Project Settings window. This gives you control of the internal memory setup in Unity. You can adjust the memory setup for individual projects.
    
*   Kernel: Improved code quality and amount of allocations in some of our base abstraction layers.
    
*   Kernel: Improved the performance of parallel sorting code.
    
*   Kernel: Improved the stability of player connection by implementing several changes:  
    
    *   Increased the number of frames to receive messages.  
        
    *   Fixed issue where player connection could corrupt message queue and required reconnecting to app.  
        
    *   Improved handling for app disconnection (for example, when the app crashes; when the app is forced to disconnect; or when the app loses connection).  
        
    *   Improved support for suspending apps on mobile platforms.
*   License: Improved license validation by syncing the access token with the licensing client every time the token changes.
    
*   macOS: Fixed the append mode for building Xcode projects.
    
*   macOS: The generated Xcode project now uses the new build system.
    
*   macOS: When generating Xcode project, it is now possible to pick the build config used for run action (can be changed in Xcode). Debug build config now has frame capture automatically enabled.
    
*   Mobile: The _Android Patch/Patch & Run_ Build Setting works for all types of changes, and is automatic. Previously, it could only be used with Script Only builds.
    
*   N/A (internal): Altered default texture compression for EmbeddedLinux to now be configurable from the player settings.
    
*   Networking: Improved UnityWebRequest on iOS to allow system to call upload data instead of using the operation queue.
    
*   Package: Enabled alpha channel capture in projects that use _HDRP_ in the _Recorder package_.
    
*   Package: Improved the migration tools so that Unity allows projects to migrate to the recent Visual Scripting version.
    
*   Package: To open the Visual Scripting editor, you can now click the open inspector button and double click a graph in the project browser.
    
*   Package: Updated names of UI elements in the Visual Scripting package to be consistent with new naming schemes.
    
*   Package: Updated the user interface of the Visual Scripting package.
    
*   Package: Visual Scripting now creates a warning message when you add more than one Input unit to a SuperUnit.
    
*   Package: Visual Scripting now creates a warning when an Input System Package event references an action that is the wrong type for that event.
    
*   Package: Visual Scripting: Migration tools are improved to let users migrate their project to the latest version of the Visual Scripting package.
    
*   Package Manager: Added new labels to package versions to clarify when a package is installed as a dependency.
    
*   Package Manager: Added support for opt-in caching of Git LFS files when you download Git packages. To enable caching, set either of the following environment variables: `UPM_ENABLE_GIT_LFS_CACHE` or `UPM_GIT_LFS_CACHE_PATH`. The latter lets you override the default cache location.
    
*   Package Manager: Changed how string literals are translated by using string.Format at definition time.
    
*   Package Manager: Fixed the _Add package from git URL_ option so that if you use a revision and a package path in the wrong order, you can't clone the repository.
    
*   Package Manager: Improved logging by adding logs for cache misses and tarball download steps.
    
*   Package Manager: Improved performance when browsing "My Assets".
    
*   Package Manager: Improved the error message when a Git dependency cannot be resolved because the path querystring and revision fragment are in the wrong order.
    
*   Package Manager: Improved the wording on the warning message when a user is using a different version of a package than the recommended version.
    
*   Package Manager: Included the Terrain Tools package in the Worldbuilding 3D feature set.
    
*   Package Manager: Increased the amount of information logged in `upm.log` at various levels.
    
*   Package Manager: Optimized Git package download times for repositories using submodules (with Git 2.28.0 or higher installed only).
    
*   Package Manager: Optimized Git package download times, most notably for repositories with a larger history.
    
*   Particles: Added a warning when users select the same shader for both the main Material slot and the Trail Material slot. This is because GPU Instanced Mesh particles must not use the same shader for particle geometry and trail geometry.
    
*   Particles: Added an exception when too much particle data is sent to `SetCustomParticleData`.
    
*   Physics: Added icon for Articulation Body Anchor Transform tool.
    
*   Physics: Added new Physics Profiler metrics.
    
*   Physics: Added units of measurement to the Articulation Body properties in the scripting documentation.
    
*   Physics: Improved Articulation Body anchor limit gizmos.
    
*   Physics: Rearranged the ArticulationBody properties. Moved Damping and Friction after Mass.
    
*   Prefabs: Added a warning to the PrefabAssetImporter editor if there are SerializeReference missing types within the Prefab. Also disabled applying modifications from the instance in case the Prefab asset contains missing types. Editing the Prefab asset in isolation preserves MissingType information.
    
*   Prefabs: Disabled editing for missing Prefabs instances.
    
*   Prefabs: Improved the Hierarchy so that you can see which Prefab instances have non-default overrides. (1323680)
    
*   Prefabs: Updated documentation for Object.DontDestroyOnLoad
    
*   Profiler: Added missing memory labels sizes to the memory snapshot format, in order to give real value to the prexisting label list. Api for access this data will be found inside the memory profiler package.
    
*   Profiler: Added profiler memory stats data. Data is similar to the Profiler Module data found in the Profiler Window
    
*   Profiler: Added profiler target data to memory snapshot format. Data consists of elements such as Unity version, product name, total gfx memory, total physical memory, etc.
    
*   Profiler: Encoded managed heap section type inside the snapshot format, for retrieval via the memory profiler package.
    
*   Profiler: Improved the Memory Profiler module UI to clearly show how the high level memory stats contribute towards the total memory usage.
    
*   Profiler: Modified native connection reporting for the Memory Profiler in order to properly report connections between Assets.
    
*   Profiler: Tethered Android devices no longer require manually calling ADB commands in the CLI, in order to be picked up as connection targets by the Editor. Multiple tethered android devices are now supported.
    
*   Scene/Game View: Added Shortcut Manager entries for "Toggle Selection Outline" and "Toggle Selection Wireframe."
    
*   Scene/Game View: Extended the `PlaceObject` method to support SceneView grids and 2D.
    
*   Scene/Game View: Improved API documentation for Overlays feature, including multiple new code examples.
    
*   Scene/Game View: Improved the _EditorToolContext_ UI.
    
*   Scene/Game View: Improved the documentation for `EditorTool`.
    
*   Scene/Game View: Improved the documentation for `HandleUtility.PickGameObject`.
    
*   Scene/Game View: Refreshed icons for Scene View toolbars.
    
*   Scripting: Certificate validation callbacks from .Net libraries pass now also previously identified root certificates along (i.e. the full validated chain if any). ([1191987](https://issuetracker.unity3d.com/issues/dropbox-api-v2-file-upload-fails-and-argumentoutofrangeexception-is-thrown-when-calling-uploadsessionstartasync-method))
    
*   Scripting: Changed the Managed Stripping Level to be minimal for new projects when targeting the IL2CPP backend.
    
*   Scripting: Enabled user code to build against .NET Standard 2.1 and .NET Framework 4.8.
    
*   Scripting: Ensure players using the Mono scripting runtime backend always use a JIT (Just-In-Time) friendly set of class libraries, even if the ".NET Standard 2.0" API Compatibility Level is chosen. This provides consistency for Mono players no matter what API Compatibility Level is chosen in the player settings.
    
*   Scripting: Improved runtime performance of many UnityEngine math scripting APIs when using the IL2CPP scripting back-end: Color, Color32, Math, Matrix4x4, Quaternion, Vector2, Vector2Int, Vector3, Vector3Int, Vector4.
    
*   Scripting: Improved runtime performance of UnityEngine math scripting APIs (Matrix4x4, Quaternion, Vector2, Vector2Int, Vector3, Vector3Int, Vector4) when using the Mono scripting back-end.
    
*   Scripting: Improved search UI and indexing.
    
*   Scripting: Improved the Editor experience for setting up Unity version defines with assembly definition files.
    
*   Scripting: In this Unity version, you can schedulw managed jobs from non-main control threads.
    
*   Scripting: Multithreaded asset garbage collection and increased speed by up to 2.5x.
    
*   Scripting: OnChangedCallback is invoked when elements are duplicated in ReorderableList. (1307386)
    
*   Scripting: Reduce and optimize regex usage to improve performance
    
*   Scripting: Renamed ".NET Standard" to ".NET Standard 2.1" in the Api Compatibility Level options.
    
*   Scripting: Updated C# language version to 9.0 for compilation and IDE's  
    We will support a subset of the language features from:  
    https://docs.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-9  
    These is the features that we support:  
    
    *   Pattern matching enhancements  
        
    *   Function pointers  
        
    *   Target-typed new expressions  
        
    *   Static anonymous functions  
        
    *   Target-typed conditional expressions  
        
    *   Extension GetEnumerator support for foreach loops  
        
    *   Lambda discard parameters  
        
    *   Attributes on local functions  
        
    *   New features for partial methods.
*   Scripting: `CompiliationPipeline.GetAssemblies` now correctly includes .NET Compiler Platform (Roslyn) analyzers in `ScriptCompilerOptions`.
    
*   Search: Improved asset indexer performances and index size.
    
*   Search: Improved asset search performance by ~4x.
    
*   Search: Share the same search debouncing threshold with the Project Browser and the Search window. ([1298380](https://issuetracker.unity3d.com/issues/project-browser-search-has-slower-response-when-compared-to-quick-search-and-hierarchy-search))
    
*   Search: Use a single Search Provider to search for any indexed object.
    
*   Serialization: Improved the way that `SerializeReference` handles missing types. Instances where the type is missing are replaced with `null`. Other instances are editable and if there are fields that previously referred to the missing type which are still null, the missing type is preserved.
    
*   Serialization: Objects referenced from `SerializeReference` fields now have stable IDs, which reduces the risk of conflicts when multiple users collaborate on a scene file. Additionally, it also improves support for Undo and Prefab modes, especially when `SerializeReference` is used inside arrays and lists. In addition, references now come with a new format with backward compatibility support for older assets.
    
*   Shadergraph: Added View Vector Node doc.
    
*   Shaders: Improved caching of the Shader import artifacts when a shader is reverted or has no changes after a reimport.
    
*   Shaders: Reduced memory consumption when loading shaders.
    
*   Shaders: Removed the fixed shader keyword limits. The number of Global keywords is now limited to UInt32, the number of local shader keywords is now limited to UInt16.
    
*   Terrain: Improved the worst-case performance while painting on high-resolution (2k x 2k or higher) Terrain heightmaps. (1283138)
    
*   Terrain: Terrain brushes that sample empty regions at the edge of a terrain now sample the nearest terrain's edge. This corrects brush preview off the edge of a terrain, and corrects the bug of melting terrain edges for the following brushes: Smooth Height, Contrast, Sharpen Peaks, Slope Flatten, Hydrolic, Thermal, Wind, Pinch, Smudge and Twist.
    
*   Tests: Improved the logging in iOS automation so that existing log messages are clarified, and added new ones.
    
*   UI: Added a visualization for the raycast padding around a Graphic object.
    
*   UI: Improved tooltips so that when a tooltip is displayed, hovering another UI control that can display a tooltip makes the new tooltip appear immediately.
    
*   UI: Reused PropertyFields backing fields when possible.
    
*   UI: Updated the icons for Terrain's tool selection.
    
*   UI Toolkit: Added a new RuntimeDefault theme with less overhead for runtime usage.
    
*   UI Toolkit: Improved UI Toolkit event debugger. Improvements include optimizations, adjustable UI, settings, event and callback filtering, and event replay.
    
*   UI Toolkit: Improved USS validation to support more complex properties.
    
*   UI Toolkit: Made performance improvements to reduce the number of managed heap allocations while rendering sprites in the UI Toolkit.
    
*   UI Toolkit: Modified buttons to be focusable.
    
*   UI Toolkit: Modified TransitionEvents to be collapsed when relevant.
    
*   UI Toolkit: Set UIDocument's execution order to -100 to ensure root visual element is created when user's OnEnable runs.
    
*   UI Toolkit: Usage hints can now be changed on a `VisualElement` without having to remove it from the hierarchy to help preserve styling and layout.
    
*   Undo System: Added the Undo history UI.
    
*   Version Control: Added Checkin and Update confirmation notification.
    
*   Version Control: Improved load time performance.
    
*   Version Control: Made stability and performance improvements to the Version Control package (com.unity.collab-proxy).
    
*   Video: Improved the automatic selection of target material texture properties in VideoPlayer. It detects \[MainTexture\] attributes, then detects them by the \_MainTex naming convention.
    
*   Virtual Texturing: Updated tile requests to be returned via `PopRequests` more frequently.
    
*   Virtual Texturing: Updated `InvalidateRegion` calls to generate new tile requests in their "importance" order. The importance is defined as a combination of the tile's screen space size and the the number of frames since the tile has been requested. This makes completing tile requests contribute more to the rendering result when `InvalidateRegion` is called continuously.
    
*   Web: Updated UnityWebRequest's libCurl backend (used on most platforms).
    
*   WebGL: Added support for Screen Orientation Locking and Auto-Rotating for mobile browsers which supports the Screen Orientation API.
    
*   WebGL: Refactored `unityInstance.Quit()` in UnityLoader.js and `call QuitCleanup` from both `unityInstance.Quit()` and `Application.Quit()`.
    
*   WebGL: Updated WebGL compiler to Emscripten 2.0.19 and removed support for the obsolete asm.js linker target.
    
*   Windows: Changed Alt + Enter to default to native resolution which makes the image more crisp and reduces the chance of letterboxing.
    
*   XR: Added support for adding new reference objects at runtime. Added support for ARCore session recording and playback.
    
*   XR: Removed "Preview" text from UI display element.
    

### API Changes

*   2D: Added: Added a Vector3Int constructor accepting two integers for x and y, with z set to 0.
    
*   2D: Added: Added GetAnimationFrameCount, GetAnimationFrame, GetAnimationTime, SetAnimationFrame and SetAnimationTime to get and change the animation timings for Tiles on the Tilemap.
    
*   2D: Added: Added GetTilesRangeCount and GetTilesRangeNonAlloc to get the positions and Tiles between a given start and end positions in a Tilemap.
    
*   2D: Added: Added SetTile/s API using a TileChangeData struct to allow users to set a Tile at a position with color and transform at once instead of invoking 3 calls to do so.
    
*   2D: Added: Allow user to register for notification when the SpriteRenderer's Sprite property has changed.
    
*   2D: Added: New API to query SpriteAtlas information IsIncludedInBuild and GetMasterAtlas.
    
*   2D: Added: Support for default sprite mask material in URP and public api method to retrieve the default 2d mask material.
    
*   Android: Added: Added AndroidJavaObject.CloneReference to enable having multiple references to the same Java object. ([1277152](https://issuetracker.unity3d.com/issues/there-is-no-way-to-have-2-instances-of-androidjavaobject-with-different-references))
    
*   Android: Added: New APIs to manage fast-follow and on-demand delivered asset packs. The APIs wrap Google's PlayCore functionality.
    
*   Android: Added: TargetDevices player setting, so users can select if they want their Android application to run on all devices, just Android phones, tablets, and TV devices, or just Chrome OS devices.
    
*   Animation: Changed: Marked obsolete AnimationMixablePlayable.Create(PlayableGraph graph, int inputCount, bool normalizeWeights) due to unused parameter normalizeWeights. Added new method AnimationMixablePlayable.Create(PlayableGraph graph, int inputCount). (1332215)
    
*   Asset Bundles: Added: Added public API to specify the amount of memory reserved for the shared AssetBundle loading cache.
    
*   Asset Bundles: Added: New API DownloadHandlerAssetBundle.autoLoadAssetBundle for loading AssetBundles asynchronously from DownloadHandlerAssetBundle.
    
*   Asset Import: Added: Added removeConstantScaleCurves in Model Importer. ([1252606](https://issuetracker.unity3d.com/issues/animations-without-scale-curves-get-given-scale-curves-on-import))
    
*   Asset Import: Added: AssetPostprocessor.OnPreprocessCameraDescription and AssetPostprocessor.OnPreprocessLightDescription.
    
*   Asset Import: Added: New public methods MonoImporter.SetIcon/GetIcon and PluginImporter.SetIcon/GetIcon.
    
*   Asset Pipeline: Added: Added a method to the TextureImporter to get the source texture width and height.
    
*   Asset Pipeline: Added: AssetDatabase.SaveAssetIfDirty() to save a specific asset, rather than making a call to AssetDatabase.SaveAssets().
    
*   Build Pipeline: Added: Added the BuildOptions.CleanBuildCache flag to force the incremental player build pipeline to do a clean rebuild of everything.
    
*   Build Pipeline: Added: Callback function BuildPlayerProcessor.PrepareForBuild. This callback can be implemented by users who wish to produce artifacts before the build starts, or to add StreamingAssets to a build without first putting them in the project assets folder.
    
*   Build Pipeline: Deprecated: PackedAsset.file has been deprecated. Instead, to find the matching report file for a particular asset the recommended way is to do a filename lookup in the report.
    
*   Burst: Added: Intrinsics: Neon - Added support for basic vld1 APIs.
    
*   Editor: Added: API on the QueryEngine to better control filtering.
    
*   Editor: Added: Callback to run validation step on materials using a ShaderGUI: \`ValidateMaterial(Material).
    
*   Editor: Added: Introduced Control modifier key to ShortcutManager.
    
*   Editor: Added: Make DraganDrop API to allow user to cusmize drop in legacy window (ProjectBrowser, hierarchy, sceneview).
    
*   Editor: Added: Making hyperLinkClicked public. It is now possible to subscribe to the event EditorGUI.hyperLinkClicked to handle click on a TextField with <;a>;<;/a>; tag.
    
*   Editor: Changed: AndroidArchitecture.x86 and AndroidArchitecture.x86\_64 have been renamed with capital X's. They are now AndroidArchitecture.X86 and AndroidArchitecture.X86\_64.
    
*   Editor: Changed: Decorated EditorGUIUtility.GetIconForObject/SetIconForObject obj parameter with \[NotNull\].
    
*   Editor: Changed: PlayerSettings BuildTargetGroup dependent properties now receive NamedBuildTarget in the API.
    
*   Editor: Changed: Visibility of EditorGUIUtility.GetIconForObject/SetIconForObject from internal to public.
    
*   Editor: Obsoleted: Obsoleted internal method MonoImporter.CopyMonoScriptIconToImporters with \[Obsolete\] and a WarningMessage when called.
    
*   GI: Added: Added two new callbacks. Unity calls `LightProbes.needsRetetrahedralization` whenever the current registered probes and tetrahedralization are out of sync. Unity calls `LightProbes.tetrahedralizationCompleted` after (re-)tetrahedralization is done.
    
*   GI: Added: Added `LightingSettings.lightmapCompression`, which makes it possible for users to select a quality level for lightmap compression.
    
*   GI: Added: Made it possible to opt out of generating a scene's automatic ambient probe and default reflection probe.
    
*   GI: Deprecated: Deprecated `LightmapSettings.textureCompression` and replaced it with `LightingSettings.lightmapCompression`.
    
*   Graphics: Added: "Expand/Collapse All" buttons to Rendering Debugger window menu.
    
*   Graphics: Added: A new API for compiling shaders from editor code and obtaining reflection info was added to ShaderData.Pass.
    
*   Graphics: Added: A new player setting "Upload Cleared Texture Data" was added to revert to the old default behavior of uploading initialised data to video memory when creating a texture from script.
    
*   Graphics: Added: Added a blitter utility class. Moved from HDRP to RP core.
    
*   Graphics: Added: Added a class for drawing shadow cascades: `UnityEditor.Rendering.ShadowCascadeGUI.DrawShadowCascades`.
    
*   Graphics: Added: Added a realtime 2D texture atlas utility classes. Moved from HDRP to RP core.
    
*   Graphics: Added: Added an option to change the visibilty of the Volumes Gizmos (Solid, Wireframe, Everything), available at Preferences >; Core Render Pipeline.
    
*   Graphics: Added: Added class for drawing shadow cascades `UnityEditor.Rendering.ShadowCascadeGUI.DrawShadowCascades`.
    
*   Graphics: Added: Added CommandBuffer.SetGlobalInteger().
    
*   Graphics: Added: Added common include file for meta pass functionality. ([1211436](https://issuetracker.unity3d.com/issues/hdrp-terrain-is-not-visible-in-baked-lightmap-scene-debug-view))
    
*   Graphics: Added: Added Editor window that allow showing an icon to browse the documentation.
    
*   Graphics: Added: Added Fallback Material to DrawSettings.
    
*   Graphics: Added: Added helper for Volumes (Enable All Overrides, Disable All Overrides, Remove All Overrides).
    
*   Graphics: Added: Added IndentLevelScope (for VolumeComponentEditor child class only) to handle indentation of the field and the checkbox.
    
*   Graphics: Added: Added new API function inside DynamicResolutionHandler and new settings in GlobalDynamicResolutionSettings to control low res transparency thresholds. This should help visuals when the screen percentage is too low.
    
*   Graphics: Added: Added new API functions with no side effects to \[DynamicResolutionHandler\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@7.1/api/UnityEngine.Rendering.DynamicResolutionHandler.html) to retrieve resolved dynamic resolution scale (DRS) and to apply DRS on a size.
    
*   Graphics: Added: Added new API to customize the rtHandleProperties of a particular RTHandle. This is a temporary work around to assist with viewport setup of Custom post process when dealing with DLSS or TAAU.
    
*   Graphics: Added: Added new API to replace the use cases of the ShadowAuto, DepthAuto and VideoAuto GraphicsFormat enum members (which will be deprecated in the future).
    
*   Graphics: Added: Added new utils functions to access and set data on `SphericalHarmonicsL2`.
    
*   Graphics: Added: Added OverridablePropertyScope (for VolumeComponentEditor child class only) to handle the Additional Property, the override checkbox and disable display and decorator attributes in one scope.
    
*   Graphics: Added: Added project-wide settings for RenderPipeline with RenderPipelineGlobalSettings.
    
*   Graphics: Added: Added some getters for the Streaming Virtual Texturing settings.
    
*   Graphics: Added: Added the method `DrawHeaders`to the \[VolumeComponentsEditors\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@8.0/api/UnityEditor.Rendering.VolumeComponentEditor.html).
    
*   Graphics: Added: Added UNITY\_PREV\_MATRIX\_M and UNITY\_PREV\_MATRIX\_I\_M shader macros to support instanced motion vector rendering.
    
*   Graphics: Added: Added VolumeComponentMenuForRenderPipelineAttribute to specify a volume component only for certain RenderPipelines.
    
*   Graphics: Added: Added `IAdditionalData` interface to identify the additional datas on the core package.
    
*   Graphics: Added: Allowing Rendering Layer Names to not collide in UI. Includes a new API RenderPipelineAsset.prefixedRenderingLayerMaskNames to fetch a unique list of rendering layer mask names for UI needs.
    
*   Graphics: Added: AssetPostprocessor.OnPostprocessTexture3D ( Texture3D )  
    AssetPostprocessor.OnPostprocessTexture2DArray ( Texture2DArray ).
    
*   Graphics: Added: Automatic spaces to enum display names used in Rendering Debugger and add support for InspectorNameAttribute.
    
*   Graphics: Added: Calculating correct rtHandleScale by considering the possible pixel rounding when DRS is on.
    
*   Graphics: Added: DebugUI.Flags.IsHidden to allow conditional display of widgets in Rendering Debugger.
    
*   Graphics: Added: DebugUI.Foldout.isHeader property to allow creating full-width header foldouts in Rendering Debugger.
    
*   Graphics: Added: DefaultFormat is extended with the new DepthStencil and Shadow values. You can use SystemInfo.GetGraphicsFormat with these new values to get the default GraphicsFormat for a DepthStencil or Shadow RenderTexture on a platform.
    
*   Graphics: Added: Documentation links to Light Sections.
    
*   Graphics: Added: Introduce the RendererList API.
    
*   Graphics: Added: Made GetQualitySettings() method public. This method is used by internal code to implement undo functionality in the Unity Editor.
    
*   Graphics: Added: Method to generate a Texture2D of 1x1 with a plain color.
    
*   Graphics: Added: Mouse & touch input support for Rendering Debugger runtime UI, and fix problems when InputSystem package is used.
    
*   Graphics: Added: New API functions inside DynamicResolutionHandler to get mip bias. This allows dynamic resolution scaling applying a bias on the frame to improve on texture sampling detail.
    
*   Graphics: Added: New API in DynamicResolutionHandler to handle multicamera rendering for hardware mode. Changing cameras and resetting scaling per camera should be safe.
    
*   Graphics: Added: New API to detect when Unity renders with a different type of Render Pipeline : RenderPipelineManager.activeRenderPipelineTypeChanged.
    
*   Graphics: Added: New Depth/Stencil formats to GraphicsFormat: D16\_UNorm, D24\_UNorm, D24\_UNorm\_S8\_UInt, D32\_SFloat, D32\_SFloat\_S8\_UInt.
    
*   Graphics: Added: New draw API as a set of Graphics.RenderX() functions. All the old draw API Graphics.DrawX() functions work as before but many of them can be easily converted to the new API to gain from the added functionality. Some added functionality of the new API:  
    
    *   Support custom per-instance data for RenderMeshInstanced(), per-instance motion vector and rendering layer mask definitions, and easy light probe setup  
        
    *   Support for multi-command indirect draws & future proofing for hardware implementation on supported platforms  
        
    *   Custom world bounds for all mesh rendering (e.g. to support mesh deformation in vertex shaders).
*   Graphics: Added: New methods on CoreEditorDrawers, to allow adding a label on a group before rendering the internal drawers.
    
*   Graphics: Added: New SRPLensFlareData Asset.
    
*   Graphics: Added: New utility function GraphicsFormatUtility.GetDepthStencilFormat. This function lets you easily select the right format on each platform for a certain amount of depth and/or stencil bits.
    
*   Graphics: Added: Red, Green, Blue Texture2D on CoreEditorStyles.
    
*   Graphics: Added: Reminder if the data of probe volume might be obsolete.
    
*   Graphics: Added: Rendering.SupportedRenderingFeatures.reflectionProbesBlendDistance to provide SRPs with the ability to enable the blend distance fields in the ReflectionProbe inspector.
    
*   Graphics: Added: RenderTexture.depthStencilFormat and RenderTextureDescriptor.depthStencilFormat properties. You can now set the exact Depth/Stencil buffer format on a RenderTexture using the depthStencilFormat property. Before, each platform backend would decide what format is used without any control or visibility. The existing APIs that take a number of depth bits will still select the same format as before on each backend. When upgrading RenderTexture assets from an older project, all Depth/Stencil buffers that had more than 16bits will be converted to D24\_UNorm\_S8\_UInt. On high end platforms, this could result in 24bits for depth instead of 32bits resulting in visual artifacts. You need to change the Depth/Stencil format on the RenderTexture asset if that is the case.
    
*   Graphics: Added: Sampling noise to probe volume sampling position to hide seams between subdivision levels.
    
*   Graphics: Added: ScriptableRenderContext.SubmitForRenderPassValidation added to validate whether RenderPass API calls inside the context are eligible for execution.
    
*   Graphics: Added: SpeedTree8MaterialUpgrader, which provides utilities for upgrading and importing SpeedTree 8 assets to scriptable render pipelines.
    
*   Graphics: Added: Support for additional properties for Volume Components without custom editor.
    
*   Graphics: Added: Support for Lens Flare Data Driven (from images and Procedural shapes), on HDRP.
    
*   Graphics: Added: SystemInfo. supportsMultisampleResolveDepth to query platforms Multisample resolve of depth attachments support.
    
*   Graphics: Added: This PR adds a API function checking is all the systems of an Visual Effect are sleeping.
    
*   Graphics: Added: Unified the scope of the \[Material Editor\](https://docs.unity3d.com/2021.2/Documentation/ScriptReference/MaterialEditor.html) headers.
    
*   Graphics: Added: Unity.External.NVIDIA APIs to expose NVIDIA-specific plugin functionality (for controlling DLSS and other features). These APIs are available by enabling the NVIDIA native package on the package manager.
    
*   Graphics: Added: `ReflectionProbe.UpdateCachedState()` to update the internal data related to reflection probe used by the culling system.
    
*   Graphics: Changed: Exposed UseSceneFiltering API as public.
    
*   Graphics: Changed: Renamed Texture2D.Resize to Reinitialize. ([1312670](https://issuetracker.unity3d.com/issues/texture2d-dot-resize-toggles-graphicsformat-each-time-its-called-between-linear-and-srgb))
    
*   Graphics: Changed: RenderBufferStoreActions.Resolve and RenderBufferStoreActions.StoreAndResolve can now be set using the RenderTarget API.
    
*   Graphics: Changed: VFX.VFXManager.PrepareCamera and VFX.VFXManager.ProcessCameraCommand now can take an optional parameter for camera XR settings.
    
*   Graphics: Deprecated: Deprecated ShadowAuto, DepthAuto and VideoAuto graphics formats and introduce a new alternative api. (See the Upgrade Guide for details.).
    
*   Graphics: Deprecated: Most of BatchRenderGroup API will be fully deprecated in 2022.2 (and replaced by a new API).
    
*   Graphics: Obsoleted: ReflectionProbe.defaultReflectionSet has been deprecated in favor of ReflectionProbe.defaultReflectionTexture.
    
*   Graphics: Removed: Removed GraphicsFormatUtility.GetDepthStencilFormat(int) after being public for two alpha releases.
    
*   HDRP: Added: "Conservative" mode for shader graph depth offset.
    
*   HDRP: Added: Ability to animate many physical camera properties with Timeline.
    
*   HDRP: Added: Ability to control focus distance either from the physical camera properties or the volume.
    
*   HDRP: Added: Added a better support for LODs in the ray tracing acceleration structure.
    
*   HDRP: Added: Added a built-in custom pass to draw object IDs.
    
*   HDRP: Added: Added a complete solution for volumetric clouds for HDRP including a cloud map generation tool.
    
*   HDRP: Added: Added a custom post process injection point AfterPostProcessBlurs executing after depth of field and motion blur.
    
*   HDRP: Added: Added a dialog box when you import a Material that has a diffusion profile to add the diffusion profile to global settings.
    
*   HDRP: Added: Added a Falloff Mode (Linear or Exponential) in the Density Volume for volume blending with Blend Distance.
    
*   HDRP: Added: Added a Force Forward Emissive option for Lit Material that forces the Emissive contribution to render in a separate forward pass when the Lit Material is in Deferred Lit shader Mode.
    
*   HDRP: Added: Added a minimum motion vector length to the motion vector debug view.
    
*   HDRP: Added: Added a parameter to control the vertical shape offset of the volumetric clouds. (1358528)
    
*   HDRP: Added: Added a property on the HDRP asset to allow users to avoid ray tracing effects running at too low percentages. ([1342588](https://issuetracker.unity3d.com/issues/dlss-dxr-ray-tracing-effects-do-not-scale-well-with-dlss-and-produce-jagged-slash-pixelated-results))
    
*   HDRP: Added: Added a property to control the fallback of the last bounce of a RTGI, RTR, RR ray to keep a previously existing side effect on user demand.
    
*   HDRP: Added: Added a setting in the HDRP asset to change the Density Volume mask resolution of being locked at 32x32x32 (HDRP Asset >; Lighting >; Volumetrics >; Max Density Volume Size).
    
*   HDRP: Added: Added a shortcut to HDRP Wizard documentation.
    
*   HDRP: Added: Added a slider that controls how much the volumetric clouds erosion value affects the ambient occlusion term.
    
*   HDRP: Added: Added a slider to control the fallback value of the directional shadow when the cascade have no coverage.
    
*   HDRP: Added: Added an example in the documentation that shows how to use the accumulation API for high quality antialiasing (supersampling).
    
*   HDRP: Added: Added an option to have double sided GI be controlled separately from material double-sided option.
    
*   HDRP: Added: Added an option to render screen space global illumination in half resolution to achieve real-time compatible performance in high resolutions. ([1353727](https://issuetracker.unity3d.com/issues/ssgi-denoise-and-ssgitrace-has-poor-performance))
    
*   HDRP: Added: Added browsing of the documentation of Compositor Window.
    
*   HDRP: Added: Added color and intensity customization for Decals.
    
*   HDRP: Added: Added dependency to mathematics and burst, HDRP now will utilize this to improve on CPU cost. First implementation of burstified decal projector is here.
    
*   HDRP: Added: Added info box when low resolution transparency is selected, but its not enabled in the HDRP settings. This will help new users find the correct knob in the HDRP Asset.
    
*   HDRP: Added: Added light unit slider for automatic and automatic histrogram exposure limits.
    
*   HDRP: Added: Added new AOV APIs for overriding the internal rendering format, and for outputing the world space position.
    
*   HDRP: Added: Added new API in CachedShadowManager.
    
*   HDRP: Added: Added pivot point manipulation for Decals (inspector and edit mode).
    
*   HDRP: Added: Added shader graph unit test for IsFrontFace node.
    
*   HDRP: Added: Added slides to control the shape noise offset.
    
*   HDRP: Added: Added support for internal plugin materials and HDSubTarget with their versioning system.
    
*   HDRP: Added: Added support for reflection probes as a fallback for ray traced reflections. (1338644)
    
*   HDRP: Added: Added support for the camera bridge in the graphics compositor
    
*   HDRP: Added: Added support for Unlit shadow mattes in Path Tracing. ([1335487](https://issuetracker.unity3d.com/issues/unlit-shader-graph-with-shadow-matte-option-enabled-does-not-receive-shadows-when-path-tracing-is-enabled))
    
*   HDRP: Added: Added support of motion vector buffer in custom postprocess.
    
*   HDRP: Added: Added TargetMidGrayParameterDrawer.
    
*   HDRP: Added: Added the receiver motion rejection toggle to RTGI (1330168)
    
*   HDRP: Added: Added the support of volumetric clouds for baked and realtime reflection probes.
    
*   HDRP: Added: Added three animation curves to control the density, erosion, and ambient occlusion in the custom submode of the simple controls.
    
*   HDRP: Added: Added tooltips for content inside the Rendering Debugger window.
    
*   HDRP: Added: Added two toggles to control occluder rejection and receiver rejection for the ray traced ambient occlusion (1330168)
    
*   HDRP: Added: Added UV manipulation for Decals (edit mode).
    
*   HDRP: Added: Added ValidateMaterial callbacks to ShaderGUI.
    
*   HDRP: Added: Added View Bias for mesh decals.
    
*   HDRP: Added: Added warning for when a light is not fitting in the cached shadow atlas and added option to set maximum resolution that would fit.
    
*   HDRP: Added: API to allow OnDemand shadows to not render upon placement in the Cached Shadow Atlas.
    
*   HDRP: Added: Area Light support for Hair and Fabric master nodes.
    
*   HDRP: Added: Deferred shading debug visualization.
    
*   HDRP: Added: Documentation for volumetric clouds.
    
*   HDRP: Added: Exposed update upon light movement for directional light shadows in UI.
    
*   HDRP: Added: Global settings check in Wizard.
    
*   HDRP: Added: Help URL for volumetric clouds override.
    
*   HDRP: Added: Lens Flare Samples.
    
*   HDRP: Added: Localization on Wizard window.
    
*   HDRP: Added: LTC Fitting tools for all BRDFs that HDRP supports.
    
*   HDRP: Added: Mixed RayMarching/RayTracing mode for RTReflections and RTGI.
    
*   HDRP: Added: New checkbox to enable mip bias in the Dynamic Resolution HDRP quality settings. This allows dynamic resolution scaling applying a bias on the frame to improve on texture sampling detail.
    
*   HDRP: Added: New control slider on RTR and RTGI to force the LOD Bias on both effects.
    
*   HDRP: Added: Path tracing support for AxF material.
    
*   HDRP: Added: Path tracing support for stacklit material.
    
*   HDRP: Added: Scale Mode setting for Decals.
    
*   HDRP: Added: Speed Tree 8 shader graph as default Speed Tree 8 shader for HDRP.
    
*   HDRP: Added: Support for Fabric material in Path Tracing.
    
*   HDRP: Added: Support for lighting full screen debug mode in automated tests.
    
*   HDRP: Added: Support for mip bias override on texture samplers through the HDAdditionalCameraData component.
    
*   HDRP: Added: Support for multi volumetric cloud shadows.
    
*   HDRP: Added: Support for screen space shadows (directional and point, no area) for shadow matte unlit shader graph.
    
*   HDRP: Added: Support for surface gradient based normal blending for decals.
    
*   HDRP: Added: Support for tessellation for all master node in shader graph.
    
*   HDRP: Added: Support for volumetric clouds in planar reflections.
    
*   HDRP: Added: Support of interpolators for SV\_POSITION in shader graph.
    
*   HDRP: Added: Toggle to render the volumetric clouds locally or in the skybox.
    
*   HDRP: Added: Way for fitting a probe volume around either the scene contents or a selection.
    
*   IL2CPP: Removed: Removed IIl2CppProcessor interface.
    
*   IL2CPP: Removed: Removed IUnityLinkerProcessor.OnBeforeRun and IUnityLinkerProcessor.OnAfterRun interface methods.
    
*   iOS: Added: Added `iOS.Device.iosAppOnMac` flag to check if app built for iOS is running on Mac equipped with Apple Silicon chip.
    
*   iOS: Changed: EditorUserBuildSettings.symlinkLibraries renamed to EditorUserBuildSettings.symlinkSources, both Android and iOS will use this property.
    
*   iOS: Deprecated: ScreenOrientation.Landscape as it was a synonym for ScreenOrientation.LandscapeLeft, and not "some Landscape orientation", which is confusing. (1320447)
    
*   Linux: Added: LinuxServer value added to RuntimePlatform enum.
    
*   macOS: Added: OSXServer value added to RuntimePlatform enum.
    
*   Package: Added: (Recorder) Added public API for AOVRecorderSettings.
    
*   Package Manager: Added: Added a new `AddAndRemove` method to the `UnityEditor.PackageManager.Client` API which can be used to add and/or remove multiple packages to/from the project in a single operation.
    
*   Physics: Added: Expose ArticulationBody.collisionDetectionMode property to set various collision detection modes, like Discrete, Continuous and etc.
    
*   Physics: Added: Expose the improved patch friction mode that will distribute the normal force over the friction anchors and thus match analytical results closer.
    
*   Physics: Added: Exposed a new property in RaycastHit called colliderInstanceID, which returns the instance ID of the collider the ray collided with.
    
*   Physics: Added: ForceMode argument to ArticulationBody.Add force and related functions.
    
*   Physics: Added: Property for retrieving ArticulationBody components during a collision event. Articulation bodies can be retrieved by Collision.articulationBody.
    
*   Physics: Added: Property for retrieving either ArticulationBody or Rigidbody components to collision events under Collision.body.
    
*   Plugins: Added: New IUnityLog interface for message logging to Unity console and log in native plugins.
    
*   Plugins: Added: New IUnityProfilerV2 interface with Profiler Counters API in native plugins.
    
*   Prefabs: Added: Exposed FindAllInstancesOfPrefab to scripting.
    
*   Prefabs: Added: New API for source prefab apply/revert context menu hook on a property field.
    
*   Prefabs: Added: New API to define a C# scoped region in which prior to every inspector/editor imgui property being drawn a callback can be called with the associated Rect and SerializedProperty.
    
*   Prefabs: Changed: The classes PrefabStage and PrefabStageUtility have been moved out of the experimental namespace UnityEditor.Experimental.SceneManagement to the namespace UnityEditor.SceneManagement, leaving nothing left in UnityEditor.Experimental.SceneManagement. The move is supported by the API updater. Note that the Timeline package needs to be at least version 1.3.0 to compile with this change all later versions can be fixed by the API Updater.
    
*   Profiler: Added: Added Profiler.EmitSessionMetaData api to pass generic metadata to the Profiler associated with profiling session.
    
*   Profiler: Added: API to create GPU sampling ProfilerMarker.
    
*   Profiler: Added: New C# custom Categories API.
    
*   Profiler: Changed: Added GPU profiling capabilities to ProfilerRecorder API.
    
*   Scripting: Added: Added FileUtil.GetPhysicalPath and FileUtil.GetLogicalPath methods to convert logical paths to physical and vice versa.
    
*   Scripting: Added: APIs for the AsyncReadManager, to enable chaining and canceling of reads.
    
*   Scripting: Added: Component.GetComponentInParent(Type t, bool includeInactive) method to match GameObject. ([1331778](https://issuetracker.unity3d.com/issues/component-dot-getcomponentinparent-doesnt-have-an-overload-for-getting-components-of-inactive-objects))
    
*   Search: Added: Added SearchService.ShowPicker API to pick any search item result.
    
*   Serialization: Added: Expand SerializationUtility class to allow checking for missing type instances and removing them from a SerializeReference Host.
    
*   Serialization: Added: New SerializationUtility class for access to Managed Reference Ids.
    
*   Serialization: Added: Support "get" on SerializedProperty.managedReferenceValue.
    
*   Services: Added: Added new com.unity.services.core package that is used for common behaviour of Game Service packages
    
*   Services: Changed: Updating analytics dashboard to point to new location.
    
*   Shadergraph: Added: Added **LinearGrey** and **Red** as default texture mode options for \[Texture2D properties\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/api/UnityEditor.ShaderGraph.Internal.Texture2DShaderProperty.DefaultType.html?q=%20linearGrey).
    
*   Shadergraph: Added: Added a checkbox to toggle the**Disable Global Mip Bias** setting for \[Sample Texture 2D\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Sample-Virtual-Texture-Node.html) and Sample Texture 2D array nodes.
    
*   Shadergraph: Added: Added a new \[Dropdown Node\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Sub-Graph-Dropdown-Node.html) that makes it possible to control compile time branching in Sub Graphs from their parent graph.
    
*   Shadergraph: Added: Added a new \[target\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Graph-Target.html) for the Built-In Render Pipeline which includes Lit and Unlit sub-targets.
    
*   Shadergraph: Added: Added a ShaderGraph animated preview framerate throttle.
    
*   Shadergraph: Added: Added a \[Split Texture Transform Node\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Split-Texture-Transform-Node.html) which makes it possible to use or override a texture's tiling and offset values.
    
*   Shadergraph: Added: Added a \[Tiling and Offset Node\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Tiling-And-Offset-Node.html) for modifying Texture2D input.
    
*   Shadergraph: Added: Added a \[`Calculate Level Of Detail Texture 2D`\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Calculate-Level-Of-Detail-Texture-2D-Node.html) node, which maps to the HLSL intrinsic functions `CalculateLevelOfDetail` and `CalculateLevelOfDetailUnclamped`.
    
*   Shadergraph: Added: Added a \[`Gather Texture 2D`Node \](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Gather-Texture-2D-Node.html) for retrieving four samples (red component only) for the bilinear interpolation of Texture2D samples.
    
*   Shadergraph: Added: Added ability to define custom vertex-to-fragment interpolators.
    
*   Shadergraph: Added: Added an HLSL file that implements a version of the Unity core LODDitheringTransition function for crossfading between levels of detail.
    
*   Shadergraph: Added: Added Categories to the \[Blackboard\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Blackboard.html), which makes it easier to organize shader \[properties\](https://docs.unity3d.com/Manual/SL-Properties.html) and \[Keywords\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Keywords.html) in the Shader Graph tool. The Material Inspector for URP and HDRP also includes these categories for materials created with Shader Graphs.
    
*   Shadergraph: Added: Added custom interpolator documentation
    
*   Shadergraph: Added: Added custom interpolator thresholds on Shader Graph project settings page.
    
*   Shadergraph: Added: Added information about selecting and unselecting items to the Blackboard article.
    
*   Shadergraph: Added: Added many node synonyms for the Create Node search so that it's easier to find nodes.
    
*   Shadergraph: Added: Added selection highlight and picking shader passes for URP target.
    
*   Shadergraph: Added: Added stage control functionality for ShaderGraph \[Keywords\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Keywords.html) to make it possible to have fragment-only or vertex-only keywords.
    
*   Shadergraph: Added: Added Tessellation Option to PositionNode settings, to provide access to the pre-displaced tessellated position.
    
*   Shadergraph: Added: Added the \[Eye Index\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Eye-Index-Node.htm), \[Instance ID\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Instance-ID-Node.html), and \[Vertex ID\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Vertex-ID-Node.html) nodes to Shader Graph.
    
*   Shadergraph: Added: Added visible errors for invalid stage capability connections to shader graph.
    
*   Shadergraph: Added: Added \[SpeedTree Sub Graph Assets\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/SpeedTree8-SubGraphAssets.html) to support SpeedTree 8: SpeedTree8Wind, SpeedTree8ColorAlpha, and SpeedTree8Billboard.
    
*   Shadergraph: Added: Added \[`Branch On Input Connection`\](https://docs.unity.cn/Packages/com.unity.shadergraph@12.0/manual/Branch-On-Input-Connection-Node.html node. This node supports conditional branching in Sub Graphs.
    
*   Shadergraph: Added: Added `Dropdown` node to each dropdown property for configuring branch control.
    
*   Shadergraph: Added: Added `Sprite` option to Main Preview, which is similar to `Quad` but does not allow rotation. `Sprite` is used as the default preview for URP Sprite shaders.
    
*   Shadergraph: Added: Added `Use Custom Binding` option to properties. When this option is enabled, you can connect a property to a \[`Branch On Input Connection`\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/manual/Branch-On-Input-Connection-Node.html) node.
    
*   Shadergraph: Added: Adding control of anisotropic settings on inline Sampler state nodes in ShaderGraph.
    
*   Shadergraph: Added: It is now possible to mark textures as \\\[MainTexture\\\] and colors as \\\[MainColor\\\].
    
*   Shadergraph: Added: The \[Texture2D\](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.0/api/UnityEditor.ShaderGraph.Internal.Texture2DShaderProperty.DefaultType.html) **Bump** option is now called **Normal Map**, and properties with this option enabled take the `[NormalMap]` tag.
    
*   Shaders: Added: Added a missing API to check shader compilation warnings.  
    Added a missing API to get information about individual shaders. ([1340374](https://issuetracker.unity3d.com/issues/no-api-to-determine-if-a-shader-has-warnings))
    
*   Shaders: Added: Added UnityEngine.Rendering.GlobalKeyword struct to represent keywords in the global keyword space.  
    Added UnityEngine.Rendering.LocalKeyword struct to represent keywords in the local keyword space.  
    Added UnityEngine.Rendering.LocalKeyword struct to represent the keyword space of a particular shader or compute shader.  
    Added ComputeShader.enabledKeywords and Material.enabledKeywords to query or set all enabled keywords simultaneously.  
    Added ComputeShader.keywordSpace and Shader.keywordSpace to query the local keyword space of the corresponding shader.  
    Added optimized Material.EnableKeyword, Material.DisableKeyword, Material.IsKeywordEnabled, ComputeShader.EnableKeyword, ComputeShader.DisableKeyword and ComputeShader.IsKeywordEnabled overloads that work with the new LocalKeyword struct.  
    Added optimized CommandBuffer.EnableKeyword, CommandBuffer.DisableKeyword, Shader.EnableKeyword, Shader.DisableKeyword and Shader.IsKeywordEnabled overloads that work with the new GlobalKeyword struct.  
    Added Shader.enabledGlobalKeywords property to query the global keyword state.  
    Added Shader.globalKeywords property to query the existing global keywords.
    
*   Shaders: Added: CommandBuffer.EnableKeyword,CommandBuffer.DisableKeyword can now be used to enable a local shader keyword.
    
*   Shaders: Added: LocalKeyword.isOverridable property to check whether a given local shader keyword can be overridden by global shader keyword state.
    
*   Shaders: Added: LocalKeyword.type can now be used to understand why the local shader keyword was added to the local keyword space of a shader or compute shader.
    
*   Shaders: Added: Material.SetKeyword, ComputeShader.SetKeyword, Shader.SetKeyword and CommandBuffer.SetKeyword can now be used to set the shader keyword state directly.
    
*   Shaders: Added: UnityEngine.Rendering.ShaderKeywordType Plugin is a new type for keywords registered by shader compiler plugins.
    
*   Shaders: Deprecated: ShaderKeyword.GetGlobalKeywordName, ShaderKeyword.GetName and ShaderKeyword.GetKeywordType.
    
*   Terrain: Added: Added DetailPrototype.NoiseSeed and its GUI in terrain Detail wizards, so that the random seed for detail object placement can be specified. (1291809)
    
*   Terrain: Added: Added TerrainData.ComputeDetailInstanceTransforms that returns an array of DetailInstanceTransform structs containing the exact same transforms of details that Unity uses for rendering.
    
*   Terrain: Changed: IOnInspectorGUI ShowBrushGUI overloads removed and replaced with a single ShowBrushGUI call with default parameters.
    
*   Terrain: Changed: TerrainAPI namespace is no longer part of an experimental namespace and has been renamed TerrainTools.
    
*   Terrain: Changed: TerrainPaintTool GetDesc changed to GetDescription.
    
*   Terrain: Changed: TerrainUtility moved to UnityEngine.TerrainUtils namespace.
    
*   Terrain: Changed: TerrainUtility.TerrainMap moved to UnityEditor.TerrainUtils.TerrainMap. TerrainMap.TileCoord moved to UnityEditor.TerrainUtils.TerrainTileCoord.
    
*   Terrain: Changed: UnityEditor.TerrainAPI.TerrainPaintUtilityEditor.BrushPreview changed to UnityEditor.TerrainTools.TerrainBrushPreviewMode.
    
*   UI: Added: GetPersistentListenerState added to UnityEvent.
    
*   UI Toolkit: Added: Added visualTreeAssetSource property to VisualElement to allow identifying the VisualTreeAsset a visual tree was cloned from.
    
*   UI Toolkit: Added: Animated drag and drop support to ListView. Use reorderMode property.
    
*   UI Toolkit: Added: DestroyItem callback to ListView to have a counterpart for makeItem.
    
*   UI Toolkit: Added: Display options to ListView: showAddRemoveFooter, showFoldoutHeader, headerTitle.
    
*   UI Toolkit: Added: Expose ScrollView.mode property.
    
*   UI Toolkit: Added: New public UI Toolkit APIs:  
    
    *   Dropdownfield.choices  
        
    *   BasePopupField.choices  
        
    *   MaskField.choices  
        
    *   MaskField.choicesMasks.
*   UI Toolkit: Added: Tool for converting assets created with the package to use them without the package installation, and to convert them back to package versions.
    
*   UI Toolkit: Added: VirtualizationMethod property to collection views to allow to change between fixed height and dynamic height virtualization.
    
*   UI Toolkit: Changed: ListView's itemHeight is now a float and was renamed to fixedItemHeight to enforce the fact that it is only used with FixedHeight virtualization method.
    
*   UI Toolkit: Changed: ListView's Refresh() was split into RefreshItems() which simply rebinds reused items and Rebuild() which recreates all items from scratch.
    
*   UI Toolkit: Deprecated: CurveField.borderUssClassName and GradientField.borderUssClassName are now deprecated since the related visual element is not required to render a border anymore.
    
*   UI Toolkit: Deprecated: Deprecated OnKeyDown method in ListView. Use the event system instead, see SendEvent.
    
*   UI Toolkit: Obsoleted: ListView's onItemChosen and onSelectionChanged are now obsolete.
    
*   Universal: Added: 2D Light Texture Node. A Shader Graph node that enable sampling of the Light Textures generated by the 2D Renderer in a lit scene.
    
*   Universal: Added: Added View Vector node to mimic old behavior of View Direction node in URP.
    
*   Universal: Added: Depth and DepthNormals passes to particles shaders.
    
*   Universal: Added: Enabled deferred renderer in UI.
    
*   Universal: Added: Fixed an error where multisampled texture being bound to a non-multisampled sampler in XR. ([1297013](https://issuetracker.unity3d.com/issues/android-urp-black-screen-when-building-project-to-an-android-device-with-mock-hmd-enabled-and-multisampled-sampler-errors))
    
*   Universal: Added: SpeedTree 8 Shader Graph but did not set it as the default when importing or upgrading Speed Tree 8 assets. Because URP doesn't yet support per-material culling, this Shader Graph does not yet behave in the same way as the existing handwritten SpeedTree 8 shader for URP.
    
*   Universal: Added: Support for light layers, which uses Rendering Layer Masks to make Lights in your Scene only light up specific Meshes.
    
*   Universal: Added: Support for SSAO in Particle and Unlit shaders.
    
*   Universal: Added: \_SURFACE\_TYPE\_TRANSPARENT keyword to URP shaders.
    
*   URP: Added: "Allow Material Override" option to Lit and Unlit ShaderGraph targets. When checked, allows Material to control the surface options (transparent/opaque, blend mode, etc).
    
*   URP: Added: Added a help button on material editor to show the shader documentation page.
    
*   URP: Added: Added GetUniversalAdditionalLightData, a method that returns the additional data component for a given light or create one if it doesn't exist yet.
    
*   URP: Added: Added Lights 2D to the Light Explorer window.
    
*   URP: Added: Added Motion Vector render pass for URP.
    
*   URP: Added: Added Render Settings Converter to the Render Pipeline Converter, this tool creates and assigns URP Assets based off rendering settings of a Builtin project.
    
*   URP: Added: Added support for default sprite mask shaders for the 2D Renderer in URP.
    
*   URP: Added: Blending and box projection for reflection probes.
    
*   URP: Added: Decal support. This includes new Decal Projector component, Decal renderer feature and Decal shader graph.
    
*   URP: Added: Fixed incorrect shadow fade in deferred rendering mode.
    
*   URP: Added: Light cookies support to directional, point and spot light. Directional light cookie is main light only feature.
    
*   URP: Added: New UI for Render Pipeline Converters. Used now for Built-in to Universal conversion.
    
*   URP: Added: New URP Debug Views under Window/Analysis/Rendering Debugger.
    
*   URP: Added: Optional Depth Priming. Allows the forward opaque pass of the base camera to skip shading certain fragments if they don't contribute to the final opaque output.
    
*   URP: Added: Possibility to rename light layer values.
    
*   URP: Added: Sections on Light Inspector.
    
*   URP: Added: Store Actions' option that enables bandwidth optimizations on mobile GPU architectures.
    
*   URP: Added: Support for controlling Volume Framework Update Frequency in UI on Cameras and URP Asset as well as through scripting.
    
*   URP: Added: Two new URP specific scene templates, Basic which has a camera and directional light, then Standard which has the addition of a global volume with basic post effects setup.
    
*   URP: Added: URP global setting for stripping off shader variants.
    
*   URP: Added: URP global setting for stripping post processing shader variants.
    
*   URP: Added: URP Global Settings Asset to the Graphics Settings - a common place for project-wide URP settings.
    
*   URP: Added: VFX: Basic support of Lit output.
    
*   URP: Added: VFX: Fix light cookies integration.
    
*   URP: Added: XR: Added Late Latching support to reduce VR latency (Quest).
    
*   URP: Changed: Reorder camera inspector to be in the same order as HDRP.
    
*   Version Control: Added: VCS support can now be added to Unity with managed code only as opposed to implementing native plugin. See UnityEditor.VersionControl.VersionControlObject and related classes.
    
*   VFX Graph: Added: Added HDRP Decal output context.
    
*   VFX Graph: Added: Added Is Inside subgraph into VFX Graph additions package.
    
*   VFX Graph: Added: Added new setting in "Preferences ->; Visual Effects" to control the fallback behavior of camera buffers from MainCamera node when the main camera is not rendered.
    
*   VFX Graph: Added: Added support for Texture2D Arrays in Flipbooks.
    
*   VFX Graph: Added: Material Offset setting in inspector of the rendered outputs.
    
*   VFX Graph: Added: Motion vectors enabled for particle strips.
    
*   VFX Graph: Added: New tool : Signed Distance Field baker.
    
*   VFX Graph: Added: New tool to help set VFX Bounds.
    
*   VFX Graph: Added: Placement option (Vertex, Edge, Surface) in Sample Mesh & Skinned Mesh, allows triangle sampling.
    
*   VFX Graph: Added: Provide explicit access to spawnCount in graph
    
*   VFX Graph: Added: Restore "Exact Fixed Time Step" option on VisualEffectAsset.
    
*   VFX Graph: Added: Sample vertices of a transformed skinned mesh with Position (Skinned Mesh) and Sample Skinned Mesh operator.
    
*   VFX Graph: Added: Structured Graphics Buffer support as exposed type
    
*   VFX Graph: Added: Support 2D Renderer in URP for Unlit.
    
*   VFX Graph: Added: Support of direct link event to initialize context (which support several event within the same frame)
    
*   VFX Graph: Added: The VFX editor automatically attach to the current selection if the selected gameobject uses the currently edited VFX asset.
    
*   VFX Graph: Added: Two new buttons are available in the editor's tool bar. One will display a popup panel to handle attachement and one to lock/unlock the current attachement.
    
*   Video: Added: Advanced video encoding controls for H.264 (for Windows only) and VP8.
    
*   Windows: Added: WindowsServer value added to RuntimePlatform enum.
    
*   XR: Added: New API to the XRMeshSubsystem which allows a transform to be associated with each mesh. This provides a potential optimization for plugins that include a transform with each mesh, allowing them to avoid transforming each vertex into session-space.
    
*   XR: Removed: Removed the Windows XR SDK Plug-in from Unity. Microsoft now supports Windows MR devices using OpenXR in Unity 2021, and recommends using Unity's OpenXR plugin.
    

### Changes

*   2D: Allowed non-public fields with the SerializeField attribute as custom fields for RuleTile.
    
*   2D: Changed some PSDImporter settings to use checkboxes instead of drop-down menus.
    
*   2D: Replaced usage of Triangle.Net with in house tessellation solution.
    
*   2D: Updated com.unity.2d.sprite package license
    
*   2D: Updated com.unity.2d.tilemap package license
    
*   2D: Updated the SceneView overlays used by the Tile Palette to use UIToolkit/new Overlays framework instead of IMGUI. (1342226)
    
*   AI: Updated component-based workflow notice in the Navigation window.
    
*   Android: Allowed Android Player to use Vulkan on GPUs that are currently unknown to Unity on Android 11 or newer.
    
*   Android: Changed how Unity checks to see if an obb is compatible with an apk. Both the apk and obb now have unity\_obb\_guid file inside them and if the contents match between them, Unity treats them as being compatible.
    
*   Android: Changed the minimum supported Android version to 5.1 (API 22).
    
*   Android: Removed OpenGL ES 2.0 from Auto Graphics API. The preferred API is now Vulkan.
    
*   Android: Removed support for putting gradle resources in Assets/Plugins/Android/\[res, assets\]. you either need to use Android archive plug-ins, Android Library plug-ins, or move those files to Streaming Assets.
    
*   Android: Removed the overwrite comment in gradle files and manifest files '// GENERATED BY UNITY. REMOVE THIS COMMENT TO PREVENT OVERWRITING WHEN EXPORTING AGAIN'. Use templates if you want your changes to persist.
    
*   Android: When _Auto Graphics API_ is enabled, Require ES3.1, Require ES3.1+AEP, Require ES 3.2 properties in Android Player Settings are now available.
    
*   Android: When you export an Android project, Unity no longer creates a symbols zip package because it was always missing libil2cpp.so symbols. After you build your project manually, zip unityLibrary/symbols package if you want to upload it to Google Play.
    
*   Asset Import: Unity will not attempt to relaunch Maya or 3DsMax after the first timeout. ([1281786](https://issuetracker.unity3d.com/issues/two-attempts-are-made-to-open-maya-and-convert-a-ma-file-to-fbx-when-importing-it))
    
*   Asset Pipeline: Changed AssetPostprocessors calls so that they are ordered by their GetPostprocessOrder and then by their FullName (namespace.classname).
    
*   Build Pipeline: Unity no longer writes unsaved changes from open scenes into player builds. Instead, it asks to save changes to disk.
    
*   Burst: Added full support for Armv8.2 Neon intrinsics.
    
*   Burst: Altered the IL Post Processed 'direct call' Burst function pointers to defer until they are needed to be compiled.
    
*   Burst: Assigned rpmalloc as the native allocator on Windows to speed up concurrently executing LLVM work.
    
*   Burst: Changed how exceptions throw types and how messages are stored in Burst binaries to reduce overall binary size.
    
*   Burst: Changed how exceptions throw types, and how messages are stored in our Burst binaries to reduce binary size.
    
*   Burst: Changed how SLEEF global variables for trigonometric functions are pulled into Burst to reduce duplications.
    
*   Burst: Changed how Unity resolves function references in the compiler to improve resolving an existing function reference by 3x.
    
*   Burst: Changed the Burst minimum Editor version to 2019.4.
    
*   Burst: Changed the link step to not use response files if the command line was small enough, saving the cost of the round-trip to the disk.
    
*   Burst: Changed to inliner heuristics to improve build time and reduce executable size.
    
*   Burst: Disabled threading within the `lld` linker instances used for in-Editor and desktop cross compilation.
    
*   Burst: DOTS Runtime now shares the logging code path with the general case.
    
*   Burst: half <;->; float/double conversions now use native hardware where possible (Arm or AVX2).
    
*   Burst: Improved how Unity handles generic resolution in Cecil to cache the strictly resolved generic types and to save time in the compiler.
    
*   Burst: Improved the compiling process of a method when its assembly's dependencies have changed so that the Burst version of the method is immediately used.
    
*   Burst: Modified the IL Post Processed 'direct call' Burst function pointers so that they are not compiled until they are needed.
    
*   Burst: Named constant array data after the static field it belongs to in assembly.
    
*   Burst: Reduced the time it takes for Burst to check if any Burst-compilable code has changed to improve iteration speed.
    
*   Burst: Removed the ability to experiment with `Unity.Burst.Intrinsics.Common.Pause`.
    
*   Burst: Removed the entry-point name job/function-pointer that caused the throw in exception strings.
    
*   Burst: Removed the entry-point name of the job or function-pointer that caused an exception in exception strings to support the Burst compiler's requirement for deterministic results, which are not compatible with per-entry-point function derivations.
    
*   Burst: Restricted use of Burst in secondary Unity processes. Code normally Burst-compiled now runs under Mono.
    
*   Burst: Shared the logging code path of the general case with DOTS Runtime.
    
*   Burst: Upgraded Burst to use LLVM Version 11.0.1 by default, bringing the latest optimization improvements from the LLVM project.
    
*   Burst: Upgraded Burst to use LLVM Version 11.0.1 by default.
    
*   Editor: Added a new search field to filter dependencies.
    
*   Editor: Changed the behaviour of an Editor Window to ignore minimum and maximum sizes when being docked. Each window defines how it should adapt to the available space. ([1269298](https://issuetracker.unity3d.com/issues/package-manager-window-does-not-expand-when-its-docked-to-a-small-width-size-window))
    
*   Editor: Deleting an object reference array entry in the Inspector now removes that array element. Previously, this was a two-step process.
    
*   Editor: Made changes such that the default parent object is no longer simultaneously displayed for all loaded scenes. Now, when you use Set Default Parent Object, the scene to which the object belongs is set as active.
    
*   Editor: Modified includes and excludes in the Index Manager to keep the last selected file pattern in the enum field when you add another item.
    
*   Editor: Moved asset importing and cache server related preferences to the Asset Pipeline preferences window page.
    
*   Editor: Moved some main toolbar elements to the left align container.
    
*   Editor: Moved the UI widget used for Light Cookies from the standard Property Field to the ObjectField that provides texture preview and asset directory search capabilities, across HDRP and built-in.
    
*   Editor: Removed limitation on TooltipAttribute so you can apply it anywhere. In the Editor, currently only Tooltips on fields are visible.
    
*   Editor: Removed the dependencies help box.
    
*   Editor: Updated the Collaborate package to let users migrate to Plastic SCM.
    
*   GI: Removed Enlighten deprecation notices for Enlighten Realtime Global Illumination. Enlighten Baked Global Illumination is still deprecated.
    
*   Graphics: \*Added the blend distance of the reflection probe to Unity\_SpecCubeN\_BoxMax.w  
    \*Added information about the relative importance between SpecCube 0 and SpecCube1 to unity\_SpecCube1\_BoxMin.w
    
*   Graphics: Added a macro layer for 2D texture sampling macros to Platform ShaderLibrary API headers. This layer starts with a PLATFORM\_SAMPLE2D definition, and lets you inject sampling behavior on a render pipeline level. For example, being able to a global mipmap bias for temporal upscalers.
    
*   Graphics: Added an ArgumentException for Cubemap pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData & SetPixel/SetPixels/SetPixels32/SetPixelData) when encountering an error.
    
*   Graphics: Added an ArgumentException for CubemapArray pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData & SetPixel/SetPixels/SetPixels32/SetPixelData) when encountering an error.
    
*   Graphics: Added an ArgumentException for Texture2DArray pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData & SetPixel/SetPixels/SetPixels32/SetPixelData) when encountering an error.
    
*   Graphics: Added an ArgumentException for Texture3D pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData & SetPixel/SetPixels/SetPixels32/SetPixelData) when encountering an error.
    
*   Graphics: Added an ArgumentException for WebCamTexture pixel access functions (GetPixel/GetPixels/GetPixels32) when encountering an error. Calling these functions before the first frame update throws an exception instead of returning blank data.
    
*   Graphics: Altered LensFlare (SRP) so it can be disabled per element.
    
*   Graphics: Changed the menu path for _Generate Shader Includes_ from _Edit_ >; _Render Pipeline_ >; _Generate Shader Includes_ to _Edit_ >; _Rendering_ >; _Generate Shader Includes_.
    
*   Graphics: Changed the menu path for _LookDev_ from _Assets_ >; _Create_ >; _LookDev_ >; _Environment Library_ to _Assets_ >; _Create_ >; _Rendering_ >; _Environment Library (Look Dev)_.
    
*   Graphics: Changed the menu path for the _Graphics Compositor_ from _Window_ >; _Render Pipeline_ >; _Graphics Compositor_ to _Window_ >; _Rendering_ >; _Graphics Compositor_.
    
*   Graphics: Changed the menu path for the _Look Dev_ window from _Window_ >; _Render Pipeline_ >; _Look Dev_ to _Window_ >; _Analysis_ >; _Look Dev_.
    
*   Graphics: Changed the menu path for the _Render Graph Viewer_ from _Window_ >; _Render Pipeline_ >;\* Render Graph Viewer\* to _Window_ >; _Analysis_ >; _Render Graph Viewer_.
    
*   Graphics: Clamped the `DynamicResolutionHandler.GetScaledSize` function to only return a size value lower than its input size vlue.
    
*   Graphics: Improved IntegrateLDCharlie() to use uniform stratified sampling for faster convergence towards the ground truth.
    
*   Graphics: Improved load asset time for probe volumes.
    
*   Graphics: Improved the quality of RGBM encoded ASTC textures and removed functionality for these to fallback to ETC2.
    
*   Graphics: Improved the warning messages for \[Volumes\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@13.0/manual/Volumes.html) and their Colliders.
    
*   Graphics: LensFlare (SRP) tooltips now refer to meters.
    
*   Graphics: LensFlare Element editor now has a Thumbnail preview.
    
*   Graphics: LWRP package has been deprecated. LWRP package was maintaned with the sole purpose of providing an upgrade path to URP. See URP 2021.2 documentation for notes on how to upgrade LWRP package to 2021.2.
    
*   Graphics: Made it possible to reduce the size of the resolver RenderTarget with \[VirtualTexturing resolver\](https://docs.unity3d.com/2021.2/Documentation/ScriptReference/Rendering.VirtualTexturing.Resolver.UpdateSize.html).
    
*   Graphics: Made occlusion Radius for lens flares in directional lights, be indepeThe occlusion radius of lens flares in directional lights is now independent of the camera's far plane.ndant of the camera's far plane.
    
*   Graphics: Moved _Assets >; Create >; Shader >;Shader Variant Collection_ to _Assets >; Create >; Shader Variant Collection_.
    
*   Graphics: Moved menu item "Decal Projector" to **GameObject** &gt; **Decal Projector**.
    
*   Graphics: Moved menu item "Density Volume" to **GameObject** &gt; **Volume** &gt; **Density Volume**.
    
*   Graphics: Moved menu item "Sky and Fog Volume" to **GameObject** &gt; **Volume** &gt; **Sky and Fog Global Volume**.
    
*   Graphics: New projects that use the 3D project template now use 1920x1080 as the default resolution for the Standalone build target.
    
*   Graphics: New projects that use the 3D project template now use ASTC texture compression for the Android build target.
    
*   Graphics: New projects that use the 3D project template now use DXT5nm-style normal maps for Android, iOS, and tvOS build targets.
    
*   Graphics: New projects that use the 3D project template now use normal quality lightmaps (RGBM-encoded) for Android, iOS, and tvOS build targets.
    
*   Graphics: Removed ability to resize `unity_SpecCubeN_BoxMax` and `unity_SpecCubeN_BoxMin` to encompass the bounds of the object itself, if an SRP is active.
    
*   Graphics: Removed the DYNAMIC\_RESOLUTION snippet from the \[Lens Flare\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@12.0/manual/lens-flare-data-driven-component.html) shader in order to simplify that shader.
    
*   Graphics: Removed the postprocessing package from the core packages list.
    
*   Graphics: Renamed `D32_SFloat_S8_Uint` and `S8_Uint` to `D32_SFloat_S8_UInt` and `S8_UInt` in the `IUnityRenderingExtensions` namespace. Native plug-ins that use the old names need to be updated to use the new name.
    
*   Graphics: Restricted DXT/BCn texture compression to textures with multiple-of-four width and height. This ensures the same behavior as the Texture Importer and requires multiple-of-four dimensions when compressing.
    
*   Graphics: Restricted NPOT (Non-Power-of-Two size) textures to a single mip level if the device does not fully support NPOT. Note that this restriction only affects WebGL 1 devices, and OpenGLES 2.0-based devices that do not support the _OES\_texture\_npot_ extension.
    
*   Graphics: Serialized the Probe Volume asset as binary to improve footprint on disk and loading speed.
    
*   Graphics: Skinned Mesh Renderer GPU skinning job markers are now grouped together in captures, rather than all appearing in the root of the capture, making it easier to navigate.
    
*   Graphics: The **Render Pipeline Debug** window is now the **Rendering Debugger** window, and this new window is now accessible via Windows >; General.
    
*   Graphics: The _Volume Gizmo Color_ is now in _Colors_ >; _Scene_ >; _Volume Gizmo_.
    
*   Graphics: The RTHandleSystem no longer requires a single number of samples for all MSAA textures. You can now set the number of samples independently for all textures.
    
*   Graphics: The Volume Gizmo now renders with an alpha value of 0.125.
    
*   Graphics: Updated the base class to handle additional properties
    
*   Graphics: Updated the icon for IES, LightAnchor and LensFlare.
    
*   Graphics: Updated the IMGUI Debugger to always display on top of other windows.
    
*   Graphics: `ClearFlag.Depth` does not implicitely clear stencil anymore. Added `ClearFlag.Stencil`.
    
*   HDRP: Added **Material Validator** option to the \[Rendering Debugger\]((https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@13.0/manual/Render-Pipeline-Debug-Window.html).
    
*   HDRP: Added a debug setting to the \[Rendering Debugger\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@13.0/manual/Render-Pipeline-Debug-Window.html) to list active XR views.
    
*   HDRP: Added a help box that warns the user when a decal atlas is oversized.
    
*   HDRP: Added a more consistent shading normal calculation for path tracing. This avoids impossible shading/geometric normal combinations. (1323455)
    
*   HDRP: Added an XR single-pass test mode to the \[Rendering Debugger\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@13.0/manual/Render-Pipeline-Debug-Window.html).
    
*   HDRP: Added new sections to the Camera Inspector and improved field layout.
    
*   HDRP: Altered hair to use GGX LTC for area light specular.
    
*   HDRP: Augmented debug visualization for probe volumes.
    
*   HDRP: Cached the base types of the Volume Manager to improve memory and cpu usage.
    
*   HDRP: Changed 'Allow dynamic resolution' from _Rendering_ to _Output_ on the _Camera Inspector_.
    
*   HDRP: Changed custom render callback so when you use it, Global Camera shader constants are pushed automatically.
    
*   HDRP: Changed Density Volume for Local Volumetric Fog.
    
*   HDRP: Changed light reset to preserve type.
    
*   HDRP: Changed Link FOV to Physical Camera, and enabled the ability to show and hide everything on the Projection Section.
    
*   HDRP: Changed normal used in path tracing to create a local light list from the geometric to the smooth shading one.
    
*   HDRP: Changed some light unit slider value ranges to better reflect the lighting scenario.
    
*   HDRP: Changed the Channel Mixer Volume Component UI to show all the channels.
    
*   HDRP: Changed the convergence time of SSGI to 16 frames and the preset value.
    
*   HDRP: Changed the HDRP Render Graph to use the new RendererList API for rendering and (optional) pass culling.
    
*   HDRP: Changed the menu path for _Check Scene Content_ from _Edit_ >; _Render Pipeline_ >; _HD Render Pipeline_ >; _Check Scene Content_ for _Ray Tracing to Edit_ >; _Rendering_ >; _Check Scene Content for HDRP Ray Tracing_.
    
*   HDRP: Changed the menu path for _Edit_ >; _Render Pipeline_ >; _HD Render Pipeline_ >; _Upgrade from Builtin pipeline_ >; _Upgrade Project Materials_ to _High Definition Materials_ to _Edit_ >; _Rendering_ >; _Materials_ >; _Convert All Built-in Materials to HDRP_.
    
*   HDRP: Changed the menu path for _Export HDRP Sky to Image_ from _Edit_ >; _Render Pipeline_ >; _HD Render Pipeline_ >; _Export Sky to Image_ to _Edit_ >; _Rendering_ >; _Export HDRP Sky to Image_.
    
*   HDRP: Changed the menu path for _Render Selected HDRP Camera to log Exr_ from _Edit_ >; _Render Pipeline_ >; _HD Render Pipeline_ >; _Render Selected Camera to log Exr_ to _Edit_ >; _Rendering_ >; _Render Selected HDRP Camera to log Exr_.
    
*   HDRP: Changed the menu path for the _HDRP Wizard_ from _Window_ >; _Render Pipeline_ >; _HD Render Pipeline Wizard_ to _Window_ >; _Rendering_ >; _HDRP Wizard_.
    
*   HDRP: Changed the name of FOV Axis to Field of View Axis.
    
*   HDRP: Changed the NVIDIA install button to the standard FixMeButton.
    
*   HDRP: Changed the property Sorting Priority for the Materials with Transparent Surface type so that it is clamped on the UI from -50 to 50.
    
*   HDRP: Changed the resolution of the sky used for camera misses in Path Tracing to match the resolution of the render buffer. ([1304114](https://issuetracker.unity3d.com/issues/hdrp-dxr-pathtracer-renders-hdri-with-a-lower-resolution-than-rasterization))
    
*   HDRP: Changed the storage format of volumetric clouds presets for easier editing.
    
*   HDRP: Changed the tooltip for color shadows and semi-transparent shadows. (1307704)
    
*   HDRP: Changed the top level menu for consistency between HDRP and URP by moving **Edit/Render Pipeline/HD Render Pipeline/Upgrade from Builtin pipeline/Upgrade Scene Terrains to High Definition Terrains** to **Edit/Rendering/Materials/Convert Scene Terrains to HDRP Terrains**.
    
*   HDRP: Changed the top level menu for consistency between HDRP and URP by moving **Edit/Render Pipeline/HD Render Pipeline/Upgrade from Builtin pipeline/Upgrade Selected Materials to High Definition Materials** to **Edit/Rendering/Materials/Convert Selected Built-in Materials to HDRP**.
    
*   HDRP: Changed where _HDRP Global Settings_ are saved to their own asset (HDRenderPipelineGlobalSettings) and HDRenderPipeline's default asset refers to this new asset.
    
*   HDRP: Copied and referenced the default LookDev volume profile in the Asset folder instead of the package folder.
    
*   HDRP: Debug information for HDRP's \[Render Graph\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@12.0/manual/render-graph-system.html) is now available in the \[Rendering Debug Panel\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@13.0/manual/Render-Pipeline-Debug-Window.html).
    
*   HDRP: Density Volumes can now use a 3D RenderTexture as a mask, and that mask can use the RGBA format for RGB fog.
    
*   HDRP: Disabled specular occlusion for what we consider medium and larger scale ao >; 1.25 with a 25cm falloff interval.
    
*   HDRP: Disabled TAA jitter while using Frame Debugger.
    
*   HDRP: Disabled TAA sharpening on the alpha channel.
    
*   HDRP: Displayed an info box and disabled MSAA asset entry when ray tracing is enabled.
    
*   HDRP: Fixed a null ref exception which appeared while running playmode tests with the \[Rendering Debugger\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@13.0/manual/Render-Pipeline-Debug-Window.html) window open.
    
*   HDRP: Fixed upscaling issue that is exaggerated by DLSS. ([1347250](https://issuetracker.unity3d.com/issues/hdrp-dlss-with-volumetric-clouds-lower-the-resolution-below-a-quarter-and-makes-the-results-very-pixelated))
    
*   HDRP: Hybrid duplicated reflection probes set to br ignored during light baking.
    
*   HDRP: Improved how the HDRP Wizard handles the Render Pipeline settings. The section Global contains data from the HDRP Settings section and the Render Pipeline Asset property in Project Settings >; Graphics. The section Current Quality contains data from the Render Pipeline Asset property in the Quality level that is currently in use.
    
*   HDRP: Improved labels for cloud scroll direction and cloud type.
    
*   HDRP: Improved lighting models for AxF shader area lights.
    
*   HDRP: Improved physically-based _Depth of Field_ with better near defocus blur quality.
    
*   HDRP: Improved screen space global illumination.
    
*   HDRP: Improved shadow cascade GUI drawing with pixel perfect, hover, and focus functionalities.
    
*   HDRP: Improved the area cookie behavior for higher smoothness values to reduce artifacts.
    
*   HDRP: Improved the fly through ghosting artifacts in the volumetric clouds.
    
*   HDRP: Improved the performance and visual quality of the clamping approach for RTR and RTGI.
    
*   HDRP: Improved the RTGI denoising.
    
*   HDRP: Improved volumetric clouds (added new noise for erosion, reduced ghosting while flying through, altitude distortion, and ghosting when changing from local to distant clouds, fixed issue in wind distortion along the Z axis).
    
*   HDRP: Increased the minimum density of the volumetric clouds.
    
*   HDRP: It is now considered a miss when a ray hits the sky in the ray marching part of mixed ray tracing.
    
*   HDRP: Made debug panel mip bias functions internal, not public.
    
*   HDRP: Made LitTessellation and LayeredLitTessellation fallback on Lit and LayeredLit respectively, in DXR.
    
*   HDRP: Made various improvements to the volumetric clouds.
    
*   HDRP: Modified the history validation pass so that Unity only performs it once for each frame and not for every effect.
    
*   HDRP: Moved invariants outside of loop to speed up CPU in the light loop code.
    
*   HDRP: Moved MaterialHeaderScopes to Core.
    
*   HDRP: Moved menu item "C# Custom Pass" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **HDRP C# Custom Pass**.
    
*   HDRP: Moved menu item "C# Post Process Volume" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **HDRP C# Post Process Volume**.
    
*   HDRP: Moved menu item "Custom FullScreen Pass" to **Assets** &gt; **Create** &gt; **Shader** &gt; **HDRP Custom FullScreen Pass**.
    
*   HDRP: Moved menu item "Custom Renderers Pass" to **Assets** &gt; **Create** &gt; **Shader** &gt; **HDRP Custom Renderers Pass**.
    
*   HDRP: Moved menu item "Decal Shader Graph" to **Assets** &gt; **Create** &gt; **Shader Graph** &gt; **HDRP** &gt; **Decal Shader Graph**.
    
*   HDRP: Moved menu item "Diffusion Profile" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **HDRP Diffusion Profile**.
    
*   HDRP: Moved menu item "Eye Shader Graph" to **Assets** &gt; **Create** &gt; **Shader Graph** &gt; **HDRP** &gt; **Eye Shader Graph**.
    
*   HDRP: Moved menu item "Eye Shader Graph" to **Assets** &gt; **Create** &gt; **Shader Graph** &gt; **HDRP** &gt; **Hair Shader Graph**.
    
*   HDRP: Moved menu item "Fabric Shader Graph" to **Assets** &gt; **Create** &gt; **Shader Graph** &gt; **HDRP** &gt; **Decal Fabric Shader Graph**.
    
*   HDRP: Moved menu item "High Definition Render Pipeline Asset" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **HDRP Asset**.
    
*   HDRP: Moved menu item "Lit Shader Graph" to **Assets** &gt; **Create** &gt; **Shader Graph** &gt; **HDRP** &gt; **Lit**.
    
*   HDRP: Moved menu item "Post Process Pass" to **Assets** &gt; **Create** &gt; **Shader** &gt; **HDRP Post Process**.
    
*   HDRP: Moved menu item "StackLit Shader Graph" to **Assets** &gt; **Create** &gt; **Shader Graph** &gt; **HDRP** &gt; **StackLit Shader GraphShader Graph**.
    
*   HDRP: Moved menu item "Unlit Shader Graph" to **Assets** &gt; **Create** &gt; **Shader Graph** &gt; **HDRP** &gt; **Unlit Shader Graph**.
    
*   HDRP: Moved some Volumetric clouds properties to the additional properties section. (1357926)
    
*   HDRP: Moved the Decal Gizmo Color initialization to preferences.
    
*   HDRP: Moved the `supportRuntimeDebugDisplay` option from HDRPAsset to HDRPGlobalSettings.
    
*   HDRP: Reduced the maximum distance per ray step of volumetric clouds.
    
*   HDRP: Refactored platform abstraction code for shader optimization.
    
*   HDRP: Removed an unnecessary `RenderGraphBuilder.ReadTexture`call in the **Set Final Target** pass.
    
*   HDRP: Removed backplate from rendering of lighting cubemaps.
    
*   HDRP: Removed redundant checkboxes (Show Inactive Objects and Isolate Selection) from the Emissive Materials tab of the Light Explorer.
    
*   HDRP: Removed the Bilinear and Lanczos upscale filter.
    
*   HDRP: Removed the MaterialPass option from probe volume _Evaluation_ modes.
    
*   HDRP: Removed the option for reflection probes to render SSAO, SSGI, SSR, ray tracing effects, or volumetric reprojection.
    
*   HDRP: Renamed the "Link Light Layer" property to "Custom Shadow Layer".
    
*   HDRP: Renamed the **Cloud Offset** property in the **Volume** component of **Volumetric Clouds** to **Cloud Map Offset**. (1358528)
    
*   HDRP: Renamed the Decal Projector to HDRP Decal Projector.
    
*   HDRP: Replaced the context menu with a search window when you add a custom pass.
    
*   HDRP: Restored the old version of the RendererList structs/API for compatibility.
    
*   HDRP: Split up the HDProjectSettings with the new HDUserSettings in UserProject. Now the Wizard working variable should not intefere with the versioning tool. (1330640)
    
*   HDRP: Surfaced`ReflectionTypeLoadExceptions` in `HDUtils.GetRenderPipelineMaterialList()` to allow you to act on any reflection errors in the HDRP assembly.
    
*   HDRP: The **Ambient Mode** property of the **Sky** settings for the \[Visual Environment\](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@13.0/manual/Override-Visual-Environment.html) component is now **Dynamic** by default.
    
*   HDRP: The **Render Pipeline Debug** window is now the **Rendering Debugger** window, and this new window is now accessible via Windows >; General.
    
*   HDRP: The default black texture to use for mixed reality is now opaque. It's alpha value is now 1 whereas previously it was 0.
    
*   HDRP: The depth of field at half or quarter resolution is now computed consistently with the full resolution option. (1335687)
    
*   HDRP: The Film Grain effect does not affect the alpha channel now.
    
*   HDRP: The minimal Fog Distance value in the Density Volume is now 0.05.
    
*   HDRP: The URP Asset Inspector **General** section is now **Rendering**.
    
*   HDRP: Updated the HDRP config package so that it is embeded instead of copied locally. The `Packages` folder is versioned by Collaborate. ([1276518](https://issuetracker.unity3d.com/issues/hdrp-config-package-does-not-download-when-using-collaborate-slash-cloud-build))
    
*   HDRP: Updated the recursive rendering documentation.
    
*   HDRP: Updated the UI for the Frame Settings section: default values in the HDRP Settings section and the Custom Frame Settings property are always editable.
    
*   HDRP: Updated Virtual Texturing Resolver to now perform RTHandle resize logic in HDRP instead of in core Unity.
    
*   HDRP: Used the new API for updating Reflection Probe state (fixes garbage allocation). (1290521)
    
*   iOS: Changed default texture compression format from PVRTC to ASTC.
    
*   License: Disabled the package entitlement feature.
    
*   Mobile: Changed minimum iOS/tvOS version to 12.
    
*   Package: Changed the package display name from "Unity Recorder" to "Recorder" in the package manager.
    
*   Package: Fixed a wrong label for the WebM codec in the _Recorder package_.
    
*   Package: Prevented invalid GPU callback data from being written to a frame for the Recorded; this change skips the problematic frame and logs an error message.
    
*   Package: Removed legacy Recorders: MP4, EXR, PNG, WEBM and GIF Animation from the Recorder package.
    
*   Package: Visual Scripting: Changed NotEquals node in non-scalar mode to be consistent with Equals.
    
*   Package Manager: Changed location of the Git LFS cache enabled by setting the `UPM_ENABLE_GIT_LFS_CACHE`'s environment variable to always be located under the global cache root, even when the cache root location is customized.
    
*   Package Manager: Changed the error and warning box to look like the info box.
    
*   Package Manager: Renamed the _Import again_ button to _Reimport_.
    
*   Package Manager: Updated In App Purchasing package to include missing documentation.
    
*   Physics: Adjusted anchor position based on anchor/parentAnchor transforms to better fit the expected result.
    
*   Profiler: The Unity Profiler now only shows threads that have profiler markers generated since you opened the Profiler.
    
*   Profiler: This release contains stability and performance improvements of the Profile Analyzer package. For more information, see the \[Profile Analyzer Changelog\](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.1/changelog/CHANGELOG.html) page.
    
*   Scene/Game View: Changed the default shortcut for the _Show Overlay_ menu option to _Spacebar_.
    
*   Scene/Game View: Fixed styling issues with the _Overlays_ feature.
    
*   Scene/Game View: Moved Component Tools Overlay to the regular Tools Overlay.
    
*   Scene/Game View: Updated the new default shortcut for Toggle overlays to "\`".
    
*   Scripting: Quaternion ToString() prints five decimal digits by default. (36265)
    
*   Scripting: Vector2, Vector3, Vector4, Bounds, Plane, Ray, Ray2D ToString by default prints two decimal digits (up from one). (1205206)
    
*   Search: ref:`now only searches results that have a direct dependency on`.
    
*   Search: Removed the resource Search Provider (res:).
    
*   Services: In the In-App Purchasing (IAP) Settings, when IAP package version 2 or less is installed, the "Migrate" button section is no longer available.
    
*   Shadergraph: Added borders to the Graph Inspector item style, to differentiate between separate items better.
    
*   Shadergraph: Adjusted the Blackboard article to clarify multi-select functionality.
    
*   Shadergraph: Changed BranchOnInputNode to choose NotConnected branch when generating a preview.
    
*   Shadergraph: Changed the "Create Node" action in ShaderGraph stack separator context menu to "Add Block Node" and added it to the main stack context menu.
    
*   Shadergraph: Condensed report errors and warnings to a single error for ShaderGraph SubGraphs.
    
*   Shadergraph: Fixed an issue to ensure that enum keywords may not have duplicate reference names or invalid characters. ([1287335](https://issuetracker.unity3d.com/issues/shadergraph-choosing-two-enum-keyword-display-names-that-dont-overlap-but-make-the-reference-names-overlap-causes-desync))
    
*   Shadergraph: Improved docs for SampleTexture2D, SampleTexture2DLOD, SampleTexture2DArray, SampleTexture3D, SampleCubemap, SampleReflectedCubemap, TexelSize, NormalFromTexture, ParallaxMapping, ParallaxOcclusionMapping, Triplanar, Sub Graphs, and Custom Function Nodes to reflect changes to texture wire data structures.
    
*   Shadergraph: Improved documentation for Swizzle Node.
    
*   Shadergraph: In Unity 2021.2, if you select more than 20 items in the Shader Editor, the Graph Inspector shows only the first 20 selected nodes.
    
*   Shadergraph: Modified the the shader permutation variant limit so that only ShaderGraph keywords count towards the limit; SubGraph keywords do not.
    
*   Shadergraph: Moved menu item "Blank Shader Graph" to **Asset** &gt; **Create** &gt; **Shader Graph** &gt; **Blank Shader Graph**.
    
*   Shadergraph: Moved menu item "Sub Graph" to **Asset** &gt; **Create** &gt; **Shader Graph** &gt; **Sub Graph**.
    
*   Shadergraph: Moved menu item "VFX Shader Graph" to **Asset** &gt; **Create** &gt; **Shader Graph** &gt; **VFX Shader Graph**.
    
*   Shadergraph: Properties and Keywords are no longer separated by type on the blackboard. Categories now allow for any combination of properties and keywords to be grouped together as the user defines.
    
*   Shadergraph: Updated the Custom Function node to use the new ShaderInclude asset type instead of the TextAsset type. The node performs the .hlsl and .cginc checks.
    
*   Shadergraph: Updated/corrected View Direction doc.
    
*   Shadergraph: Vector2/Vector3/Vector4 property types will now be properly represented by a matching Vector2/Vector3/Vector4 UI control in the URP + HDRP Material Inspector as opposed to the fallback Vector4 field that was used for any multi-dimensional vector type.
    
*   Shaders: Added a shader warning for when reserved constants names with consecutive underscores are used.
    
*   Shaders: Increased the global keyword limit to 384.
    
*   Shaders: Shader compiler logs are now generated in a project's **Logs** folder instead of the **Library** folder.
    
*   Shaders: The methods Shader.DisableKeyword, Shader.IsKeywordEnabled, and CommandBuffer.DisableKeyword will no longer create a global keyword if the keyword does not exist.
    
*   Tests: Changed iOS automation code so that it uses `Shell.ExecuteProgramAndGetStdout` for process handling.
    
*   UI Toolkit: By default, rendering data of `VisualElements` with an opacity of zero is now generated and remains up-to-date, allowing animation in opacity without causing performance drops.
    
*   UI Toolkit: Marked the com.unity.ui package, which is incompatible with 21.2 and above, as deprecated.
    
*   UI Toolkit: Optimized some data access for Live Reload feature.
    
*   UI Toolkit: Optimized some data access for the _Live Reload_ feature.
    
*   UI Toolkit: Removed additional overhead of attaching to panel for Live Reload when the option is turned off to improve performance in loading VisualTreeAssets.
    
*   UI Toolkit: URLs in UXML and USS files now support explicit GUID-based asset references. This allows assets referenced by UI assets to be renamed or moved within your project without breaking asset references. The UI Builder saves both UXML and USS files using this format. Note that this URL format is backward-compatible, but the URL query parameters are ignored in older Unity versions.
    
*   Universal: Added Depth and DepthNormals passes to particle shaders.
    
*   Universal: Deprecated GetShadowFade in Shadows.hlsl. Use GetMainLightShadowFade or GetAdditionalLightShadowFade instead.
    
*   Universal: Enabled subsurface scattering with global illumination for handwritten Universal ST8 shaders.
    
*   Universal: Improved shadow cascade GUI drawing with pixel perfect, hover and focus functionalities.
    
*   Universal: Material editor now uses the same MaterialHeaderScope as HDRP.
    
*   Universal: Modified URP profiling scopes. Remove low impact scopes from the command buffer to improve performance. Fixed the name and invalid scope for the context.submit() scope. Changed the default profiling name of ScriptableRenderPass to Unnamed\_ScriptableRenderPass.
    
*   Universal: Moved menu item "2D Renderer" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **URP 2D Renderer**.
    
*   Universal: Moved menu item "Forward Renderer" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **URP Forward Renderer**.
    
*   Universal: Moved menu item "Lit Shader Graph" to **Asset** &gt; **Create** &gt; **Shader Graph** &gt; **URP** &gt; **Lit Shader Graph**.
    
*   Universal: Moved menu item "Pipeline Asset (2D Renderer)" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **URP Asset (with 2D Renderer)**.
    
*   Universal: Moved menu item "Pipeline Asset" (Forward Renderer) to **Assets** &gt; **Create** &gt; **Rendering** &gt; **URP Asset (with Forward Renderer)**.
    
*   Universal: Moved menu item "Post-process Data" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **URP Post-process Data**.
    
*   Universal: Moved menu item "Renderer Feature" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **URP Renderer Feature**.
    
*   Universal: Moved menu item "Sprite Lit Shader Graph" to **Asset** &gt; **Create** &gt; **Shader Graph** &gt; **URP** &gt; **Sprite Lit Shader Graph**.
    
*   Universal: Moved menu item "Sprite Unlit Shader Graph" to **Asset** &gt; **Create** &gt; **Shader Graph** &gt; **URP** &gt; **Sprite Unlit Shader Graph**.
    
*   Universal: Moved menu item "Unlit Shader Graph" to **Asset** &gt; **Create** &gt; **Shader Graph** &gt; **URP** &gt; **Unlit Shader Graph**.
    
*   Universal: Moved menu item "Upgrade Project Materials to 2D Renderer Materials" to **Edit** &gt; **Rendering** &gt; **Materials** &gt; **Convert All Built-in Materials to URP 2D Renderer**.
    
*   Universal: Moved menu item "Upgrade Project Materials to URP Materials" to **Edit** &gt; **Rendering** &gt; **Materials** &gt; **Convert All Built-in Materials to URP**.
    
*   Universal: Moved menu item "Upgrade Project URP Parametric Lights to Freeform" to **Edit** &gt; **Rendering** &gt; **Lights** &gt; **Convert Project URP Parametric Lights to Freeform**.
    
*   Universal: Moved menu item "Upgrade Scene Materials to 2D Renderer Materials" to **Edit** &gt; **Rendering** &gt; **Materials** &gt; **Convert All Built-in Scene Materials to URP 2D Renderer**.
    
*   Universal: Moved menu item "Upgrade Scene URP Parametric Lights to Freeform" to **Edit** &gt; **Rendering** &gt; **Lights** &gt; **Convert Scene URP Parametric Lights to Freeform**.
    
*   Universal: Moved menu item "Upgrade Selected Materials to URP Materials" to **Edit** &gt; **Rendering** &gt; **Materials** &gt; **Convert Selected Built-in Materials to URP**.
    
*   Universal: Moved menu item "XR System Data" to **Assets** &gt; **Create** &gt; **Rendering** &gt; **URP XR System Data**.
    
*   Universal: Moved the code that evaluates the fog from the vertex shader to the pixel shader. This improves the rendering of fog for big triangles and the fog quality. This can change the look of the fog slightly.
    
*   Universal: Optimized the Bokeh Depth of Field shader on mobile by using half precision floats.
    
*   Universal: Reduced the size of the fragment input struct of the TerrainLitPasses, LitGBufferPass, SimpleLitForwardPass, and SimpleLitGBufferPass lighting shaders.
    
*   Universal: Removed unused temporary depth buffers for Depth of Field and Panini Projection.
    
*   Universal: Renamed the Forward Renderer asset to the Universal Renderer asset. The Universal Renderer asset contains the Rendering Path property, which you can set to either the Forward Rendering Path or the Deferred Rendering Path.
    
*   Universal: Renamed UniversalRenderPipelineCameraEditor to URPCameraEditor.
    
*   Universal: Shadow fade now uses border value for calculating shadow fade distance and fall off linearly.
    
*   Universal: The DepthNormals passes sample the normal maps if the passes run on a Material now, otherwise the passes output the geometry normals.
    
*   Universal: The format of the SSAO texture is now R8 instead of ARGB32 on platforms that support the format.
    
*   Universal: The function to upgrade from LWRP to URP was removed. If you want to upgrade your ptoject from LWRP to URP, you must first upgrade to a previous URP version, and then upgrade to this version.
    
*   Universal: The method ClearFlag.Depth does not implicitly clear the Stencil buffer anymore. Use the new method ClearFlag.Stencil.
    
*   Universal: The Opacity as Density blending feature for the Terrain Lit shader is now disabled when the Terrain object has more than four Terrain Layers. This behavior is now similar to the Height-blend feature of the Terrain Lit shader.
    
*   Universal: The performance of the Bokeh mode of the Depth of Field effect is improved. The CPU performs certain caluculations instead of the GPU now.
    
*   Universal: The property Advanced Options >; Priority is renamed to Sorting Priority.
    
*   Universal: The UNITY\_Z\_0\_FAR\_FROM\_CLIPSPACE macro now remaps the coordinates to the \[0, far\] range on all platforms consistently. Previously, Unity did not perform the remapping on OpenGL platforms, discarding the range \[-near, 0\].
    
*   URP: Added shadergraph support for VFX directly on Universal target.
    
*   URP: Changed 2D Lights to inherit from Light2DBase.
    
*   URP: Changed material upgrader to upgrade AnimationClips in projects that have curves bound to renamed material properties.
    
*   URP: Changed Pixel Snapping and Upscale Render Texture in the PixelPerfectCamera to a dropdown.
    
*   URP: Changed process to stripping shader variants per renderer feature instead of combined renderer features.
    
*   URP: Changed the default name of new URP assets.
    
*   URP: Changed the opaque pass depth to be copied instead of scheduling a depth prepass when MSAA is enabled and a depth texture is required.
    
*   URP: Improved PixelPerfectCamera UI/UX.
    
*   URP: Made 2D shadow casting more efficient.
    
*   URP: Modified the behavior of setting a camera's Background Type to "Dont Care" on mobile. "Dont Care" now fills the render target with arbitrary data at the beginning of the frame, which might be faster in some situations. Note that there are no guarantees for the exact content of the render target, so projects should only use "Dont care" if they are guaranteed to render to, or otherwise write every pixel every frame.
    
*   URP: Moved all 2D APIs out of the experimental namespace.
    
*   URP: Moved the advanced settings in eachg section of the the URP Asset Inspector to **Show Additional Properties**.
    
*   URP: Refactored some of the array resizing code around decal projector rendering to use new APIs in render core.
    
*   URP: Reversed `UniversalRendererData` and `ForwardRendererData` GUIDs to improve the upgrade experience from Unity versions 2019LTS, 2020LTS and 2021.1. Issues upgrading 2021.2 Alpha/Beta versions and are recommended to start with a fresh library if initial upgrade fails.
    
*   URP: Updated URP to no longer render via an intermediate texture unless actively required by a Renderer Feature. See the upgrade guide for compatibility options and how assets are upgraded.
    
*   URP: URP Asset Inspector - `General` section has been renamed to `Rendering`.
    
*   Version Control: Improved usage analytics around Editor and Plugin version. Made workspace migration adjustments.
    
*   Version Control: Made the following improvements for Plastic SCM:  
    
    *   Updated license to better conform with expected customer usage.  
        
    *   Updated documentation file to meet standards.  
        
    *   Updated third-party usage.  
        
    *   No longer requires downloading of the full Plastic client. Basic features work without additional installation. Features that require the full Plastic client will allow download and install as needed.  
        
    *   Usability improvements around checking in code.  
        
    *   Improved update workspace tab UX.  
        
    *   Plastic SCM context menu is now available even if the Plastic SCM window is closed.
*   Version Control: Simplified and decluttered UI.
    
*   VFX Graph: Allowed the remaking of existing links.
    
*   VFX Graph: Integrated Transform to VFXTypes : Circle, ArcCircle, Sphere, ArcSphere, Torus, ArcTorus, Cone, ArcCone.
    
*   VFX Graph: Moved menu item "Point Cache Bake Tool" to **Window** &gt; **VFX** &gt; **Utilities** &gt; **Point Cache Bake Tool**.
    
*   VFX Graph: Moved menu item "Rebuild And Save All VFX Graphs" to **Edit** &gt; **VFX** &gt; **Rebuild And Save All Visual Effect Graphs**.
    
*   VFX Graph: Moved menu item "Visual Effect Defaults" to **Assets** &gt; **Create** &gt; **VFX** &gt; **VFX Defaults**.
    
*   VFX Graph: Moved menu item "Visual Effect Graph" to **Assets** &gt; **Create** &gt; **VFX** &gt; **VFX Graph**.
    
*   VFX Graph: Moved menu item "Visual Effect Graph" to **Window** &gt; **VFX** &gt; **VFX Graph**.
    
*   VFX Graph: Moved menu item "Visual Effect Subgraph Block" to **Assets** &gt; **Create** &gt; **VFX** &gt; **VFX Subgraph Block**.
    
*   VFX Graph: Moved menu item "Visual Effect Subgraph Operator" to **Assets** &gt; **Create** &gt; **VFX** &gt; **VFX Subgraph Operator**.
    
*   VFX Graph: Property Binder : Handle Remove Component removing linked hidden scriptable objectfields.
    
*   VFX Graph: Property Binder : Prevent multiple VFXPropertyBinder within the same game object.
    
*   VFX Graph: Sphere and Cube outputs are now experimental.
    
*   Virtual Texturing: Updated `PopRequests` to allow the destination list to have a different size than the texture stack's `maxActiveRequests` value.
    
*   WebGL: Eliminated the Python dependency from the Brotli compressor.
    

### Fixes

*   2D: 2D light is rendered in half in its Y-axis when two Sprite Shape objects with same Order In Layer are visible on the Screen ([1274010](https://issuetracker.unity3d.com/issues/2d-light-is-rendered-in-half-in-its-y-axis-when-two-sprite-shape-objects-with-same-order-in-layer-are-visible-on-the-screen))
    
*   2D: Add null arguments checks for Sprite.GetPhysicsShape, Sprite.OverridePhysicsShape and Sprite.OverrideGeometry ([1306258](https://issuetracker.unity3d.com/issues/crash-when-spriterenderer-dot-sprite-dot-getphysicsshape-gets-null-passed-in-as-physicsshape-parameter))
    
*   2D: Call Tilemap.tilemapChanged callback when Tilemap component is reset or ResizeBounds is called. ([1304936](https://issuetracker.unity3d.com/issues/tilemap-does-not-invoke-tilemap-dot-tilemaptilechanged-event-when-tilemap-component-is-reset))
    
*   2D: Fix crash when loading a scene with a GameObject with an invalid Tilemap and a TilemapCollider2D. ([1314326](https://issuetracker.unity3d.com/issues/crash-on-tilemapcollider2d-prepareshapes-when-enabling-a-broken-tilemap))
    
*   2D: Fix issue with the Sorting Group where the sorted renderers are not in hierarchical order when their sorting criteria are the same. ([1309075](https://issuetracker.unity3d.com/issues/objects-of-the-sortinggroup-are-sorted-incorrectly-after-instantiating-new-objects-inside-of-sortinggroup-member))
    
*   2D: Fix Sprite Preview in inspector becomes unrecognizable when Sprite size is big ([1299189](https://issuetracker.unity3d.com/issues/sprite-preview-window-loses-pixels-and-the-sprites-are-indistinguishable-when-the-sprite-is-either-too-tall-or-too-wide))
    
*   2D: Fixed 2D Animation manual documentation.
    
*   2D: Fixed 2D Animation package description.
    
*   2D: Fixed 2D PSDImporter doesn't apply settings from Sprite Editor Window when changes made in Inspector. (1339799)
    
*   2D: Fixed 2D PSDImporter package description.
    
*   2D: Fixed an issue where Name and Texture fields were overlapping with each other in the Secondary Textures module of the Sprite Editor. ([1284356](https://issuetracker.unity3d.com/issues/2d-the-name-and-texture-fields-are-overlapping-with-each-other-in-secondary-textures))
    
*   2D: Fixed Bone and Sprite influence lists to display correctly. (1349041)
    
*   2D: Fixed duplication of Tilemap Selection Box when the Grid and the Tilemap are offset in transform. ([1293341](https://issuetracker.unity3d.com/issues/2d-tilemap-selection-duplicating-when-cell-anchors-and-scale-altered))
    
*   2D: Fixed exception thrown when manually adding vertices in the Skinning Editor to a Sprite without mesh. (1340105)
    
*   2D: Fixed exception when adding a new Rule when no Rule is selected.
    
*   2D: Fixed extrusion of CompositeCollider2D when an offset distance has been set. ([1328999](https://issuetracker.unity3d.com/issues/composite-collider-2d-inconsistent-offset-results-when-duplicated))
    
*   2D: Fixed GridSelection on a Tile Palette losing its target when the Tile Palette is saved. (1327582)
    
*   2D: Fixed initial rendering animated tiles when a CompleteObjectUndo is registered for a Tilemap while in Play mode.
    
*   2D: Fixed issue when the size of a GridSelection is set to negative values. ([1318891](https://issuetracker.unity3d.com/issues/2d-multiple-errors-thrown-continuously-on-resizing-the-grid-size-of-tilemap))
    
*   2D: Fixed issue where Tilemap does not preserve transform changes or color when inserting or deleting cells. (1315084)
    
*   2D: Fixed issue with setting a Spritesheet with padding between Sprites on a Tile Palette having a positional offset when there should not be one.
    
*   2D: Fixed issue with sprite mask debug color when sprite renderers are batched. ([1328538](https://issuetracker.unity3d.com/issues/2d-sprite-mask-sprite-mask-shading-mode-view-is-not-correctly-displayed-when-changing-mask-interaction-or-sorting-layer))
    
*   2D: Fixed mouse position calculation after SceneView overlay changes.
    
*   2D: Fixed MouseDrag including previous mouse positions from initial drag.
    
*   2D: Fixed MouseDrag not including final mouse position after drag.
    
*   2D: Fixed NullReferenceException from being thrown when doing a Grid Select on a Grid which is not enabled. ([1295122](https://issuetracker.unity3d.com/issues/2d-tilemap-nullreferenceexception-in-console-when-grid-component-is-disabled-and-palette-select-tool-is-used))
    
*   2D: Fixed offset placement of Tile placed when dragging in a single Sprite or Tiles onto the Tile Palette window.
    
*   2D: Fixed on deselecting game object from the Inspector window leads to deselecting Sprite Shape Renderer. ([1317728](https://issuetracker.unity3d.com/issues/spriteshapeprofile-on-deselecting-game-object-from-the-inspector-window-leads-to-deselecting-sprite-shape-renderer))
    
*   2D: Fixed Paint tool triggering a Tile Palette edit when Paint tool is active and is removed from the Tile Palette default tools.
    
*   2D: Fixed performance regression in PSDImporter Editor. (1349148)
    
*   2D: Fixed potential Sprite reference lost when upgrading from 2021.1. (1358979)
    
*   2D: Fixed SpriteRect and Name File Id does not match in meta file. (1319819)
    
*   2D: Make tooltips appear closer to the label for Tilemap Info in the Tilemap Editor rather than in the center. (1294929)
    
*   2D: Mark com.unity.2d.tilemap.extras as discoverable
    
*   2D: Prevent Tile Palette Prefabs from showing as a Active Target for the Tile Palette window when selected.
    
*   2D: Prevented users from selecting a disabled GameObject as an active target for the Tile Palette. ([1327021](https://issuetracker.unity3d.com/issues/2d-tilemap-palette-windows-active-tilemap-still-shows-tilemap-which-is-disabled-in-sceneview))
    
*   2D: Removes GC.Alloc when Tilemap.HasSyncTileCallback is called which is internally called for each SetTile/s.
    
*   2D: Sprite Atlas importer does not show name on top (1300861)
    
*   2D: Swapped behavior of rotating clockwise and counter-clockwise.
    
*   2D: Unable to exclude Objects for Packing property from Sprite Atlas preset ([1294393](https://issuetracker.unity3d.com/issues/unable-to-exclude-objects-for-packing-property-from-sprite-atlas-preset))
    
*   AI: Fixed a crash when exiting play mode while a NavMesh asynchronous update call is being scheduled. ([1297742](https://issuetracker.unity3d.com/issues/crash-on-entering-play-mode-when-a-script-is-calling-navmeshsurface-dot-updatenavmesh))
    
*   AI: Fixed crashes from building from meshes larger than the allowed size threshold. ([1298356](https://issuetracker.unity3d.com/issues/crash-on-rasterizetri-when-baking-navmesh))
    
*   AI: Fixed issue where the NavMeshModifierBox did not override the area type with existing higher index. ([1078153](https://issuetracker.unity3d.com/issues/a-navmesh-modifier-volume-gets-overridden-by-a-navmesh-area-which-is-further-in-the-area-list))
    
*   AI: Fixed the gizmos of navigation OffMeshLinks when the distance from start to end is small. (805223)
    
*   Android: Added a new AndroidDevice.hardwareType property, which is set to AndroidHardwareType.ChromeOS if running on a Chrome OS device. This is helpful if an app needs to run Chrome OS-specific code.
    
*   Android: Added a warning if making an IL2CPP Android build without Arm64 binaries (1318322)
    
*   Android: Added fullscreen flag to manifest to better handle static splash screen. ([1310347](https://issuetracker.unity3d.com/issues/custom-static-image-for-splash-screen-moves-on-android-build-when-loading))
    
*   Android: Android: Fix lightmap quality warning text in PlayerSettings. (1337631)
    
*   Android: Clamp Android minimum bundle version to greater than 0 ([1307476](https://issuetracker.unity3d.com/issues/android-gradle-build-fails-when-the-bundle-version-code-value-is-lower-than-1))
    
*   Android: Fix high memory usage for textures when uploading textures at runtime using Vulkan ([1300900](https://issuetracker.unity3d.com/issues/vulkan-mono-the-amount-of-memory-allocated-for-textures-on-vulkan-is-significantly-higher-compared-to-gles3))
    
*   Android: Fix rendering errors when trying to use Particle Systems with instancing on devices that don't support it ([1312433](https://issuetracker.unity3d.com/issues/particle-system-with-mesh-render-mode-causes-glsl-link-error-on-android-mali-devices))
    
*   Android: Fixed Android build failures due to unsupported manifest features when targeting API 23 or below. ([1340517](https://issuetracker.unity3d.com/issues/android-cannot-build-with-target-and-min-sdk-set-to-22))
    
*   Android: Fixed artifacts when exceeding geometry working set memory limit on Mali GPUs when using Vulkan GraphicsJobs.
    
*   Android: Fixed Build&Run when apk name contains duoble quote. ([1323395](https://issuetracker.unity3d.com/issues/linux-android-apk-is-built-but-not-installed-when-you-build-and-run-with-a-file-name-containing-a-special-character))
    
*   Android: Fixed compatibility with OpenGL ES shaders in asset bundles built with Unity 2018.x or older. ([1329702](https://issuetracker.unity3d.com/issues/android-material-is-rendered-black-in-devices-using-adreno-gpus-when-loaded-from-asset-bundle-created-using-unity-2018))
    
*   Android: Fixed computeBufferStartIndex of ComputeBuffer.GetData being ignored when using Vulkan. ([1299902](https://issuetracker.unity3d.com/issues/computebuffer-dot-getdata-buffer-offset-count-does-not-take-offset-into-account-on-vulkan))
    
*   Android: Fixed crash during shutdown on Adreno devices when using Vulkan. (1330396)
    
*   Android: Fixed crash when using R16 UNorm and similar formats with Vulkan on devices that don't support it. ([1314282](https://issuetracker.unity3d.com/issues/android-adreno-application-crashes-when-loading-a-r16-bit-texture-on-development-builds))
    
*   Android: Fixed incorrect resolution scaling on PowerVR devices when BlitType Auto is used ([1287131](https://issuetracker.unity3d.com/issues/android-resolution-scaling-mode-fixed-dpi-is-not-working-properly-on-some-android-devices))
    
*   Android: Fixed Patch not working on some newer Android devices due to permission issue. (1343844)
    
*   Android: Fixed runtime decompression of ASTC HDR cubemaps on devices that don't support ASTC HDR. (1323739)
    
*   Android: Fixed screen safe area values at startup. ([1327752](https://issuetracker.unity3d.com/issues/safearea-when-device-is-held-in-portrait-app-is-running-in-portrait-upside-down-windowed-mode-safearea-values-are-incorrect))
    
*   Android: Fixed shader compile error when signed bitfieldExtract is generated for ES 3.0 shader target. (1327731)
    
*   Android: Fixed shaders with bitfield operations compilation errors on Adreno3XX GPUs.
    
*   Android: Il2cpp resources will be extracted during player launch only when needed, for ex., changes in scripts. Previously they would be extracted each time you make a new build from Unity.
    
*   Android: Preserve ComputeBuffer data when doing partial updates using ComputeBuffer.SetData ([1300424](https://issuetracker.unity3d.com/issues/partial-updates-of-computebuffer-slash-graphicsbuffer-using-setdata-dont-preserve-existing-data-when-using-opengl-es))
    
*   Android: Resolved an Android build failure when the Target SDK was set to below 24. (1340438)
    
*   Android: Resolved an issue that prevented features such as tessellation and geometry shaders from being marked as supported on Android devices whose driver supports OpenGL ES 3.1 with AEP but not 3.2.
    
*   Android: Updated Kotlin version to fix potential compatibility problems in Android Studio. ([1325245](https://issuetracker.unity3d.com/issues/android-build-fails-because-of-duplicate-classes-when-using-kotlin-plugins-in-your-project))
    
*   Animation: 1D BlendTree's threshold values were draggable when not the hot control. ([1217253](https://issuetracker.unity3d.com/issues/blendtree-1d-parameter-blend-thresholds-can-be-edited-from-any-editor-window-when-value-is-inputted-and-enter-is-pressed))
    
*   Animation: Added a tooltip for the auto live link button in the animator window. ([1283065](https://issuetracker.unity3d.com/issues/animation-tooltip-is-missing-for-the-auto-live-link-button-in-the-animator-window))
    
*   Animation: Added checks to prevent and capture crash for the GetRootBlendTreeChildWeights function. (1282475)
    
*   Animation: Added option to set the single layer optimization for AnimationLayerMixerPlayable that is enable by default in previous version. ([1159548](https://issuetracker.unity3d.com/issues/animationlayermixerplayable-ignores-weight-when-inputcount-is-not-greater-than-1))
    
*   Animation: Fixed a bug where the .controller file would grow in size even after undoing states. ([1194086](https://issuetracker.unity3d.com/issues/unity-animator-controller-data-leak))
    
*   Animation: Fixed a bug where the parameters list being previewed would not display in the inspector window. ([1190190](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-error-is-thrown-when-expanding-transition-blendtree-parameters))
    
*   Animation: Fixed AddAssetToSameFile assert thrown on adding SMB on unpersisted AnimatorState or AnimatorStatemachine. ([1233556](https://issuetracker.unity3d.com/issues/animation-addassettosamefile-failed-exception-thrown-on-adding-script-on-the-preset-of-the-animation-state))
    
*   Animation: Fixed an animation performance test failing on specific device (iOS/Android) (1307702)
    
*   Animation: Fixed an issue when trying to record elements from array where the index elements were 2 or 4. ([1242410](https://issuetracker.unity3d.com/issues/material-is-applied-to-two-slots-when-applying-material-to-a-single-slot-while-recording-animation))
    
*   Animation: Fixed an issue where an animation playable events would still fire while it was paused. ([1227098](https://issuetracker.unity3d.com/issues/playbles-animationstart-and-animationmiddle-are-constantly-called-when-the-playable-is-paused-and-settime-0-is-called))
    
*   Animation: Fixed an issue where the application would crash if modifying the graph while being traversed. ([1282046](https://issuetracker.unity3d.com/issues/editor-crashes-on-animationlayermixerplayable-processrootmotion-after-connecting-timelineplayable-to-animationmixerplayable))
    
*   Animation: Fixed an issue where the checkbox wouldn't align properly with its label in the transition list. ([1259438](https://issuetracker.unity3d.com/issues/imgui-solo-and-mute-transitions-checkbox-positions-are-misaligned))
    
*   Animation: Fixed an issue where the destination state would indicate INVALID instead of the known destination state in the transition list of the inspector window
    
*   Animation: Fixed an issue where the slider of the animation window would go into the hierarchy part of the window when the animation window was too small width wise (1288823)
    
*   Animation: Fixed an issue where the stabilize feet would not get saved upon entering playmode. ([1245722](https://issuetracker.unity3d.com/issues/animator-dot-stabilizefeet-is-set-to-false-after-the-second-time-of-calling-the-update-method-when-using-playables-api))
    
*   Animation: Fixed an issue where the transition to a base layer state machine would be invisible ([1287749](https://issuetracker.unity3d.com/issues/transition-is-invisible-when-connecting-sub-statemachines-that-is-inside-of-another-sub-statemachine-state-to-the-base-layer))
    
*   Animation: Fixed an issue where the transition would automatically disappear if made from a lower layer state machine to an upper layer one. ([1188984](https://issuetracker.unity3d.com/issues/sub-state-machine-transitions-added-to-base-layer-are-discarded-at-runtime))
    
*   Animation: Fixed an issue where the Vector property of the material component would not have a blue tint to highlight it was being animated when in preview mode. ([1333416](https://issuetracker.unity3d.com/issues/vector4-field-of-an-animated-material-is-not-tinted-blue-or-red-when-in-animation-preview-or-recording))
    
*   Animation: Fixed an issue where warnings would appear while typing the first numbers of the time in blend tree before confirming the value. ([1250904](https://issuetracker.unity3d.com/issues/animator-blend-tree-throws-warnings-when-typing-a-decimal-value-to-animation-speed-field))
    
*   Animation: Fixed animation events to fire correctly when overriding the loop in a AnimationClipPlayable. ([1292994](https://issuetracker.unity3d.com/issues/setoverrideloop-in-animationclipplayable-doesnt-work-when-using-with-animationevents))
    
*   Animation: Fixed animation transition preview playback marker to update correctly when window is floating and animation is paused. ([1285405](https://issuetracker.unity3d.com/issues/animation-transition-preview-playback-marker-cannot-be-moved-when-the-preview-window-is-floating-and-animation-is-paused))
    
*   Animation: Fixed Animator MatchTarget to work correctly with longer time. ([1052600](https://issuetracker.unity3d.com/issues/animation-animation-becomes-distorted-after-looping-it-a-certain-amount-of-times-when-using-animator-dot-matchtarget))
    
*   Animation: Fixed BlendTree graph where nodes switch positon when play is pressed. ([1306710](https://issuetracker.unity3d.com/issues/blend-tree-groups-animation-clips-by-their-names-and-connects-them-to-blend-tree-as-one-child-node))
    
*   Animation: Fixed crash upon calling the `MonoManager::TypeToScriptingClass(Unity::Type)` method on a type that has been removed. The solution is to check if the type is valid first with `type-&gt;HasValidRuntimeTypeIndex()`. ([1319992](https://issuetracker.unity3d.com/issues/crash-on-editorcurvebindingtomono-when-animation-tab-is-open-with-a-specific-prefab-selected))
    
*   Animation: Fixed edge highlighting logic with livelink in mecanim with edge cases involving Any State and Entry nodes. ([1171704](https://issuetracker.unity3d.com/issues/animation-transition-is-shown-incorrectly-when-transitioning-from-anystate-to-a-sub-state))
    
*   Animation: Fixed for disappearing Animator State Machine information. ([1307535](https://issuetracker.unity3d.com/issues/animator-state-machine-information-disappears-from-the-inspector-when-hovering-over-the-inspector-while-state-machine-is-opened))
    
*   Animation: Fixed GetLayerWeight function in Animator to always return 1 if getting the base layer weight. ([1315029](https://issuetracker.unity3d.com/issues/animator-getlayerweight-always-returns-0-when-calling-it-on-the-base-layer-index-0))
    
*   Animation: Fixed human pose offset in Animation C# Job when root node is scaled. ([1266529](https://issuetracker.unity3d.com/issues/turning-on-the-rig-builder-in-a-humanoid-chacter-makes-it-sink-into-the-ground))
    
*   Animation: Fixed human pose with missing bones shifting when used in an Animation C# Job. ([1214897](https://issuetracker.unity3d.com/issues/animation-rigging-lower-body-gets-shifted-on-a-specific-rig-when-rig-builder-is-active))
    
*   Animation: Fixed humanoid SetLookAtWeight method for weights larger than 0.5. ([1307253](https://issuetracker.unity3d.com/issues/clampweight-doesnt-behave-correctly-when-set-to-1-and-applied-in-animator-dot-setlookatweight))
    
*   Animation: Fixed manipulation of the Current Blend Value (the red line)in BlendTree Inspector.
    
*   Animation: Fixed nan appearing in AABB when root motion is enabled in a StateMachineBehaviour by initializing MotionXReference structure upon allocation. ([1279206](https://issuetracker.unity3d.com/issues/invalid-aabb-errors-when-applyrootmotion-is-enabled-with-a-script))
    
*   Animation: Fixed ScaleConstraint on child with parent having a nulled scaled axis. ([1243185](https://issuetracker.unity3d.com/issues/scaleconstraint-gets-ignored-on-axes-that-are-set-to-zero-on-parent-gameobject))
    
*   Animation: Fixed slow performance depend on the first selected. ([1236353](https://issuetracker.unity3d.com/issues/significant-performance-drop-depending-on-the-first-clicked-object-that-triggers-the-animation-window-to-load-an-animation))
    
*   Animation: Fixed static analysis warning. (1232341)
    
*   Animation: Fixed use of PropertyStreamHandle with Addressable AnimatorController. ([1341031](https://issuetracker.unity3d.com/issues/cannot-rebind-multipositionconstraint-source-objects-when-animator-controller-is-changed-at-runtime))
    
*   Animation: Fixing an issue where an Animator with Animate Physics ON would apply physics to every transform except the root transform ([1154835](https://issuetracker.unity3d.com/issues/update-mode-animate-physics-doesnt-work-when-a-gameobject-is-animated-with-a-root-bone-and-apply-root-motion))
    
*   Animation: Force grouped animation of GroupColor for material color in URP. ([1212805](https://issuetracker.unity3d.com/issues/sprites-base-color-is-incorrect-at-runtime-when-animation-contains-material-dot-base-color-property))
    
*   Animation: Improved SetTime and GetTime documentation for playables ([1196250](https://issuetracker.unity3d.com/issues/the-first-frame-of-the-animation-playable-is-delayed-when-it-starts-to-play-in-the-play-mode-causing-a-delay-by-one-frame))
    
*   Animation: Removed invalid error messages and display correct inspector when viewing a state with invalid StateMachineBehaviours. ([1319708](https://issuetracker.unity3d.com/issues/argumentnullexception-gets-thrown-when-changing-the-base-class-to-monobehaviour-of-a-script-that-is-attached-to-a-state))
    
*   Animation: Removed multi edit on animator override controller ([1082045](https://issuetracker.unity3d.com/issues/selecting-multiple-animator-override-controller-and-adding-any-animations-to-any-field-overrides-all-the-override-controllers))
    
*   Animation: Stop animation preview when exiting edit mode with Play Mode with Reload Domain disabled to prevent accessing destroyed object. ([1214031](https://issuetracker.unity3d.com/issues/missingreferenceexception-is-thrown-when-entering-playmode-with-reload-domain-disabled-while-animation-clip-is-playing))
    
*   Animation: Updated documentation of playable to document feature of auto adding new port (1227724)
    
*   Asset Bundles: AssetBundle.Unload waits for all asset bundle async operations to be completed before proceeding.
    
*   Asset Bundles: Fixed error being logged when accessing an archive file that was modified while it was still opened. ([1319389](https://issuetracker.unity3d.com/issues/editor-crashes-when-loading-a-scene-from-a-runtime-updated-addressables-catalog))
    
*   Asset Bundles: Fixed issue where Caching.IsVersionCached returns false when loading a previously cached bundle. ([1186310](https://issuetracker.unity3d.com/issues/caching-dot-isversioncached-returns-false-when-loading-bundle-from-cache))
    
*   Asset Bundles: Fixed issue where loading an asset from a bundle asynchronously while loading a texture synchronously causes a deadlock on the main thread.
    
*   Asset Import: Adding a ScriptedImporter attribute to a non-ScriptedImporter class no longer crashes the editor. ([1308671](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-experimental-dot-assetimporters-dot-scriptedimporter-generateassetdata-when-importing-asset-w-slash-scriptedimporter))
    
*   Asset Import: Apply/Revert buttons in the inspector are correctly disabled after changing a value that is being overridden by the Importer script or an AssetPostprocessor. ([1287345](https://issuetracker.unity3d.com/issues/the-inspector-window-indicates-that-there-are-unapplied-changes-after-changing-the-setting-enforced-by-a-postprocessor))
    
*   Asset Import: Assembly Ref / Definition files now have padding. ([1311970](https://issuetracker.unity3d.com/issues/assembly-definition-and-assembly-definition-reference-asset-inspectors-are-missing-padding))
    
*   Asset Import: Changing player settings Graphics APIs while editor is in Android platform no longer reimports all textures, video clips or fonts. ([1329621](https://issuetracker.unity3d.com/issues/assetimport-changing-graphics-apis-in-android-platform-reimports-most-of-the-assets-textures-fonts-dot-dot-dot))
    
*   Asset Import: Editing the animation clip directly from the sub-asset on first import is no longer broken. (1304418)
    
*   Asset Import: Fixed crash when importing FOV animations from 3DsMax. (1324054)
    
*   Asset Import: Fixed crash/corruption when importing animations.
    
*   Asset Import: Fixed missing normal property values from materials imported from 3DsMax 2021's Physical materials. (1313450)
    
*   Asset Import: Fixed Texture Import Platform settings getting reset when multi editing.
    
*   Asset Import: GameObjects & Prefabs can no longer be duplicated using Ctrl + D. ([1304106](https://issuetracker.unity3d.com/issues/duplicating-a-mesh-inside-fbx-container-works-but-throws-errors))
    
*   Asset Import: GatherDependenciesFromSourceFile declared in parent classes is now properly called from derived classes. ([1203843](https://issuetracker.unity3d.com/issues/scriptedimporters-gatherdependenciesfromsourcefile-is-not-executed-when-defined-in-base-class-and-called-from-derived-class))
    
*   Asset Import: ModelImporter now only renames sibling nodes with duplicate names. ([1233702](https://issuetracker.unity3d.com/issues/custom-model-has-incorrect-naming-scheme-when-imported-into-unity))
    
*   Asset Import: New flag to allow rigs with different topologies to be swapped. ([974120](https://issuetracker.unity3d.com/issues/changing-skinned-mesh-causes-unwanted-deformations-when-using-models-with-3ds-max-biped-rig))
    
*   Asset Import: Only call frame rate errors when animations are imported. ([1222562](https://issuetracker.unity3d.com/issues/asset-importer-framerate-errors-are-shown-incorrectly-when-importing-fbx-from-modo))
    
*   Asset Import: Rename of Inspector labels to make them more consistent.
    
*   Asset Import: SearchAndRemap now functions as expected in packages. ([1218857](https://issuetracker.unity3d.com/issues/importing-fbx-files-crashes-unity-when-using-an-assetpostprocessor))
    
*   Asset Import: Switching Texture Importer tabs does not dirty the importer. ([1321256](https://issuetracker.unity3d.com/issues/textureimporter-settings-get-dirtied-upon-switching-platform-setting-views-in-inspector-window-when-used-with-assetpostprocessor))
    
*   Asset Import: The Default Clip selection no longer gets stuck. (1279563)
    
*   Asset Import: Updated Log Warning to include name / object reference (1304432)
    
*   Asset Pipeline: All domain reloads are now done inside asset db. This fixes problem with reloading of asset objects when doing manual refresh. ([1341910](https://issuetracker.unity3d.com/issues/scriptableobject-serialized-fields-get-unassigned-after-importing-when-the-auto-refresh-is-disabled))
    
*   Asset Pipeline: Asset loading is safe in this callback. ([1267939](https://issuetracker.unity3d.com/issues/resources-dot-load-result-returns-false-when-called-from-initializeonload-and-when-the-asset-was-externally-changed))
    
*   Asset Pipeline: Enabled PluginSettingsWorks.WSASettings integration test (1086909)
    
*   Asset Pipeline: Fix for crash that could happen after safe mode exit
    
*   Asset Pipeline: Fixed a crash that could occur when opening a project with a meta file conflict. ([1310334](https://issuetracker.unity3d.com/issues/crash-on-metayaml-write-when-opening-a-project-with-a-meta-file-conflict))
    
*   Asset Pipeline: Fixed a very rare bug causing directory monitor not pick up all the changes that happened before a Refresh.
    
*   Asset Pipeline: Fixed an assert when fetching previews for assets in AssetBundles. ([1311115](https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-request-dot-key-dot-guid-dot-isvalid-when-selecting-a-mesh))
    
*   Asset Pipeline: Fixed an issue where a scene could become corrupt if renamed to match the name of a recently deleted scene. ([1263621](https://issuetracker.unity3d.com/issues/renaming-a-scene-deletes-its-gameobjects-when-a-scene-with-that-name-was-already-deleted))
    
*   Asset Pipeline: Fixed an issue where AssetDatabase.SaveAssetIfDirty() wouldn't save the asset if a sub-object was dirty, but the main object wasn't. (1341834)
    
*   Asset Pipeline: Fixed issue where an invalid GUID was being reported, but the file in which it resided was not. ([1275878](https://issuetracker.unity3d.com/issues/could-not-extract-guid-in-text-file-at-line-error-without-file-name-when-importing-prefab))
    
*   Asset Pipeline: Fixed issue with asset reference getting lost, if asset is modified and domain reload is done in the same refresh. (1357812)
    
*   Asset Pipeline: Fixed issue with incorrect progress bar text during startup. (1339167)
    
*   Asset Pipeline: Fixed issue with missing domain reload when entering play mode and LockReloadAssemblies is set. ([1367222](https://issuetracker.unity3d.com/issues/domain-reload-missing-when-entering-play-mode))
    
*   Asset Pipeline: Fixed issue with some FBX models being imported with a scale of 0 when 'Remove Constant Scale Curves' is enabled. (1348264)
    
*   Asset Pipeline: Fixed missing automatic scale down or import workers in order to not use excess system resources. (1343401)
    
*   Asset Pipeline: Fixed the progress bar being full during the import of assets. ([1298760](https://issuetracker.unity3d.com/issues/the-import-progress-bar-is-not-being-filled-proportionally-to-the-imported-amount-when-importing-assets))
    
*   Asset Pipeline: Fixed to script type dependency hash generation. The issues could cause unnecessary imports and in some cases missing reimports. (1295635)
    
*   Asset Pipeline: Fixed various issues relating to assets not being correctly unloaded during AssetDatabase.Refresh(). ([1186177](https://issuetracker.unity3d.com/issues/animations-are-not-playing-when-loading-scene-after-upgrading-from-unity-2019-dot-3-0b3-or-above-to-a-newer-version), [1213291](https://issuetracker.unity3d.com/issues/override-controllers-are-missing-their-state-to-clip-mapping-when-imported-via-a-custom-package), [1255803](https://issuetracker.unity3d.com/issues/references-to-animation-clips-in-blend-trees-disappear-when-a-new-animation-clip-is-added-and-the-model-is-reimported), [1299716](https://issuetracker.unity3d.com/issues/scriptableobject-has-null-reference-to-prefabs-component-when-there-is-a-reference-inside-the-scriptableobject))
    
*   Asset Pipeline: Improved performance of flushing the preload operation queue from the main thread. This can occur when accessing an operation's result on the main thread before it is completed.
    
*   Asset Pipeline: InitializeOnLoad method shouldn't be used for asset operations, because InitializeOnLoad is called before asset importing is completed. ([1279619](https://issuetracker.unity3d.com/issues/assetdatabase-dot-findassets-folder-not-found-assets-is-thrown-on-searching-from-initializeonload))
    
*   Asset Pipeline: New version of OnPostProcessAllAssets with didDomainReload parameter added. This callback should be used for domain reload related initialization that requires asset operations such as asset loading. InitializeOnLoad method shouldn't be used for asset operations, because InitializeOnLoad is called before asset importing is completed. ([1274994](https://issuetracker.unity3d.com/issues/calling-loadassetatpath-during-domainreload-returns-null-asset-if-asset-is-in-modification-list-as-well-as-a-script))
    
*   Asset Pipeline: PostProcessAllAssets callback now supports all asset db operations. ([1144276](https://issuetracker.unity3d.com/issues/prefabutility-dot-saveasprefabasset-returns-null-when-creating-new-prefab-on-assetpostprocessor-dot-onpostprocessallassets))
    
*   Asset Pipeline: Preview of material is now correctly regenerated when shader changes ([1298200](https://issuetracker.unity3d.com/issues/prefabs-thumbnail-isnt-updated-when-the-shader-is-modified))
    
*   Asset Pipeline: Previews are now correct for a prefeab when assets referenced by the prefab (like texture) changes ([1284853](https://issuetracker.unity3d.com/issues/color-of-the-prefab-preview-icon-is-not-updated-when-color-of-the-material-is-changed-and-prefab-is-reimported))
    
*   Asset Pipeline: Updated reload tests to cover async domain reload.
    
*   Asset Pipeline: Using the AssetDatabase.CreateAsset() API to create an asset from a TextAsset object where the file type specified is not a native Unity format such as .ASSET will now report an error about incorrect usage of CreateAsset. ([1241343](https://issuetracker.unity3d.com/issues/assetdatabase-dot-createasset-generates-uneccessary-content-into-a-text-file-when-creating-a-textasset))
    
*   Audio: (OSX) Sound effects in Audio Mixer were not always selected when clicked. ([1124032](https://issuetracker.unity3d.com/issues/mac-sound-effects-in-audio-mixer-arent-always-selected-when-clicked))
    
*   Audio: AudioClip reference was lost when loading a new Scene even if AudioSource was set to DontDestroyOnLoad. ([1314527](https://issuetracker.unity3d.com/issues/audioclip-reference-is-lost-when-loading-a-new-scene-even-if-audiosource-is-set-to-dontdestroyonload))
    
*   Audio: Fixed AudioClip reference being lost when loading a new Scene even if AudioSource is set to DontDestroyOnLoad.
    
*   Audio: Fixed deadlock caused by interaction between output suspend/resume logic and DSPGraph output hooks.
    
*   Audio: Fixed DSPGraph playback not pausing when player is paused.
    
*   Audio: Fixed editor crash when undoing after reordering snapshots in the audio mixer.  
    Fixed exception when deleting snapshots. ([1324578](https://issuetracker.unity3d.com/issues/editor-crashes-when-reordering-audio-mixer-snapshots-and-undoing))
    
*   Audio: Fixed microphone API not working when automatic output device suspension was active. (1318560)
    
*   Audio: SoundManager optimizations for lowering main thread performance degradations caused by having a large amount of loaded audio clips in a scene. (1146312)
    
*   Audio: Topological changes such as adding/removing/moving effects in the audio mixer resulted in glitches and, depending on mixer configuration, loud bursts. ([666910](https://issuetracker.unity3d.com/issues/effects-leak-when-renaming-an-exposed-parameter))
    
*   Bug Reporter: Fixed a bug where the crash reporting symbol uploader process would crash on parsing certain dSYM files.
    
*   Bug Reporter: Improved failing filename error message to make it reflect the source of the problem better. ([1298484](https://issuetracker.unity3d.com/issues/mac-bug-reporter-fails-to-archive-the-project-when-there-are-special-characters-in-a-folder-name))
    
*   Bug Reporter: Multiple Qt library copies are no longer included.
    
*   Bug Reporter: Reset Bug Reporter style to match Windows styling ([1296042](https://issuetracker.unity3d.com/issues/bug-reporter-unity-bug-reporter-window-doesnt-follow-unity-design-guidelines))
    
*   Build Pipeline: Added an API to gather the lighting and fog modes used by the active scene. (1293228)
    
*   Build Pipeline: Added build target Dedicated Server.
    
*   Build Pipeline: Errors from catastrophically failing incremental build pipeline steps are now clearer.
    
*   Build Pipeline: Fixed a bug where data builds would unnecessarily rerun in incremental player builds if the project contained editor resources.
    
*   Build Pipeline: Fixed a bug where UnityLinker would unnecessarily rerun without changes in incremental player builds.
    
*   Build Pipeline: Fixed a potential file name issue on windows in incremental player builds.
    
*   Build System: Fixed a problem with the detection of Microsoft.VCLibs SDK extension for UWP builds.
    
*   Burst: Added PreserveAttribute to prevent the internal log from being stripped in il2cpp builds.
    
*   Burst: Added PreserveAttribute to prevent the internal log from being stripped in il2cpp builds.
    
*   Burst: Broken link restored for known issues with debugging and profiling.
    
*   Burst: Broken link restored for known issues with debugging and profiling.
    
*   Burst: clang segmentation fault on iOS when member function debug information was emitted, it is disabled for this platform now.
    
*   Burst: Clang segmentation fault on iOS when member function debug information was emitted, it is disabled for this platform now.
    
*   Burst: Corrected 'Enable safety checks tooltip\`.
    
*   Burst: Corrected 'Enable safety checks tooltip\`.
    
*   Burst: Crash when extracting sequence point information for error reporting/debug information generation.
    
*   Burst: Direct Call extension methods that only differ on argument types are now supported (previously Burst's `AssemblyLoader` would complain about multiple matches).
    
*   Burst: Dots runtime function pointer transform has been simplified, making it less brittle and fixing some bad IL generation.
    
*   Burst: Dots runtime function pointer transform has been simplified, making it less brittle and fixing some bad IL generation.
    
*   Burst: Fixed a bug in LLVM that it would incorrectly convert some memset ->; memcpy if both pointers derived from the same memory address, and where one indexed into the 0th element of the pointer.
    
*   Burst: Fixed a bug that occurred when an explicitly laid out struct was used by a dup instruction, which caused an internal compiler error.
    
*   Burst: Fixed a bug that occurred when an explicitly laid out struct was used by a `dup` instruction, which caused an internal compiler error.
    
*   Burst: Fixed a bug where eager-compilation could pick up out-of-date global Burst menu options for compiling.
    
*   Burst: Fixed a bug where eager-compilation could pick up out-of-date global Burst menu options for compiling.
    
*   Burst: Fixed a bug where explicitly casting from an int to IntPtr would not sign extend the value.
    
*   Burst: Fixed a bug where explicitly casting from an int to `IntPtr` would not sign extend the value.
    
*   Burst: Fixed a bug where having any \[DllImport\] in a class that used the Direct Call mechanism could result in an illegal CompileFunctionPointer call being produced by our post processor.
    
*   Burst: Fixed a bug where having any `[DllImport]` in a class that used the Direct Call mechanism could result in an illegal `CompileFunctionPointer` call being produced by our post processor.
    
*   Burst: Fixed a bug where if a user had defined multiple implicit or explicit casts, the compiler could resolve to the wrong cast.
    
*   Burst: Fixed a bug where if a user had defined multiple implicit or explicit casts, the compiler could resolve to the wrong cast.
    
*   Burst: Fixed a bug where loading from a vector within a struct, that was got from a NativeArray using an indexer, would cause the compiler to crash.
    
*   Burst: Fixed a bug where loading from a vector within a struct, that was got from a `NativeArray` using an indexer, would cause the compiler to crash.
    
*   Burst: Fixed a bug where the Burst post-processing for direct call would cause duplicate function pointers to be compiled, wasting compile time in the editor and caused an Editor launch stall.
    
*   Burst: Fixed a bug where the Burst post-processing for direct call would cause duplicate function pointers to be compiled, wasting compile time in the editor and caused an Editor launch stall.
    
*   Burst: Fixed a bug where the multi-CPU dispatcher (used for player builds targetting multiple CPU architectures) could end up generating invalid instructions.
    
*   Burst: Fixed a bug where the progress bar would report double the amount of pending compile jobs if a user changed the Burst options while background compilation was going on.
    
*   Burst: Fixed a bug where the progress bar would report double the amount of pending compile jobs if a user changed the Burst options while background compilation was going on.
    
*   Burst: Fixed a bug whereby sometimes some LLVM intrinsics could be incorrectly marked as unused causing invalid codegen with calls to math.acos.
    
*   Burst: Fixed a bug with using multiple `IsXXXSupported` intrinsics in the same boolean condition would fail.
    
*   Burst: Fixed a minor debug information bug where built-in types with methods (like `System.Int32`) would generate incorrect debug information.
    
*   Burst: Fixed a possible DivideByZeroException due to race condition in TermInfoDriver initialization code.
    
*   Burst: Fixed a regression where managed static fields, in static constructors that would also be compiled with Burst, could cause a compile time failure for mixing managed and unmanaged state.
    
*   Burst: Fixed a very obscure bug where if you had a function-pointer that was called from another function-pointer of job, and that function-pointer happened to be compiled in a player build in the same bucket as the caller, and the no-alias cloning analysis identified that it could clone the original function-pointer to enable more aliasing optimizations, it could create a duplicate symbol error.
    
*   Burst: Fixed a very obscure bug where if you had a function-pointer that was called from another function-pointer of job, and that function-pointer happened to be compiled in a player build in the same bucket as the caller, and the no-alias cloning analysis identified that it could clone the original function-pointer to enable more aliasing optimizations, it could create a duplicate symbol error.
    
*   Burst: Fixed alignment issues associated with xxHash3 on ArmV7 (case 1288992)
    
*   Burst: Fixed alignment issues associated with xxHash3 on ArmV7 (case 1288992).
    
*   Burst: Fixed an issue where Burst would erroneously error on BurstCompile.CompileFunctionPointer calls when building for the DOTS Runtime.
    
*   Burst: Fixed an issue where Burst would erroneously error on `BurstCompile.CompileFunctionPointer` calls when building for the DOTS Runtime.
    
*   Burst: Fixed an issue where if a user used a math function (like `cos`, `sin`, etc) then LLVM would preserve both the scalar and vector implementations even if they were trivially dead, causing us to inject otherwise dead functions into the resulting binary.
    
*   Burst: Fixed Burst's handling of stack-recovery, in the editor, on Apple Silicon hardware. (1345235)
    
*   Burst: Fixed compilation errors when targeting Arm CPUs and using some of the Intel intrinsics
    
*   Burst: Fixed compilation errors when targeting Arm CPUs and using some of the Intel intrinsics.
    
*   Burst: Fixed compilation errors when targeting Intel CPUs and using some of the Arm Neon intrinsics
    
*   Burst: Fixed compilation errors when targeting Intel CPUs and using some of the Arm Neon intrinsics.
    
*   Burst: Fixed crashes on 32 bit windows when calling function pointers from managed code and using IL2CPP.
    
*   Burst: Fixed crashes on 32 bit windows when calling function pointers from managed code and using IL2CPP.
    
*   Burst: Fixed DOTS Runtime JobProducer Bursting code to support JobProducers with multiple generic arguments, complex job wrapper and generic jobs.
    
*   Burst: Fixed managed implementation of sub\_ss intrinsic
    
*   Burst: Fixed managed implementation of sub\_ss intrinsic.
    
*   Burst: Fixed managed implementations of blend\_epi32 and mm256\_blend\_epi32 intrinsics on Mono
    
*   Burst: Fixed managed implementations of blend\_epi32 and mm256\_blend\_epi32 intrinsics on Mono.
    
*   Burst: Fixed multi-CPU dispatcher (used for player builds targetting multiple CPU architectures) generating invalid instructions.
    
*   Burst: Fixed namespace issue triggering a warning in the editor.
    
*   Burst: Fixed some intrinsics not checking target CPU against required CPU, so it was possible to use some intrinsics without an IsXXXSupported check.
    
*   Burst: Fixed some intrinsics not checking target CPU against required CPU, so it was possible to use some intrinsics without an IsXXXSupported check.
    
*   Burst: Fixed the 1.5 restriction that Direct Call methods can only be called from the main thread, now they work when called from any thread.
    
*   Burst: Fixes DOTS Runtime JobProducer Bursting code to support JobProducers with multiple generic arguments, complex job wrapper and generic jobs.
    
*   Burst: Function calls using in modifiers on blittable structs where being treated as non blittable.
    
*   Burst: Gracefully handle failing to find a particular assembly in the ILPP to prevent an ICE.
    
*   Burst: IL Function Pointer Invoke Transformation now uses correct runtime library for dots runtime.
    
*   Burst: IL Function Pointer Invoke Transformation now uses correct runtime library for dots runtime.
    
*   Burst: IL Function Pointer Invoke Transformation updated to handle transforms that affect instructions that are the destination of a branch.
    
*   Burst: IL Function Pointer Invoke Transformation updated to handle transforms that affect instructions that are the destination of a branch.
    
*   Burst: Internal Compiler Error if a call was discarded (via BurstDiscard for example), but the callsites required an ABI transform e.g. struct return.
    
*   Burst: Internal Compiler Error if a call was discarded (via BurstDiscard for example), but the callsites required an ABI transform e.g. struct return.
    
*   Burst: Intrinsics: Neon - fixed vget\_low and vget\_high producing suboptimal code
    
*   Burst: Intrinsics: Neon - fixed vget\_low and vget\_high producing suboptimal code.
    
*   Burst: Made `math.shuffle` compile correctly when non-constant `ShuffleComponent`'s are used.
    
*   Burst: Multiple bugfixes (please look at https://docs.unity3d.com/Packages/com.unity.burst@1.5/changelog/CHANGELOG.html for a detailed list).
    
*   Burst: PDB debug information for instance methods that also used struct return were incorrect.
    
*   Burst: PDB debug information for instance methods that also used struct return were incorrect.
    
*   Burst: Private \[BurstCompile\] methods no longer throw MethodAccessException
    
*   Burst: Private `[BurstCompile]` methods no longer throw `MethodAccessException`.
    
*   Burst: Revert to internal linkage for Android X86 (32bit) to ensure ABI compliance.
    
*   Burst: String interpolation issues when using Dots / Tiny runtime.
    
*   Burst: String interpolation issues when using Dots / Tiny runtime.
    
*   Burst: Strings can now be passed between methods.
    
*   Burst: The Direct Call injected delegate now has a unique suffix to avoid type-name clashes.
    
*   Burst: When generating Line Table only debug information, an unreachable could occur due to a missing check.
    
*   Burst: When generating Line Table only debug information, an unreachable could occur due to a missing check.
    
*   Core: Fixed bug where shadows disappear in the frustum corners from false positives in the shadow culling. ([1153151](https://issuetracker.unity3d.com/issues/lwrp-shadows-are-being-culled-incorrectly-in-the-corner-of-the-camera-viewport-when-the-far-clip-plane-is-small))
    
*   Core: Fixed bug with shadow fade where the shadows will be culled with a hard line across the fade and also stretches the fade beyond the projected shadow.
    
*   Core: Fixed issue where Profiler/Memory Profiler cannot be connected to Standalone build when Run in Background is disabled. ([1355728](https://issuetracker.unity3d.com/issues/profiler-slash-memory-profiler-cannot-be-connected-to-standalone-build-when-run-in-background-is-disabled))
    
*   Documentation: Changed the documentation for HorizontalLayout and VerticalLayout. ([1260855](https://issuetracker.unity3d.com/issues/verticallayoutgroup-children-position-is-not-updated-when-a-childs-scale-is-animated))
    
*   Documentation: Fixed html bug in TestRunnerApi API code snippet (DS-1973).  
    Fix typo bug in PreBuildSetup code example (DS-1974).  
    Fix incorrect syntax in command line reference (DS-1971).
    
*   Documentation: Fixed incorrect documentation for SaveCurrentModifiedScenesIfUserWantsTo. ([1170364](https://issuetracker.unity3d.com/issues/editorscenemanager-dot-savecurrentmodifiedscenesifuserwantsto-returns-true-when-dont-save-is-selected))
    
*   Documentation: Fixed missing function signatures from RayTracingAccelerationStructure.AddInstance C# API in 2021.2 documentation.
    
*   DX12: DX12 Standalone Player crashes at startup when using 32-bit player support. (1315964)
    
*   DX12: Fix int shader uniforms in .raytrace shaders being displayed as Floats in the Frame Debugger. ([1305552](https://issuetracker.unity3d.com/issues/dxr-integer-values-set-using-raytracingshader-dot-setint-are-displayed-as-floats-in-frame-debugger))
    
*   DX12: Fixed flickering issue on mesh particles. (1357667)
    
*   DX12: Fixed wrong error message saying that vertex format SNorm16 is not supported when building a Ray Tracing Acceleration Structure. The format is supported.
    
*   DX12: Significant performance cost of using SRP batcher on DX12 reduced. (1286694)
    
*   Editor: (Dynamic Hints) Fixed: NullReferenceException when a prefab with a missing script is hovered in the ProjectBrowser
    
*   Editor: A warning is now displayed when modifying the enable analytics preference, informing the user that it will require a restart of the editor. (1307652)
    
*   Editor: Added API Updater rule to update global API AssetModificationProcessor to UnityEditor namespace ([1064480](https://issuetracker.unity3d.com/issues/deprecated-unityengine-dot-assetmodificationprocessor-should-be-removed))
    
*   Editor: Added new functionality to decouple the PlayerLoop() when the targetFrameRate is set to a finite value, so that it does not effect/slow down the other Editor windows. ([1158168](https://issuetracker.unity3d.com/issues/application-dot-targetframerate-affects-the-speed-of-other-windows-in-editor-when-changing-frame-rates))
    
*   Editor: Added playerGraphicsAPI TestSettings parameter.
    
*   Editor: Added support for dragging across delayed UI fields to change variables. ([1263630](https://issuetracker.unity3d.com/issues/terrain-input-value-for-all-the-properties-not-changing-when-a-mouse-is-dragged-over-it-under-mesh-resolution))
    
*   Editor: Added tooltips in the Scene template Inspector. ([1324637](https://issuetracker.unity3d.com/issues/editor-tooltips-are-not-displayed-when-hovering-over-scene-template-properties))
    
*   Editor: Allow hierarchy search to find scripts which share names of internal types. ([1252479](https://issuetracker.unity3d.com/issues/searching-in-the-hierarchy-window-does-not-yield-any-results-when-the-components-name-is-used-internally-eg-audiomanager))
    
*   Editor: Allow multiple Unity versions to display in the "Open With..." menu and dialog. Allow the user to choose one as the default. ([1202338](https://issuetracker.unity3d.com/issues/exported-package-file-becomes-not-recognized-and-without-icon-when-installing-and-uninstalling-unity-versions-via-hub))
    
*   Editor: Close add ratio window after selecting from aspect ratio menu. ([1284690](https://issuetracker.unity3d.com/issues/game-view-aspect-ratio-window-doesnt-get-closed-when-the-aspect-ratio-selected))
    
*   Editor: ColorUsageAttribute is now respected when the inspector window is in debug mode. ([1312714](https://issuetracker.unity3d.com/issues/hdr-true-in-the-colorusageattribute-is-not-respected-when-the-inspector-is-in-the-debug-mode))
    
*   Editor: Create default index when opening the index manager if it was never created before.
    
*   Editor: Custom editors that live in a Unity package will now be used only is a user defined custom editor is not found. ([1300193](https://issuetracker.unity3d.com/issues/unityengine-dot-ui-dot-image-component-editor-cannot-be-overriden-by-custom-editor))
    
*   Editor: Default PropertyDrawer.OnGUI no longer renders multiple overlapping labels. (1335958)
    
*   Editor: Deleting search query from project browser won't break the search window (1336787)
    
*   Editor: Display the menu item name when its execution time is longer than the user wait threshold (i.e. 3 seconds) (1313062)
    
*   Editor: Displayed a warning when the min and max values are equal for the Slider. ([1328583](https://issuetracker.unity3d.com/issues/ui-minmaxslider-disappears-when-enable-slash-disable-whole-numbers-checkbox-for-ui-slider))
    
*   Editor: enable tabbing in the editor while modifier keys are pressed excluding command, control, and alt ([1299846](https://issuetracker.unity3d.com/issues/macos-tab-key-with-caps-lock-enabled-doesnt-navigate-to-next-field))
    
*   Editor: Ensure invalid Sketchup model UVs are initialized to zero.
    
*   Editor: Event.current.type scrollWheel pointerType value is now registered as PointerType.Mouse in the mac editor ([1261326](https://issuetracker.unity3d.com/issues/macos-event-dot-current-dot-type-scrollwheel-pointertype-value-is-not-registered-as-pointertype-dot-mouse-when-the-editor-is-focused))
    
*   Editor: Favorite star is always visible for favorited items (1336789)
    
*   Editor: Fix arrow key functionality in dialogs in the Mac Editor. ([1279832](https://issuetracker.unity3d.com/issues/macos-text-caret-position-cannot-be-moved-via-arrow-keys-in-the-build-project-pop-up-window))
    
*   Editor: Fix for detecting and warning the user on imbalanced GUI layout groups ([1289223](https://issuetracker.unity3d.com/issues/guilayout-dot-beginhorizontal-or-beginvertical-does-not-warn-for-imbalances))
    
*   Editor: Fix for layer names being clipped in Culling Mask and Volume Mask dropdowns of a HDRP project ([1307655](https://issuetracker.unity3d.com/issues/hdrp-graphics-compositor-texts-are-clipped-in-culling-mask-and-volume-mask-properties-dropdown-options))
    
*   Editor: Fix popup windows in the Linux Editor to show on the right-hand monitor if requested from the right-hand monitor ([1294722](https://issuetracker.unity3d.com/issues/linux-context-menu-opens-on-the-first-connected-monitor-when-the-editor-window-is-located-on-the-second-one))
    
*   Editor: Fix styling of selected search query if hovering (1336784)
    
*   Editor: Fixed "Cannot get non-existing progress id" error appearing in the Console when entering Play mode. ([1312446](https://issuetracker.unity3d.com/issues/cannot-get-non-existing-progress-id-error-appears-in-console-when-entering-the-play-mode))
    
*   Editor: Fixed a bug where test filter would match project or player path (DSTP-412).
    
*   Editor: Fixed a crash that occurred when using the Memory Profiler to capture memory use for very large scenes. (1316870)
    
*   Editor: Fixed a memory leak while using SerializedObjects in the AssetImporter inspectors. (1232758)
    
*   Editor: Fixed a regression in where users could no longer assign a Render Texture to the light cookie widget in the UI. ([1355504](https://issuetracker.unity3d.com/issues/render-texture-cannot-be-assigned-as-a-cookie-of-lights-when-assigning-through-the-inspector))
    
*   Editor: Fixed add an extra null check for monitor enumeration. (1320164)
    
*   Editor: Fixed an edge case where removing and re-adding a sub asset would cause the local file id of the object to change unnecessarily. ([1323357](https://issuetracker.unity3d.com/issues/subasset-ordering-changes-in-version-control-when-removing-and-re-adding-all-subassets))
    
*   Editor: Fixed an error is thrown after re-building a library of previous Editor version project when the Profiler of 2020.2 project is opened. ([1273439](https://issuetracker.unity3d.com/issues/an-error-is-thrown-after-re-building-a-library-of-previous-editor-version-project-when-the-profiler-of-2020-dot-2-project-is-opened))
    
*   Editor: Fixed an issue in macOS where popup buttons would show their popup far from the button if the button was near the bottom of the screen. ([1323332](https://issuetracker.unity3d.com/issues/macos-native-dropdown-menu-shifts-upwards-when-dropdown-that-is-clicked-is-close-to-the-bottom-of-the-screen))
    
*   Editor: Fixed an issue to avoid difference in Width and Height for EditorGUI.RectIntField fields compared to other fields in the Transform section. ([1297283](https://issuetracker.unity3d.com/issues/editorgui-dot-rectintfield-generated-fields-are-incorrect-width-and-height))
    
*   Editor: Fixed an issue to avoid MinMaxSlider disappears for UI Slider. ([1323384](https://issuetracker.unity3d.com/issues/ui-minmaxslider-disappears-when-min-and-max-have-the-same-values-for-ui-slider))
    
*   Editor: Fixed an issue to avoid typing or pasting unlimited characters in Project and Console search fields. ([1331001](https://issuetracker.unity3d.com/issues/project-and-console-window-search-bars-have-no-text-length-limits-and-might-freeze-when-pasting-a-large-number-of-symbols))
    
*   Editor: Fixed an issue to avoid warning log when selected sub-asset with an empty name. ([1333540](https://issuetracker.unity3d.com/issues/a-gameobject-name-cannot-be-set-to-an-empty-string-warning-is-logged-when-sub-asset-has-an-empty-name))
    
*   Editor: Fixed an issue to display checkmark next to "Everything" in drop-down for "Culling Mask" property value ([1299181](https://issuetracker.unity3d.com/issues/layermask-properties-showing-mixed-dot-dot-dot-selection-when-all-flags-are-selected-instead-of-everything))
    
*   Editor: Fixed an issue to display Color32 Picker Context Menu at right position on right click. ([1334328](https://issuetracker.unity3d.com/issues/color32-picker-context-menu-will-always-display-in-the-left-corner-regardless-of-where-the-mouse-click-is-positioned))
    
*   Editor: Fixed an issue to display Normalmap Encoding PlayerSetting only in supported platforms. (1330505)
    
*   Editor: Fixed an issue to display proper LayerMask properties value on selection. ([1308984](https://issuetracker.unity3d.com/issues/layermask-properties-showing-mixed-dot-dot-dot-selection-when-no-flags-are-selected-instead-of-nothing))
    
*   Editor: Fixed an issue to display Rect Transform Anchors in Scene View, with multiple Inspector windows open and when firstly opened one has been locked. ([1221384](https://issuetracker.unity3d.com/issues/rect-transform-anchors-invisible-in-scene-view-with-multiple-inspector-windows-open-when-firstly-opened-one-has-been-locked))
    
*   Editor: Fixed an issue to display tooltip for "Maximum LOD Level" and "LOD Bias" Properties under Quality settings. ([1296474](https://issuetracker.unity3d.com/issues/imgui-maximum-lod-level-and-lod-bias-properties-tooltip-missing-under-quality-in-the-project-setting-window))
    
*   Editor: Fixed an issue to enable cut and copy in context when Array Size field is selected. ([1290634](https://issuetracker.unity3d.com/issues/copying-array-size-field-is-blocked-via-the-context-menu-until-a-different-field-is-copied-first))
    
*   Editor: Fixed an issue to set top bit flag of an uint enum with inspector. (1298289)
    
*   Editor: Fixed an issue to stop clearing Asset's name property when resetting it via the Inspector.
    
*   Editor: Fixed an issue to stop sharing Player Settings properties between Player Settings window and Serialized Preset. ([1263069](https://issuetracker.unity3d.com/issues/platform-selection-is-shared-between-player-settings-window-and-serialized-preset))
    
*   Editor: Fixed an issue where an empty column is expanded when detaching/attaching UISystemPreviewWindow in the Profiler. ([1241234](https://issuetracker.unity3d.com/issues/detaching-and-reattaching-unityeditor-dot-uisystempreviewwindow-from-profiler-window-expands-empty-column))
    
*   Editor: Fixed an issue where calling EditorGUI.PropertyField with a serialized LayerMask and GUIContent.none prints a label. (1304172)
    
*   Editor: Fixed an issue where check box is shown on Inspector Titlebar for ScriptableObjects ([1301335](https://issuetracker.unity3d.com/issues/the-enable-checkbox-is-displayed-when-using-editorguilayout-dot-inspectortitlebar-and-the-scriptableobject-has-an-onenable-method))
    
*   Editor: Fixed an issue where Default Text preset is not applied when creating a new Text object. ([1328458](https://issuetracker.unity3d.com/issues/text-default-text-preset-is-not-applied-when-creating-a-new-text-object))
    
*   Editor: Fixed an issue where null reference exceptions can be thrown when opening a URP project. ([1310784](https://issuetracker.unity3d.com/issues/nullreferenceexception-errors-are-thrown-when-opening-the-project-until-anything-is-selected-in-the-project-window-hierarchy))
    
*   Editor: Fixed an issue where out argument out of range exceptions are thrown when deleting Japanese characters in the input field. ([1201105](https://issuetracker.unity3d.com/issues/error-is-thrown-when-deleting-japanese-characters-in-tmp-inputfield))
    
*   Editor: Fixed an issue where Shift-Delete does not delete the property for Object field. ([1286390](https://issuetracker.unity3d.com/issues/custom-scriptable-objects-prefab-property-doesnt-get-deleted-when-pressing-ctrl-plus-del))
    
*   Editor: Fixed an issue where the Assembly definition asset does not save after an apply action on import setting pop up. ([1309567](https://issuetracker.unity3d.com/issues/changes-to-assembly-definition-asset-are-not-saved-after-pressing-the-apply-button-in-the-unapplied-import-settings-pop-up))
    
*   Editor: Fixed an issue where the mouse cursor over the text field's cancel button is displayed as text instead of arrow and the cursor flickers when mouse is hovered over the cancel button. (1314173, 1314177)
    
*   Editor: Fixed an issue where warning appears when Scrollbar Navigation is set to Vertical and Direction is set to "Top To Bottom" ([1245473](https://issuetracker.unity3d.com/issues/warning-appears-when-scrollbar-navigation-is-set-to-vertical-and-direction-is-set-to-top-to-bottom))
    
*   Editor: Fixed an issue where warnings are thrown in the console when the layout is set to default while in play mode. ([1317240](https://issuetracker.unity3d.com/issues/missing-referenced-script-warnings-are-thrown-when-resetting-the-editor-layout-to-default-while-in-play-mode))
    
*   Editor: Fixed an issue where Window title tooltip does not disappear after closing Editor window. ([1283915](https://issuetracker.unity3d.com/issues/hdrp-compositor-graphics-compositor-tooltip-does-not-disappear-after-closing-compositor-window))
    
*   Editor: Fixed and issue with toolbar dropdown buttons while resizing editor window on OSX. ([1299763](https://issuetracker.unity3d.com/issues/imgui-account-layer-and-layout-buttons-are-not-selectable-while-resizing-the-editor))
    
*   Editor: Fixed ArgumentNullException when selecting 'Static-dropdown' in the Prefab Overrides window. ([1295412](https://issuetracker.unity3d.com/issues/improved-prefabs-argumentnullexception-errors-are-thrown-on-selecting-static-dropdown-in-overrides-window))
    
*   Editor: Fixed assets not getting moved when there's a folder of the same name in the selection. ([1318098](https://issuetracker.unity3d.com/issues/only-one-asset-gets-moved-when-trying-to-move-multiple-assets-with-the-same-name-to-a-different-directory-in-the-project-window))
    
*   Editor: Fixed broken normal map previews (1339051)
    
*   Editor: Fixed color picker keeps updating color preview when the EyeDropper is used and Esc key is pressed. ([1291991](https://issuetracker.unity3d.com/issues/vfxgraph-add-color-node-color-preview-continues-showing-the-color-selection-when-the-esc-key-was-pressed))
    
*   Editor: Fixed console window fails to repaint unless hovered over if it had been maximized before. ([1300081](https://issuetracker.unity3d.com/issues/windows-console-window-fails-to-repaint-unless-hovered-over-if-it-had-been-maximized-before))
    
*   Editor: Fixed crash when adding a component to an object fails and prompts a modal dialog. (1348654)
    
*   Editor: Fixed Ctrl-click on macOS editor not bringing up "Properties..." context menu on inspector object reference fields properly. ([1316779](https://issuetracker.unity3d.com/issues/macos-ctrl-plus-click-does-not-open-context-menu-in-the-inspector))
    
*   Editor: Fixed cursor flickering from double arrow to single arrow over splitter on Mac and Windows. ([1295344](https://issuetracker.unity3d.com/issues/splitter-resize-cursors-flicker-on-linux-and-windows))
    
*   Editor: Fixed cursor hide in Linux playmode. (1350956)
    
*   Editor: Fixed cursor locking on Windows when the cursor is on a non-primary display. ([1282412](https://issuetracker.unity3d.com/issues/cursor-dot-lockstate-locking-out-of-the-screen-when-using-two-monitors-with-different-scales))
    
*   Editor: Fixed debug assert message in MenuControllerLinux.cpp's OnSizeAllocate() call to GetGtkWindowSize(). (1319050)
    
*   Editor: Fixed dragging horizontally along the last sibling in the Hierachy and other TreeViews to specify an alternative parent and sibling for the dragged items. (1294910)
    
*   Editor: Fixed empty reason on passed tests results xml (DSTR-63).
    
*   Editor: Fixed error is thrown on performing undo operation on a gameobject after adding 'New Script' component. ([1312440](https://issuetracker.unity3d.com/issues/undo-inspector-framework-error-is-thrown-on-performing-undo-operation-on-a-gameobject-after-adding-new-script-component))
    
*   Editor: Fixed failure to load window layout when Editor tries to create new asset from SettingsProvider callback at startup. ([1322299](https://issuetracker.unity3d.com/issues/failed-to-load-window-layout-when-editor-tries-to-create-new-asset-from-settingsprovider-callback-at-startup))
    
*   Editor: Fixed File->;Open Recent Scene menu entries not working correctly after upgrading project from versions earlier than 2021.2.0a5. ([1338322](https://issuetracker.unity3d.com/issues/recent-scenes-break-after-upgrading-project))
    
*   Editor: Fixed floating windowing jumping desktop spaces when using cmd + tab to refocus the editor on mac. ([1298279](https://issuetracker.unity3d.com/issues/macos-switching-to-unity-when-it-is-in-another-desktop-moves-the-last-selected-window-to-the-current-desktop))
    
*   Editor: Fixed for Canvas Group Interactable flag being applied to the GameObject even when the Canvas Group component is disabled. ([1324097](https://issuetracker.unity3d.com/issues/canvas-group-interactable-flag-is-applied-to-the-gameobject-when-the-canvas-group-component-is-disabled))
    
*   Editor: Fixed gameview not responding to some input when the mouse is over another window in the macOS editor. ([1358134](https://issuetracker.unity3d.com/issues/input-dot-getkey-does-not-trigger-when-the-mouse-cursor-is-outside-the-game-window))
    
*   Editor: Fixed gradient swatches were not refreshed after undoing preset change. (1261595)
    
*   Editor: Fixed GUIToScreenpoint being inconsistent between play mode and standalone. ([1305557](https://issuetracker.unity3d.com/issues/guitoscreenpoint-returns-physical-screen-coordinates-when-in-guigroup))
    
*   Editor: Fixed hierarchy window top Scene header foldout not visible when scrolled. (1298679)
    
*   Editor: Fixed incorrect bounds when LineRenderer GameObject was not enabled and point editing mode was activated. (1288693)
    
*   Editor: Fixed infinite layout error loop when Editor UI is broken. (1327876)
    
*   Editor: Fixed instancing being ignored in the Shadow Pass when using the Mobile Diffuse shader. (1318675)
    
*   Editor: Fixed issue when `.` suffix was applied to BuildTargets without extension.
    
*   Editor: Fixed issue where the Intensity parameter of a Default Light Preset is not applied after creating Directional Light Game object. ([1199933](https://issuetracker.unity3d.com/issues/preset-intensity-parameter-of-a-default-light-preset-is-not-applied-after-creating-directional-light-game-object))
    
*   Editor: Fixed issue with CRTL Drag not working when a single item is selected in project browser one-column layout. ([1222445](https://issuetracker.unity3d.com/issues/dragging-asset-with-ctrl-to-duplicate-it-only-deselects-asset-when-it-has-already-been-selected-in-one-column-layout))
    
*   Editor: Fixed issue with Reference Icon overlapping with Preset Manager text on decreasing the width of the Project Settings window. ([1282739](https://issuetracker.unity3d.com/issues/imgui-reference-icon-overlapped-with-preset-manager-text-on-decreasing-the-width-of-the-project-settings-window))
    
*   Editor: Fixed issue with Stack trace input Field being Misaligned on resizing Player setting Preset. ([1276715](https://issuetracker.unity3d.com/issues/imgui-stack-trace-input-field-is-misaligned-on-resizing-player-setting-preset))
    
*   Editor: Fixed jumping scroll-bar when working with arrays. ([1362327](https://issuetracker.unity3d.com/issues/scrolling-is-jumping-when-scrolling-in-the-input-manager))
    
*   Editor: Fixed keycode for new input system on Linux to reflect hardware keycode/physical key location. (1343619)
    
*   Editor: Fixed missing comma in the manifest file used by the guardian tool.
    
*   Editor: Fixed NullReferenceException error is thrown when pressing up/down arrow key in the Project's search bar while in Play Mode. ([1318065](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-pressing-up-slash-down-arrow-key-in-the-projects-search-bar-while-in-play-mode))
    
*   Editor: Fixed NullReferenceException when trying to open Object Picker for ScriptableObject variable. ([1293117](https://issuetracker.unity3d.com/issues/nullreferenceexception-when-trying-to-open-object-picker-for-scriptableobject-variable))
    
*   Editor: Fixed Profile Analyzer - Mac keyboard commands not updating correct chart. (1327944)
    
*   Editor: Fixed ReorderableList having wrong label/field width ratio.
    
*   Editor: Fixed Repeat and Retry attribute for UnityTest in PlayMode (DSTR-237).
    
*   Editor: Fixed Scene's Hierarchy visibility and pickability settings being reset after building. ([1271518](https://issuetracker.unity3d.com/issues/scenes-hierarchy-visibility-and-pickability-settings-are-reset-after-building))
    
*   Editor: Fixed selection issues with Shift + Arrow Up/Down in the Hierarchy. ([1320614](https://issuetracker.unity3d.com/issues/selecting-elements-with-shift-plus-up-slash-down-arrow-is-broken-in-hierarchy-window))
    
*   Editor: Fixed settings move erratically when the setting you are looking for is located in another platform's tab. ([1293497](https://issuetracker.unity3d.com/issues/settings-are-jumping-around-when-the-setting-you-are-looking-for-is-located-in-another-platforms-settings))
    
*   Editor: Fixed slow enter playmode time for a specific scene file that contained sequential File ID Hint values. ([1308128](https://issuetracker.unity3d.com/issues/entering-play-mode-takes-upwards-of-1-hour-when-auto-generating-high-amounts-of-objects))
    
*   Editor: Fixed so that undocked windows can exit full screen/unmaximize. ([1293516](https://issuetracker.unity3d.com/issues/unable-to-unmaximize-console-window-after-undocking-and-maximizing-it-on-macos))
    
*   Editor: Fixed some styling issues with the main editor toolbar ([1296757](https://issuetracker.unity3d.com/issues/styling-issues-in-the-app-toolbar))
    
*   Editor: Fixed Terrain dependency cloning.
    
*   Editor: Fixed the background color of toolbar dropdowns when hovered and pressed ([1313159](https://issuetracker.unity3d.com/issues/toolbar-button-dropdowns-that-are-currently-selected-should-use-the-selected-slash-checked-state-rather-than-the-hover-state))
    
*   Editor: Fixed the behavior where anchor preset window remains open even after a double click. ([1302650](https://issuetracker.unity3d.com/issues/ui-anchor-preset-window-remains-active-even-after-setting-preset))
    
*   Editor: Fixed the editor trying to move an already moved file after dragging a component from the Inspector to the Project Window. ([1301332](https://issuetracker.unity3d.com/issues/the-editor-tries-to-move-a-file-that-has-been-moved-before-when-dragging-the-containers-name-from-inspector-to-project-window))
    
*   Editor: Fixed the GUI error in the console when a media file is opened. ([1294494](https://issuetracker.unity3d.com/issues/gui-error-gets-thrown-in-the-console-when-double-clicking-on-the-selected-video-in-the-object-field))
    
*   Editor: Fixed the issue where editor doesn't show unsaved changes pop up if editor is closed using Unity ->; Quit menu item. ([1320565](https://issuetracker.unity3d.com/issues/macos-editor-doest-show-unsaved-changes-pop-up-if-editor-is-closed-using-unity-quit-menu-item))
    
*   Editor: Fixed the issue where old window was not loosing focus after clicking on a mini pop-up of new window and further new window also gets focus. ([1219099](https://issuetracker.unity3d.com/issues/gameobject-selection-remains-active-in-the-hierarchy-window-when-inspector-window-is-made-active-while-a-dropdown-menu-is-open))
    
*   Editor: Fixed the issue with missing tooltip for Editor tools button. ([1296952](https://issuetracker.unity3d.com/issues/imgui-icons-of-the-editor-tool-is-distorted-and-tooltip-is-missing))
    
*   Editor: Fixed the issue with the Blue highlight being misaligned for the Cooking options dropdown in Mesh Collider. ([1276638](https://issuetracker.unity3d.com/issues/prefabs-blue-highlight-override-indicator-is-misaligned-for-cooking-options-dropdown-in-mesh-collider))
    
*   Editor: Fixed the LOD Group Inspector frames being too dark when using the Light Skin. (1311960)
    
*   Editor: Fixed the path to the scene template icon when querying icon from template path. ([1325888](https://issuetracker.unity3d.com/issues/taking-snapshot-of-a-scenetemplate-in-a-readonly-package-throws-an-exception))
    
*   Editor: Fixed the Recent Scenes menu not being updated after saving via Save As and moved scenes not being correctly tracked.
    
*   Editor: Fixed the Scene View not updating when the LineRenderer Show Wireframe option was changed.
    
*   Editor: Fixed tooltips being misaligned. (1325676)
    
*   Editor: Fixed top of Game View is black when "Use display in HDR mode" is enabled and "Color Space" is set to "Linear". ([1285015](https://issuetracker.unity3d.com/issues/macos-top-of-game-view-is-black-when-use-display-in-hdr-mode-is-enabled-and-color-space-is-set-to-linear-with-dark-theme))
    
*   Editor: Fixed undo on the Advanced Object Selector using the Search Picker not reverting the object field to its original value. (1336998)
    
*   Editor: Fixed Unity does not load the last scene after a crash. (1308699)
    
*   Editor: Generate Release Notes URL according to unity version ([1301927](https://issuetracker.unity3d.com/issues/a-link-to-unity-2020-dot-2-release-notes-are-opened-when-opening-release-notes-in-unity-2021-dot-1))
    
*   Editor: IMGUI buttons don't work in Device Simulator when using the new Input System. ([1333953](https://issuetracker.unity3d.com/issues/imgui-button-presses-dont-get-registered-while-in-a-device-simulator))
    
*   Editor: Improved model import performance by a tiny amount.
    
*   Editor: Improved performance of copy/paste when duplicating large numbers of objects. ([1208321](https://issuetracker.unity3d.com/issues/pasting-undoing-and-deleting-multiple-game-objects-in-the-scene-hierarchy-is-non-linearly-slow))
    
*   Editor: Initializing the static Progress class from a thread no longer throws exceptions. ([1337421](https://issuetracker.unity3d.com/issues/asyncprogress-initializing-the-c-number-progress-class-from-a-non-main-thread-crashes-the-thread))
    
*   Editor: Limited the length of the error messages in the UserRetryDialogs to not more than 200 characters per line. ([1167593](https://issuetracker.unity3d.com/issues/error-message-with-length-of-multiple-screen-sizes-is-generated-when-creating-a-prefab-with-over-the-limit-name-length))
    
*   Editor: Menu Bar doesn't flicker anymore when dragging across monitors. ([1219094](https://issuetracker.unity3d.com/issues/profiler-dragging-standalone-profiler-window-across-monitors-with-different-scaling-settings-changes-its-menu-bar-for-a-moment))
    
*   Editor: Multiple improvements around automatic test-run of tests
    
*   Editor: Nested enumerator execution order fix (DSTR-227).
    
*   Editor: No more exception thrown in the console when inputting unsupported text in the Project Browser search bar. ([1336292](https://issuetracker.unity3d.com/issues/query-breaks-the-adb-provider-and-the-project-browser))
    
*   Editor: Open Prefab' button now uses less inspector space. (1270965)
    
*   Editor: Paste as Child should paste GO relative to parent instead of keeping world transform
    
*   Editor: Pausing playmode in the macOS Editor will no longer keep keys released in pause mode in the pressed position when playmode is unpaused. ([1322149](https://issuetracker.unity3d.com/issues/mac-editor-when-playmode-is-paused-while-a-key-is-pressed-the-gameview-doesnt-register-that-the-key-was-released))
    
*   Editor: Prevent crash when running editor with Mac system debug menu enabled through defaults. ([1301807](https://issuetracker.unity3d.com/issues/macos-crash-on-cocoamainmenu-additems-tomenu-when-apple-internal-debug-menu-is-enabled-on-a-macos))
    
*   Editor: Prevent popup windows from closing in the Linux Editor when child popups are not yet focused ([1309702](https://issuetracker.unity3d.com/issues/gradient-editor-randomly-closes-when-opening-the-color-window-on-linux))
    
*   Editor: Refactoring to make placing windows in the Mac editor more robust and ensure windows are opened on one screen. (1297362)
    
*   Editor: Release mouse if it is dragging when a dialog is opened in the windows editor. ([1271832](https://issuetracker.unity3d.com/issues/mouse-interaction-with-editor-is-disabled-with-editorutility-dot-displaydialog-when-dragging-an-asset-outside-of-the-editor-window))
    
*   Editor: Resolved Prefab object selection performance issue. ([1352527](https://issuetracker.unity3d.com/issues/selecting-a-child-object-of-a-tilemap-is-very-slow))
    
*   Editor: Set gdk cursor invisible when forcing software cursor in editor playmode ([1212108](https://issuetracker.unity3d.com/issues/linux-hardware-cursor-is-not-hidden-in-play-mode-when-using-setcursor-with-cursormode-dot-forcesoftware))
    
*   Editor: Show disable index in the index manager. ([1307781](https://issuetracker.unity3d.com/issues/search-user-created-indices-disappear-from-manager-list-if-disabled))
    
*   Editor: String, Integer, Float, Character and BoundsInt type SerializedProperties now have Copy/Paste context menu options.
    
*   Editor: support Hungarian (and other) unicode characters in editor ([1184456](https://issuetracker.unity3d.com/issues/unicode-symbols-in-0100-017f-and-0180-024f-ranges-are-not-accepted-in-the-text-field))
    
*   Editor: The arrow cursor in the Linux Editor is no longer slightly offset. ([1256724](https://issuetracker.unity3d.com/issues/on-windows-with-scrollbars-near-the-window-border-half-or-all-of-the-scrollbar-isnt-interactable))
    
*   Editor: The background task window is no longer repositioned and resized when opened from the status bar. ([1337646](https://issuetracker.unity3d.com/issues/background-tasks-window-size-change-gets-reverted-after-opening-it-while-tasks-are-running))
    
*   Editor: The EditorSceneManager now gets the correct build index for Scenes of the same name upon calls to SceneManager.GetScenesAt in Play mode. ([1128653](https://issuetracker.unity3d.com/issues/same-build-indices-are-returned-with-scene-dot-buildindex-when-scenes-have-the-same-name))
    
*   Editor: The Object Picker has a maximum number of items it shows. Now showing a note to narrow the search if more than 12000 hits are shown. ([1331728](https://issuetracker.unity3d.com/issues/asset-picker-does-not-show-the-full-list-of-available-assets))
    
*   Editor: The progress bar in the status bar no longer gets stuck in an empty state. The progress bar in the status bar no longer shows instantaneous progresses. (1341616)
    
*   Editor: The Unity Documentation shortcut is no longer installed to the Windows start menu if documentation is not installed. ([921689](https://issuetracker.unity3d.com/issues/unity-documentation-link-is-created-in-start-menu-when-installing-unity-without-documentation))
    
*   Editor: This fix makes sure to unify the il2cpp default order for managed stripping levels in the Player Settings drop-down menu to the one of Mono (Minimal >; Low >; Medium >; High).
    
*   Editor: Transform rotations from asset bundles are now correctly shown in the inspector. ([958333](https://issuetracker.unity3d.com/issues/game-objects-in-that-scene-have-wrong-rotation-value-after-loading-a-scene-from-asset-bundle))
    
*   Editor: UI not running any tests if run select on nested namespaces (DSTR-256).
    
*   Editor: Updated the iOS resolution presets of the _Aspect Ratio_ dropdown list in the _Game View_ window.  
    iOS resolution presets that were removed:  
    
    *   iPhone 4/4S Portrait  
        
    *   iPhone 4/4S Landscape  
        
    *   iPad 2/Mini Portrait  
        
    *   iPad 2/Mini Landscape  
        iOS resolution presets that were added:  
        
    *   iPhone 12 mini 2340x1080 Portrait  
        
    *   iPhone 12 mini 2340x1080 Landscape  
        
    *   iPhone 12/12 Pro 2532x1170 Portrait  
        
    *   iPhone 12/12 Pro 2532x1170 Landscape  
        
    *   iPhone 12 Pro Max 2778x1284 Portrait  
        
    *   iPhone 12 Pro Max 2778x1284 Landscape  
        
    *   iPad (7th-8th gen) 2160x1620 Portrait  
        
    *   iPad (7th-8th gen) 2160x1620 Landscape  
        
    *   iPad Air (4th gen) 2360x1640 Portrait  
        
    *   iPad Air (4th gen) 2360x1640 Landscape  
        
    *   iPad Pro 11-inch 2388x1668 Portrait  
        
    *   iPad Pro 11-inch 2388x1668 Landscape. ([1321829](https://issuetracker.unity3d.com/issues/game-view-aspect-ratio-dropdown-includes-no-longer-supported-devices))
*   Editor: Updated the style of some buttons and button groups when hovered, pressed and focused (1314662)
    
*   Editor: While Editor is entering Play Mode clicking menu doesn't return wrong entry anymore. ([1263313](https://issuetracker.unity3d.com/issues/themes-windows-help-and-window-toolbar-windows-return-wrong-entries-when-being-opened-while-editor-is-entering-play-mode))
    
*   Editor: Wrong ShaderGUI for crosspipeline shaders. (1339817)
    
*   GI: Fix case 1291662: OIDN crashes on AVX512 on MacOS ([1291662](https://issuetracker.unity3d.com/issues/macos-crash-on-zn21mkldnn-primitive-descd2ev-when-using-intel-openvino))
    
*   GI: Fix clearing of lighting data for duplicate scenes saved with the "Save As" option. ([1292192](https://issuetracker.unity3d.com/issues/the-cleared-lightmap-gets-restored-after-reopening-the-scene-that-has-been-saved-as))
    
*   GI: Fix issue with experimental lightmapping.BakeAsync(Scene) interface getting stuck when baking reflection probes in additively opened scenes in the Editor. ([1303788](https://issuetracker.unity3d.com/issues/editor-freezes-when-using-lightmapping-dot-bake-and-the-open-additive-scene-contains-a-reflection-probe))
    
*   GI: Fix Reflection probe (gizmo and texture inspector) appearance in linear color space mode. (1293558)
    
*   GI: Fixed a crash that happens when GPULM tiling is ON, exporting the training data is ON and Ambient occlusion is OFF. (1341803)
    
*   GI: Fixed an issue where sometimes the callstack in Editor.log was incomplete on Windows. (1221524)
    
*   GI: Fixed an issue where the GPU lightmapper seems to be stuck in an endless loop before finishing a bake. (1258690)
    
*   GI: Fixed automated GI tests in HDRP and URP where multiple editors are used.
    
*   GI: Fixed baked lighting on terrain holes and better performance. ([1307459](https://issuetracker.unity3d.com/issues/cpu-baked-lightmap-shows-artifacts-when-game-object-intersects-with-terrain))
    
*   GI: Fixed changes in lighting settings or lightmap parameters not affecting the appearance of baked reflection probes when baking via "Generate Lighting" in the lighting tab. ([1324641](https://issuetracker.unity3d.com/issues/changes-to-denoising-or-gi-samples-counts-are-not-rendered-in-reflection-probes-when-baking-gi-from-the-lighting-window))
    
*   GI: Fixed crash when closing editor while generating lighting. ([1354238](https://issuetracker.unity3d.com/issues/fatal-error-when-closing-the-editor-while-generating-lighting))
    
*   GI: Fixed crash with CPU OpenCL devices. ([1338498](https://issuetracker.unity3d.com/issues/crash-when-baking-lights-for-a-scene-with-a-terrain-using-progressive-gpu-lightmapper-with-a-weaker-gpu))
    
*   GI: Fixed fallback to CPU lightmapper when writing LightCookies buffer and using Clear baked Data. ([1321887](https://issuetracker.unity3d.com/issues/gpulm-fallback-to-cpulm-failing-when-writing-lightcookies-buffer-and-using-clear-baked-data))
    
*   GI: Fixed light baking gets stuck in a infinite loop when unloading a light baked scene if you have another scene open. ([1337508](https://issuetracker.unity3d.com/issues/light-baking-gets-stuck-in-a-infinite-loop-when-unloading-a-light-baked-scene-if-you-have-another-scene-open))
    
*   GI: Fixed memory usage and performance regression when baking light probes. (1324307)
    
*   GI: Fixed missing indirect lighting when using Enlighten Realtime GI in HDRP Player. ([1367133](https://issuetracker.unity3d.com/issues/missing-lights-when-using-enlighten-realtime-gi-in-hdrp))
    
*   GI: Fixed out of bounds access in probeDepthOctahedronExpandedBuffer when generating Probe Volumes 1.0 data via experimental API. ([1321881](https://issuetracker.unity3d.com/issues/gpulm-fallback-to-cpulm-failing-on-reading-totalrayscastcountbuffer))
    
*   GI: Fixed prefab instances losing their lighting when they are unpacked, and the scene is reloaded. ([1285269](https://issuetracker.unity3d.com/issues/lightmap-is-shown-in-the-inspector-window-from-an-unpacked-prefab-when-restarting-a-scene))
    
*   GI: Fixed rare crash when entering play mode while running a GI lightbake. ([1301678](https://issuetracker.unity3d.com/issues/crash-after-assertion-failed-on-expression-bakedlightchannel-4-when-entering-play-mode-after-editing-terrain-trees))
    
*   GI: Fixed reflection probes not being zeroed out when lighting is cleared.
    
*   GI: Fixed scene lighting data not getting updated when the selected Lighting Data Asset for the scene is changed. ([1263683](https://issuetracker.unity3d.com/issues/lighting-backed-lightmaps-preview-does-not-update-with-respect-to-lighting-data-asset-when-it-is-set-none))
    
*   GI: Fixed some fallbacks from GPULM to CPULM when using baked lighting and cookies. (1320169)
    
*   GI: Fixed unused return value during remapping of scene object id's. (1300323)
    
*   GI: Fixedcorruption in Probe baking when lightmap UVs are not provided. ([1337226](https://issuetracker.unity3d.com/issues/lightprobes-corruption-in-probe-baking-when-lightmap-uvs-are-not-provided))
    
*   GI: Ignore OpenCL CPU devices that are incompatible with the GPU lightmapper on macOS due to insufficient local workgroup size. ([1293520](https://issuetracker.unity3d.com/issues/gpu-lightmapper-doesnt-work-on-macos-opencl-cpu-devices))
    
*   GI: Improved error logging when reporting errors relating to UV unwraps during a lightmap bake. (1327322)
    
*   GI: Introduced a full tiled-based baking system to the GPULM to reduce memory pressure.  
    Some other improvements on memory consumption and baking speed on the GPU light mapper when the user is not activating some baking features.  
    Reduced the memory consumption of probe baking using the GPULM (4Bytes per probe).  
    Better estimation of the GPULM memory consumption even when tiling is off, making it less likely to fallback to CPULM.
    
*   GI: Make emission tooltip take Enlighten realtime GI state into account. ([1329323](https://issuetracker.unity3d.com/issues/emission-tooltip-is-not-taking-enlighten-realtime-gi-state-into-account))
    
*   GI: Make GPU lightmapper detect Intel IRIS Xe MAX GPU with 4GB memory. ([1331794](https://issuetracker.unity3d.com/issues/gpu-lightmapper-isnt-detecting-the-discrete-intel-iris-x-max-gpu-with-4gb-memory))
    
*   GI: Make it possible for the job manager to shut down the editor even if the OpenCL driver stopped working. ([1276653](https://issuetracker.unity3d.com/issues/gpu-plm-editor-stalls-on-closing-with-various-rif-errors-after-ungraceful-fallback-to-cpu-plm-when-baking-with-radeon-denoiser))
    
*   GI: Make the compression label in Lighting Window - Baked Lightmaps better. (1297198)
    
*   GI: Reenabling a disabled light, reflection probe, or light probe group now makes it immediately visible in the Light Explorer. ([1320277](https://issuetracker.unity3d.com/issues/reflection-probes-and-light-groups-are-not-getting-updated-in-the-light-explorer-when-they-are-disabled-and-re-enabled))
    
*   GI: Reimport all lightmap textures when "Lightmap Encoding" project setting is changed. ([1195551](https://issuetracker.unity3d.com/issues/changing-lightmap-encoding-setting-does-not-take-effect-unless-one-nukes-library-slash-directory-and-restarts-unity))
    
*   GI: Removed erroneous asserts in scene object identifier remapping code.
    
*   GI: Removed terrain trees from being drawn in the shadowmask scene visualization mode as background objects as they do not receive a shadowmask, anyway. ([1295410](https://issuetracker.unity3d.com/issues/wrong-scaling-in-shadow-mask-scene-view-mode))
    
*   GI: Removed the Unity process count check that is used to guard the GI Cache from getting trimmed by other Editors, as the asset import workers are counted as Editors. ([1313354](https://issuetracker.unity3d.com/issues/gicache-related-warning-when-the-out-of-process-importer-is-active))
    
*   GI: Support high intensity skyboxes for baking. ([1222492](https://issuetracker.unity3d.com/issues/plm-baked-contribution-from-high-intensity-hdris-is-not-handled-properly-in-linear-color-space))
    
*   GI: Use shadow penumbra to sort lights with penumbra by in the GPU lightmapper instead of indirect color. ([1319138](https://issuetracker.unity3d.com/issues/gpu-lightmapper-penumbra-shadow-sorting-is-incorrect))
    
*   Graphics: \* Improved support for ghosting particles.  
    
    *   Improved sharpening and other minor fixes from NVIDIA. (1345143)
*   Graphics: Add CameraBuffer VFX type to encapsulate camera buffers that can be Texture2D or Texture2DArray depending on the platform ([1213482](https://issuetracker.unity3d.com/issues/camera-buffers-cant-access-depth-or-color-buffers-in-osx-directly-in-the-vfx-graph))
    
*   Graphics: Add control to independently clear stencil buffer in CommandBuffer api.  
    Clearing depth does not implicitly clear stencil anymore.
    
*   Graphics: Added check for Vulkan support in Unity player. ([1308206](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-on-vkenumeratephysicaldevices-when-starting-the-player-without-vulkan-drivers-installed-on-the-system))
    
*   Graphics: Added exception when creating 3d textures with depth/stencil format on metal, as this is not supported. (1296524)
    
*   Graphics: Added GetActiveTerrains method which will fill a user-provided List with the active terrains, allowing users to control the resulting allocation. (1324062)
    
*   Graphics: Added Metal Compute Pipeline Validation to the Editor (1283446)
    
*   Graphics: Added per-camera freeUnusedRenderResources control to allow preservation of cameradata for infrequently-updated cameras. This prevents performance spikes that occur due to recreation of cameras that are guaranteed to be updated eventually, but at a frequency lower than once every 100 frames. (1296777)
    
*   Graphics: Added support for having multiple different Renderers on the same Game Object when using ray tracing. ([1305305](https://issuetracker.unity3d.com/issues/dxr-errors-appear-in-the-console-window-when-a-game-object-has-multiple-renderer-types))
    
*   Graphics: Apple Silicon editor game view glitches were caused by discarding/overwriting the game view render texture data - this has been fixed. ([1368374](https://issuetracker.unity3d.com/issues/game-view-glitches-with-apple-silicon-editor))
    
*   Graphics: Backport sllowing for Depth Sharing in Vulkan.
    
*   Graphics: Calculating correct rtHandleScale by considering the possible pixel rounding when DRS is on.
    
*   Graphics: Creating a RenderTexture in D3D12 with RenderTexture.antiAliasing value higher than supported by hardware will no longer crash the editor. ([1310791](https://issuetracker.unity3d.com/issues/dx12-editor-crashes-when-creating-a-rendertexture-with-rendertexture-dot-antialiasing-value-higher-than-supported-by-hardware))
    
*   Graphics: Disable Motion Vectors pass in Output Meshes even when other output has motion vectors enabled ([1313043](https://issuetracker.unity3d.com/issues/output-mesh-uses-particle-motion-vectors-even-when-it-is-not-moving-and-its-shader-is-not-set-to-support-them))
    
*   Graphics: Disabled "create material" button in terrain inspector when viewed through a preset. ([1290453](https://issuetracker.unity3d.com/issues/terrain-material-asset-doesnt-generate-in-the-project-window-on-creating-it-from-terrain-settings-in-the-preset-of-terrain))
    
*   Graphics: Disabled ShadowCaster pass in Output Meshes if castShadows is disabled.
    
*   Graphics: Fix bug where in some situations the AsyncUploadBuffer was not persisting even when QualitySettings.asyncUploadPersistentBuffer was set to true. ([1150408](https://issuetracker.unity3d.com/issues/ios-npot-textures-without-compression-uses-more-memory-than-a-regular-texture))
    
*   Graphics: Fix CPU performance issue when light probes and ray tracing effects are used together.
    
*   Graphics: Fix crash when using RenderPass without depth on Metal devices
    
*   Graphics: Fix issue with GrayScaleRGBToAlpha for 16bpc textures (1295408)
    
*   Graphics: Fix rare deadlock that can occur when a texture fails to load. (1265360)
    
*   Graphics: Fix shadow normal bias slider getting clamped at 3. ([1213200](https://issuetracker.unity3d.com/issues/urp-light-custom-normal-shadow-bias-is-capped-at-3))
    
*   Graphics: Fix Simplify button clipping in the LineRenderer Inspector when the window was narrow. ([1308478](https://issuetracker.unity3d.com/issues/shuriken-property-under-the-line-renderer-is-going-out-of-panel-when-the-inspector-window-is-resized))
    
*   Graphics: Fixed a bug with Cubemap.GetPixel(CubemapFace face, int x, int y) not passing its parameters correctly. (1305539)
    
*   Graphics: Fixed a case that render thread calls main thread only API in editor. (1317190)
    
*   Graphics: Fixed a crash that would occur when trying to create a VT GPU cache larger than the available GPU memory. (1293468)
    
*   Graphics: Fixed a crash when a RenderTexture is created using MSAA with random write flag which is an invalid combination. Return an error in the Console when this happens. ([1343544](https://issuetracker.unity3d.com/issues/urp-game-view-goes-black-when-msaa-and-cs-render-pass-feature-are-enabled))
    
*   Graphics: Fixed a crash when calling GetSize() on a RayTracingAccelerationStructure before calling the initial Build() on it. ([1363258](https://issuetracker.unity3d.com/issues/dxr-unity-editor-crashes-when-calling-getsize-on-an-acceleration-structure-before-building-it-with-build))
    
*   Graphics: Fixed a crash when passing in DepthAuto or ShadowAuto into SystemInfo.GetCompatibleFormat. (1343093)
    
*   Graphics: Fixed a critical issue on android devices & lens flares. Accidentally creating a 16 bit texture was causing gpus not supporting them to fail.
    
*   Graphics: Fixed a large, visible stretch ratio in a LensFlare Image thumbnail.
    
*   Graphics: Fixed a regression where calling the the Texture2D.Resize method with a Texture format parameter caused the underlying GraphicsFormat to flip color spaces on each call. ([1312670](https://issuetracker.unity3d.com/issues/texture2d-dot-resize-toggles-graphicsformat-each-time-its-called-between-linear-and-srgb))
    
*   Graphics: Fixed a situation which could cause the GPU to crash when a Skinned Mesh Renderer is assigned a mesh, which does not match the expected size/stride setup, and that Skinned Mesh Renderer is then used immediately before skinning has had a chance to happen.
    
*   Graphics: Fixed ACES filter artefact due to half float error on some mobile platforms.
    
*   Graphics: Fixed alignment in Volume Components.
    
*   Graphics: Fixed ALL/NONE to maintain the state on the Volume Component Editors.
    
*   Graphics: Fixed an incorrect error check in the BC7 decompressor. (1339809)
    
*   Graphics: Fixed an issue with ReadPixels() over 3 API's, where the first slice would always be returned instead of the specified depth slice. The bug was being caused by the active cubemap face only being used, the fix checks whether it should use the active depth slice or cubemap face. ([979487](https://issuetracker.unity3d.com/issues/texture2d-dot-readpixels-does-not-take-into-account-the-specified-depthslice))
    
*   Graphics: Fixed an uninitialized value problem found by Vulkan. (1309741)
    
*   Graphics: Fixed and issue where scene view filtering would now work properly for SRP's. ([1180254](https://issuetracker.unity3d.com/issues/gameobject-with-tessellation-shader-is-incorrectly-greyed-out-after-search-in-hierarchy))
    
*   Graphics: Fixed another recently added internal bug where when the shader debug level in Switch player editor settings is changed, the shaders were not corectly rebuilt.
    
*   Graphics: Fixed API to draw color temperature for Lights.
    
*   Graphics: Fixed assertion failure when releasing rendererlists in certain scenes. (1342215)
    
*   Graphics: Fixed assertion on compression of L1 coefficients for Probe Volume.
    
*   Graphics: Fixed black pixel issue in AMD FidelityFX RCAS implementation.
    
*   Graphics: Fixed bug where ComputeShader.IsSupported for OpenGL (ES) would only return false on the first call for kernel that did not compiler at runtime. (1334034)
    
*   Graphics: Fixed crash when a compute shader does not compile when using OpenGL. ([1324695](https://issuetracker.unity3d.com/issues/crash-on-android-device-when-using-gles3-dot-0))
    
*   Graphics: Fixed crash when calling AsyncGPUReadback.RequestIntoNativeArray with a temp allocated array. ([1336583](https://issuetracker.unity3d.com/issues/unity-crashes-when-forcing-render-texture-to-update-before-it-being-initialized))
    
*   Graphics: Fixed crash when calling GetPixelData with invalid arguments. ([1322485](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-entering-play-mode-and-the-index-is-out-of-range-in-texture-data))
    
*   Graphics: Fixed crash when DX12 Hardware Dynamic Resolution Scaling is enabled on XR. (1323531)
    
*   Graphics: Fixed crash when executing CommandBuffer.DrawProcedural and some other functions that refer to an already deleted ComputeBuffer or GraphicsBuffer. ([1323447](https://issuetracker.unity3d.com/issues/graphics-possible-to-crash-unity-with-a-stale-slash-disposed-graphicsbuffer-in-a-commandbuffer))
    
*   Graphics: Fixed crash when launching tutorials on Linux with AMD/Intel cards. ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Graphics: Fixed crash when switching resolutions rapidly on the unity editor when hardware DRS is enabled on HDRP. (1353948)
    
*   Graphics: Fixed crash wrong format desc of GraphicsFormat.VideoAuto on metal. (1296529)
    
*   Graphics: Fixed cropped thumbnail for Image with non-uniform scale and rotation
    
*   Graphics: Fixed disappearing mesh when "Keep Quads" is enabled in import settings. ([1327826](https://issuetracker.unity3d.com/issues/mesh-disappears-when-keep-quads-is-enabled-in-the-fbx-import-settings))
    
*   Graphics: Fixed double underscores in Hybrid Renderer shader constant names.
    
*   Graphics: Fixed DrawProcedural reporting incorrect triangle counts to FrameStats.
    
*   Graphics: Fixed empty RenderTexture.ResolveAA debug marker appearing in Frame Debugger and other frame capture tools on mobile platforms. (1330944)
    
*   Graphics: Fixed error when change Lens Flare Element Count followed by undo. (1346894)
    
*   Graphics: Fixed explicit half precision not working even when Unified Shader Precision Model is enabled.
    
*   Graphics: Fixed false-positive error message during ReadbackImage on GLCore. (1297065)
    
*   Graphics: Fixed frame debugger crash when using the RenderPass API with MSAA enabled. (1317665)
    
*   Graphics: Fixed gizmo rendering in SRP when wireframe mode is selected (1251022)
    
*   Graphics: Fixed GPU crash on Intel integrated cards when opening the editor with a scene that had VFX. ([1332956](https://issuetracker.unity3d.com/issues/gpu-crashes-on-creating-an-hdrp-project-on-integrated-gpus-when-vfx-layer-is-used))
    
*   Graphics: Fixed HDRP Camera Binder errors related to depthBuffer and colorBuffer properties. ([1353845](https://issuetracker.unity3d.com/issues/hdrp-camera-binder-throws-error))
    
*   Graphics: Fixed HDRP Runtime test failure in Vulkan caused by incorrect shader code generation. (1323529)
    
*   Graphics: Fixed IES Importer related to new API on core.
    
*   Graphics: Fixed in crash for software DRS for DLSS in dx12 when changing the resolution mid frame. (1352848)
    
*   Graphics: Fixed incorrect GeometryJob Fence initialisation causing graphical corruption in UI canvas rendering.
    
*   Graphics: Fixed incorrect warning in when creating a texture from script with a compressed format that is not supported on the Editor platform. ([1317998](https://issuetracker.unity3d.com/issues/android-non-supported-texture-format-options-are-shown-in-the-texture-import-settings))
    
*   Graphics: Fixed issue displaying a warning of different probe reference volume profiles even when they are equivalent.
    
*   Graphics: Fixed issues caused by automatically added EventSystem component, required to support Rendering Debugger Runtime UI input. (1361901)
    
*   Graphics: Fixed L2 for Probe Volumes.
    
*   Graphics: Fixed layered rendering (and validation errors) with 3D Textures when using Vulkan. (1323740)
    
*   Graphics: Fixed layered rendering to mips of 3D textures when using Vulkan. (1329180)
    
*   Graphics: Fixed Lens Flare 'radialScreenAttenuationCurve invisible'.
    
*   Graphics: Fixed Lens Flare position for celestial at very far camera distances. It now locks correctly into the celestial position regardless of camera distance. (1363291)
    
*   Graphics: Fixed Lens Flare rotation for Curve Distribution.
    
*   Graphics: Fixed Lens Flare Thumbnails.
    
*   Graphics: Fixed library function SurfaceGradientFromTriplanarProjection to match the mapping convention used in SampleUVMappingNormalInternal.hlsl and fix its description.
    
*   Graphics: Fixed Light Layers with duplicate names being hidden in Light or Renderer component. (1335982)
    
*   Graphics: Fixed Light Probe evaluation in ray tracing shaders resulting in wrong ambient colors. Fixed Light Probe Proxy Volume setup not binding SH2 L2 band uniforms in ray tracing shaders. ([1330711](https://issuetracker.unity3d.com/issues/dxr-light-probe-evaluation-in-ray-tracing-shaders-results-in-wrong-ambient-colors))
    
*   Graphics: Fixed LightAnchor too much error message, became a HelpBox on the Inspector.
    
*   Graphics: Fixed memory leak when changing SRP pipeline settings, and having the player in pause mode.
    
*   Graphics: Fixed Metal DebugGroups during Xcode GPU Frame Capture getting incorrectly nested when using RenderPass API. (1330942)
    
*   Graphics: Fixed Metal multisample depth resolve not working. (1330714)
    
*   Graphics: Fixed missing increment/decrement controls from DebugUIIntField & DebugUIUIntField widget prefabs.
    
*   Graphics: Fixed missing support for coarse/fine derivatives in shader code.
    
*   Graphics: Fixed normal bias field of reference volume being wrong until the profile UI was displayed.
    
*   Graphics: Fixed performance regression when changing Mesh vertices or indices. ([1326091](https://issuetracker.unity3d.com/issues/updating-mesh-geometry-is-much-slower-since-2021-dot-1))
    
*   Graphics: Fixed potentially conflicting runtime Rendering Debugger UI command by adding an option to disable runtime UI altogether. ([1345783](https://issuetracker.unity3d.com/issues/hdrp-it-is-not-possible-to-disable-the-runtime-debug-display-window-in-the-editor))
    
*   Graphics: Fixed problem on domain reload of Volume Parameter Ranges and UI values.
    
*   Graphics: Fixed random crash when reloading VFX under special circumstances. ([1291710](https://issuetracker.unity3d.com/issues/vfx-graph-crash-subgraph-with-output-mesh-using-a-random-for-the-mesh))
    
*   Graphics: Fixed readback/blit from backbuffer in Editor when running GLES. (1301446)
    
*   Graphics: Fixed regression where RenderTextureDescriptor.depthBufferBits or RenderTexture.depth could return GraphicsFormat.None when setting the properties to 24 or 32 bit. (1340405)
    
*   Graphics: Fixed RenderPass API MSAA and clear action issues when writing to the backbuffer on Android (1315433)
    
*   Graphics: Fixed Right Align of additional properties on Volume Components Editors.
    
*   Graphics: Fixed rotation issue now all flare rotate on positive direction. ([1348570](https://issuetracker.unity3d.com/issues/hdrp-lens-flare-flares-flipped-for-multiple-elements-with-auto-rotate-enabled))
    
*   Graphics: Fixed ScriptableRenderContext.ExecuteCommandBuffer crashing when called with a disposed command buffer ([1306222](https://issuetracker.unity3d.com/issues/unity-crashes-when-executing-commandbuffer))
    
*   Graphics: Fixed selection of sRGB format for rendertextures inspector. ([1295276](https://issuetracker.unity3d.com/issues/cant-select-srgb-color-format-for-render-texture-on-hdrp-project))
    
*   Graphics: Fixed situation where Hybrid Renderer could throw errors because of invalid reflection data.
    
*   Graphics: Fixed skybox cubemap corruption in Vulkan. (1195394)
    
*   Graphics: Fixed spacing between property fields on the Volume Component Editors.
    
*   Graphics: Fixed static batching bug related to rendering layer mask. Meshes that are set up with different rendering layer masks (unity\_RenderingLayer uniform variable in shader code), are now correctly split when static batching is enabled instead of being merged, which would otherwise generate incorrect rendering if unity\_RenderingLayer was accessed by the shader code.
    
*   Graphics: Fixed SystemInfo.supportsRenderTargetArrayIndexFromVertexShader when using Vulkan. (1269732)
    
*   Graphics: Fixed tessellation factors access in domain shaders on Metal/Vulkan. ([1337590](https://issuetracker.unity3d.com/issues/hlslcc-generates-incorrect-metal-shaders-when-tessellation-factors-are-read-in-then-domain-post-tessellation-vertex-stage))
    
*   Graphics: Fixed Texture resource state that can be incorrect when the destination texture of Graphics.Blit() is also set as \_MainTex of the blit material. (1323521)
    
*   Graphics: Fixed Texture2D.GetPixel(int x, int y, int miplevel) internally passing the miplevel parameter incorrectly. (1284757)
    
*   Graphics: Fixed Texture3D.CreateExternalTexture to work correctly with Vulkan. (1322987)
    
*   Graphics: Fixed TextureGenerator.GenerateTexture throws null pointer exception when running with enablePostProcessor to true. (1283888)
    
*   Graphics: Fixed the display name of a Volume Parameter when is defined the attribute InspectorName.
    
*   Graphics: Fixed the documentation of CommandBuffer.EndSample. ([1264605](https://issuetracker.unity3d.com/issues/commandbuffer-dot-endsample-intellisense-comment-is-identical-to-commandbuffer-dot-beginsample))
    
*   Graphics: Fixed the location of the "Shader Graph" asset create menu to be next to the "Shader" menu. ([1337080](https://issuetracker.unity3d.com/issues/shadergraph-shadergraph-menu-in-assets-right-click-menu-is-at-the-bottom))
    
*   Graphics: Fixed the multicamera tests on Linux. (1318477)
    
*   Graphics: Fixed the random position of the Rendering Submenu on Assets >; Create. (1341763)
    
*   Graphics: Fixed the selection of the Additional properties from ALL/NONE when the option "Show additional properties" is disabled.
    
*   Graphics: Fixed to RenderTexture.format not returning correct values in the case of RenderTextureFormat.Depth and RenderTextureFormat.Shadow. (1365548)
    
*   Graphics: Fixed Undo from script refreshing thumbnail.
    
*   Graphics: Fixed unstable async readback test. (1288678)
    
*   Graphics: fixed Unwrap crash when automatic margin calculation results in very small margin ([1308365](https://issuetracker.unity3d.com/issues/fbx-uv-unwrapper-crashes-on-specific-meshes))
    
*   Graphics: Fixed various issues wrt uploading Virtual texturing tiles when using non-native texture formats. (1337269)
    
*   Graphics: Fixed Volume Gizmo size when rescaling parent GameObject.
    
*   Graphics: Fixed Vulkan API AccessTextureByID which was failing due to an incorrect internal implementation.
    
*   Graphics: Fixing bug were a very strong emissive could leak if placed behind a canvas surface in the scene. ([1295722](https://issuetracker.unity3d.com/issues/hdrp-high-emissive-material-leaks-through-canvas-ui-image-in-screen-space-camera-in-scene-view))
    
*   Graphics: Flagged kFormatB10G11R11\_UFloatPack32 as a HDR format (1310527)
    
*   Graphics: Force reload of VFX graph compute shaders when reloading assembly. ([1107178](https://issuetracker.unity3d.com/issues/unity-crashes-if-the-vfx-graph-package-is-removed-while-vfx-graph-stuff-exists-in-the-scene))
    
*   Graphics: Game View Stats Saved by Batching is always 0 when using SRPBatcher. ([1329391](https://issuetracker.unity3d.com/issues/game-view-stats-saved-by-batching-is-always-0-when-using-srpbatcher))
    
*   Graphics: GetGraphicsApiMask should be called in VisualEffectImporter to force reimport while changing API. (1300054)
    
*   Graphics: GetPixels,SetPixels,GetPixels32,SetPixels32 will now throw exceptions when failing instead of printing error messages. A number of bugs were fixed that could crash unity. ([1293040](https://issuetracker.unity3d.com/issues/crash-in-getcolorblockcolors-when-calling-texture2d-dot-getpixels32-for-crunched-texture-formats))
    
*   Graphics: Graphics: Fixing DLSS vulkan black pixels / frame corruption of first frame. (1335735)
    
*   Graphics: GUIView.GrabPixels() on Metal will now fill the RenderTexture with valid content (1223120)
    
*   Graphics: Help boxes with fix buttons do not crop the label.
    
*   Graphics: Make metal query max tessellation factor from the driver instead of clamping to 16 always. ([1289859](https://issuetracker.unity3d.com/issues/mac-maxtessellationlevel-cannot-be-changed-for-metal))
    
*   Graphics: Metal shaders will compile correctly when referencing tessellation factors in the domain shader. ([1139698](https://issuetracker.unity3d.com/issues/shader-is-rendered-wrongly-in-magenta-or-light-blue-color-without-any-errors-when-using-macos))
    
*   Graphics: Minor UX improvements on Quality Settings Panel.
    
*   Graphics: NVIDIA package no longer gets enabled when a project is updated to a new version of unity. This was the result of a bad configuration. ([1342012](https://issuetracker.unity3d.com/issues/upgrading-projects-automatically-enables-com-dot-unity-dot-modules-dot-nvidia-package))
    
*   Graphics: Order of DLSS quality enumerations changed for better and more intuitive user experience. This change does not break API. (1335732)
    
*   Graphics: OSX Metal editor playmode wasn't using VSync in the game view properly when enabled - this has been fixed. (1371550)
    
*   Graphics: Partially fix limitation of sending only one event per frame : the direct link supports multiple event sent within the same frame.
    
*   Graphics: Pause VFX when frame debugger is enabled. ([1195088](https://issuetracker.unity3d.com/issues/profiling-frame-debugger-flickers-when-a-vfx-is-present))
    
*   Graphics: Properly handle terrain pixel error calculations for orthographic cameras. ([1244606](https://issuetracker.unity3d.com/issues/terrains-pixel-error-value-has-no-effect-when-orthographic-cameras-near-clipping-plane-is-set-to-zero))
    
*   Graphics: Provided an appropriate API to update builtin reflection probes internal data. ([1207660](https://issuetracker.unity3d.com/issues/realtime-reflection-probe-is-not-updated-correctly-when-parent-containing-probe-slash-camera-slash-model-is-moved-in-play-mode))
    
*   Graphics: Put objects with negative scale into separate static batch. This makes normal maps display correctly on those objects. ([1205209](https://issuetracker.unity3d.com/issues/static-batching-changes-normal-map-on-gameobjects-when-negative-values-are-used-on-scale))
    
*   Graphics: Reduced main thread hitching caused by Shader loading.
    
*   Graphics: Removed GraphicsFormat warning for RenderTextures when changing color space to gamma. ([1284779](https://issuetracker.unity3d.com/issues/srgb-format-warning-occurs-when-color-space-is-set-to-gamma-and-hdr-is-off))
    
*   Graphics: Removed the error message when encountering incompatible pipeline stages on DX12.
    
*   Graphics: Removed the unneeded data copy of the initialised memory to video memory when creating a texture from script. (1337186)
    
*   Graphics: Removed unnecessary api files for NVIDIA Module.
    
*   Graphics: Removed URP and HDRP templates. They are now dynamic templates
    
*   Graphics: RenderTextures are no longer forced to use Clamp border sampling if a format with depth is used. ([1292651](https://issuetracker.unity3d.com/issues/rendertexture-wrap-mode-does-nothing))
    
*   Graphics: Resolved exact fixed time step flickering while using strip (and other unexpected behavior). (1289829)
    
*   Graphics: Scissor test was automatically disabled when changing render-targets. It is not the case anymore and is consistent with other platforms.
    
*   Graphics: Skip wind calculations for Speed Tree 8 when wind vector is zero. ([1335487](https://issuetracker.unity3d.com/issues/unlit-shader-graph-with-shadow-matte-option-enabled-does-not-receive-shadows-when-path-tracing-is-enabled))
    
*   Graphics: Support undo of Global Settings assignation ([1342987](https://issuetracker.unity3d.com/issues/undo-is-not-working-in-global-settings))
    
*   Graphics: The warning was removed because URP / HDRP now no longer need to have an asset assigned to both Graphics and Quality to work. (1335986)
    
*   Graphics: Updated SpeedTree importer editor to correctly regenerate materials with custom render pipelines. Only shows the "Receive Shadows" toggle if that functionality is supported by the current SupportedRenderingFeatures. (1338973)
    
*   Graphics: Using CopyTexture on textures with different MSAA sample counts throws an error. ([1308132](https://issuetracker.unity3d.com/issues/using-copytexture-on-textures-with-different-msaa-sample-counts-throws-an-error))
    
*   Graphics: Virtual Texturing fallback texture sampling code correctly honors the enableGlobalMipBias when virtual texturing is disabled.
    
*   Graphics: Visual Effects in prefabs always show as modified. ([1285787](https://issuetracker.unity3d.com/issues/prefab-visual-effects-in-prefabs-always-show-as-modified))
    
*   Graphics: Visual effects will continue to cast shadows even when they are not visible in camera. ([1279851](https://issuetracker.unity3d.com/issues/output-vfx-dont-cast-shadows-when-culled))
    
*   Graphics: VisualEffect could cause an unexpected assert if the graph samples a skinned mesh renderer with cloth ([1307808](https://issuetracker.unity3d.com/issues/assertions-when-sampling-cloth-skinned-mesh-renderer-in-vfx))
    
*   Graphics: When adding Overrides to the Volume Profile, only show Volume Components from the current Pipeline.
    
*   Graphics: When creating PVRTC texture which is not POT and square throw an exception, as it is not supported and might result in crashes later on. (1329461)
    
*   HDRP: Added a new property to control the ghosting reduction for volumetric clouds. (1357702)
    
*   HDRP: Allow negative wind speed parameter.
    
*   HDRP: Assets going through the migration system are now dirtied.
    
*   HDRP: Cleanup Shader UI.
    
*   HDRP: Fix crash on VolumeComponentWithQualityEditor when the current Pipeline is not HDRP
    
*   HDRP: Fixed a bug with Reflection Probe baking would result in an incorrect baking reusing other's Reflection Probe baking.
    
*   HDRP: Fixed a bug with Reflection Probe baking would result in an incorrect baking reusing other's Reflection Probe baking.
    
*   HDRP: Fixed a compilation issue for AxF carpaints on Vulkan
    
*   HDRP: Fixed a divide-by-zero warning for anisotropic shaders (Fabric, Lit).
    
*   HDRP: Fixed a lack of syncronization between the camera and the planar camera for volumetric cloud animation data.
    
*   HDRP: Fixed a limit case when the camera is exactly at the lower cloud level. (1316988)
    
*   HDRP: Fixed a locale issue with the diffusion profile property values in ShaderGraph on PC where comma is the decimal separator.
    
*   HDRP: Fixed a memory leak related to not disposing of the RTAS at the end HDRP's lifecycle.
    
*   HDRP: Fixed a NaN generating in Area light code.
    
*   HDRP: Fixed a null ref exception when adding a new environment to the Look Dev library.
    
*   HDRP: Fixed a null ref exception when no opaque objects are rendered.
    
*   HDRP: Fixed a nullref in volume system after deleting a volume object. ([1348374](https://issuetracker.unity3d.com/issues/hdrp-missingreferenceexception-is-thrown-when-volume-is-destroyed-after-its-layer-is-changed))
    
*   HDRP: Fixed a nullref when binding a RTHandle allocated from a RenderTextureIdentifier with CoreUtils.SetRenderTarget.
    
*   HDRP: Fixed a regression that broke punctual and directional raytraced shadows temporal denoiser. (1360132)
    
*   HDRP: Fixed a warning to Rendering Debugger Runtime UI when debug shaders are stripped.
    
*   HDRP: Fixed a warning when enabling tile/cluster debug.
    
*   HDRP: Fixed ability to override AlphaToMask FrameSetting while camera in deferred lit shader mode.
    
*   HDRP: Fixed ability to override AlphaToMask FrameSetting while camera in deferred lit shader mode.
    
*   HDRP: Fixed access to main directional light from script.
    
*   HDRP: Fixed Additional Velocity for Alembic not taking correctly into account vertex animation.
    
*   HDRP: Fixed aliasing artifacts that are related to numerical imprecisions of the light rays in the volumetric clouds. (1340731)
    
*   HDRP: Fixed ambient occlusion strenght incorrectly using GTAOMultiBounce.
    
*   HDRP: Fixed an error when deleting the 3D Texture mask of a local volumetric fog volume (1339330)
    
*   HDRP: Fixed an incompatibility between MSAA and Volumetric Clouds.
    
*   HDRP: Fixed an inconsistency between perf mode and quality mode for material simplification in RTGI.
    
*   HDRP: Fixed an inconsistency between perf mode and quality mode for sky lighting.
    
*   HDRP: Fixed an issue in the planar reflection probe convolution.
    
*   HDRP: Fixed an issue that clamped the volumetric clouds offset value. (1357318)
    
*   HDRP: Fixed an issue that made camera motion vectors unavailable in custom passes.
    
*   HDRP: Fixed an issue that made Custom Pass buffers inaccessible in ShaderGraph.
    
*   HDRP: Fixed an issue where auto baking of ambient and reflection probe done for builtin renderer would cause wrong baking in HDRP.
    
*   HDRP: Fixed an issue where disabled reflection probes were still sent into the the ray tracing light cluster.
    
*   HDRP: Fixed an issue where first frame of SSAO could exhibit ghosting artefacts.
    
*   HDRP: Fixed an issue where runtime debug window UI would leak game objects.
    
*   HDRP: Fixed an issue where selection in a debug panel would reset when cycling through enum items.
    
*   HDRP: Fixed an issue where sometime a docked lookdev could be rendered at zero size and break.
    
*   HDRP: Fixed an issue with debug overriding emissive material color for deferred path. (1313123)
    
*   HDRP: Fixed an issue with Decal normal blending producing NaNs.
    
*   HDRP: Fixed an issue with half res ssgi upscale.
    
*   HDRP: Fixed an issue with normal management for recursive rendering (1324082)
    
*   HDRP: Fixed an issue with reflection probe normalization via APV when no probes are in scene.
    
*   HDRP: Fixed an issue with resolution dependence for physically based depth of field.
    
*   HDRP: Fixed an issue with surface gradient based normal blending for decals (volume gradients weren't converted to SG before resolving in some cases).
    
*   HDRP: Fixed an issue with TAA causing objects not to render at extremely high far flip plane values.
    
*   HDRP: Fixed an issue with the capture callback (now includes post processing results).
    
*   HDRP: Fixed an issue with the mipmap generation internal format after rendering format change.
    
*   HDRP: Fixed an issue with volumetric clouds on vulkan. (1354802)
    
*   HDRP: Fixed artifact appearing when diffuse and specular normal differ too much for eye shader with area lights.
    
*   HDRP: Fixed artifacts in volumetric cloud shadows.
    
*   HDRP: Fixed assert failure when enabling the probe volume system for the first time.
    
*   HDRP: Fixed AxF debug output in certain configurations ([1333780](https://issuetracker.unity3d.com/issues/shader-compilation-error-when-generating-normal-material-aov-of-a-model-using-axf-shader))
    
*   HDRP: Fixed bad feedback loop occuring when auto exposure adaptation time was too small.
    
*   HDRP: Fixed banding in the volumetric clouds. (1353672)
    
*   HDRP: Fixed black pixel issue in AMD FidelityFX RCAS implementation.
    
*   HDRP: Fixed blocky looking bloom when dynamic resolution scaling was used.
    
*   HDRP: Fixed box light attenuation.
    
*   HDRP: Fixed case where the SceneView don't refresh when using LightExplorer with a running and Paused game. (1354129)
    
*   HDRP: Fixed cases in which object and camera motion vectors would cancel out, but didn't.
    
*   HDRP: Fixed Clouds on Metal or platforms that don't support RW in same shader of R11G11B10 textures.
    
*   HDRP: Fixed computation of geometric normal in path tracing (1293029)
    
*   HDRP: Fixed conflicting runtime debug menu command with an option to disable runtime debug window hotkey.
    
*   HDRP: Fixed contact shadow debug views not displaying correctly upon resizing of view.
    
*   HDRP: Fixed contact shadows tile coordinates calculations.
    
*   HDRP: Fixed controls for clouds fade in.
    
*   HDRP: Fixed corruption in player with lightmap uv when Optimize Mesh Data is enabled ([1357902](https://issuetracker.unity3d.com/issues/hdrp-materials-of-gameobjects-are-rendered-incorrectly-in-the-projects-built-application))
    
*   HDRP: Fixed CPU performance on DLSS, avoiding to recreate state whenever a target can fall into the safe min/max resolution specified by the system.
    
*   HDRP: Fixed crash on SubSurfaceScattering Editor when the selected pipeline is not HDRP
    
*   HDRP: Fixed cropping issue with the compositor camera bridge (1340549)
    
*   HDRP: Fixed custom pass custom buffer not bound after being created inside a custom pass.
    
*   HDRP: Fixed custom pass delete operation. ([1354871](https://issuetracker.unity3d.com/issues/hdrp-unable-to-remove-custom-pass-item-from-custom-pass-volume))
    
*   HDRP: Fixed custom pass volume not executed in scene view because of the volume culling mask.
    
*   HDRP: Fixed custom pass workflow for single camera effects.
    
*   HDRP: Fixed custom post process name not displayed correctly in GPU markers.
    
*   HDRP: Fixed custom post process template not working with Blit method.
    
*   HDRP: Fixed CustomPassUtils scaling issues when used with RTHandles allocated from a RenderTexture.
    
*   HDRP: Fixed CustomPassUtils.Copy function not working on depth buffers.
    
*   HDRP: Fixed decal draw order for ShaderGraph decal materials.
    
*   HDRP: Fixed Decal's pivot edit mode 2D slider gizmo not supporting multi-edition.
    
*   HDRP: Fixed Decal's UV edit mode with negative UV.
    
*   HDRP: Fixed decals in material debug display.
    
*   HDRP: Fixed diffusion profile being reset to default on SpeedTree8 materials with subsurface scattering enabled during import.
    
*   HDRP: Fixed diffusion profile breaking after upgrading HDRP ([1337892](https://issuetracker.unity3d.com/issues/hdrp-diffusion-profile-materials-get-corrupted-on-upgrade))
    
*   HDRP: Fixed diffusion profile displayed in the inspector.
    
*   HDRP: Fixed disabled menu item for volume additional properties.
    
*   HDRP: Fixed distortion when resizing the graphics compositor window in builds. ([1328968](https://issuetracker.unity3d.com/issues/view-inside-the-build-is-distorted-when-using-the-graphics-compositor-and-resizing-the-window))
    
*   HDRP: Fixed Dof, would sometimes get corrupted when DLSS was on caused by TAA logic accidentally being on for DOF. ([1357722](https://issuetracker.unity3d.com/issues/dlss-with-custom-quality-modes-produces-unexpected-results-and-causes-artifacts-in-game-view-with-depth-of-field-enabled))
    
*   HDRP: Fixed double camera preview.
    
*   HDRP: Fixed double contribution from the clear coat when having SSR or RTR on the Lit and StackLit shaders. ([1352424](https://issuetracker.unity3d.com/issues/raytraced-reflections-are-not-realistic-with-coat-mask))
    
*   HDRP: Fixed edge bleeding when rendering volumetric clouds.
    
*   HDRP: Fixed EmissiveLighting Debug Light mode not managing correctly emissive for unlit.
    
*   HDRP: Fixed enabling a lensflare in playmode.
    
*   HDRP: Fixed error in the RTHandle scale of Depth Of Field when TAA is enabled.
    
*   HDRP: Fixed error when disabling opaque objects on a camera with MSAA.
    
*   HDRP: Fixed error with motion blur and small render targets.
    
*   HDRP: Fixed exposure issues with volumetric clouds on planar reflection.
    
*   HDRP: Fixed exposure not being properly handled in ray tracing performance (RTGI and RTR). (1346383)
    
*   HDRP: Fixed fabric IBL (Charlie) pre-convolution performance and accuracy (uses 1000x less samples and is closer match with the ground truth).
    
*   HDRP: Fixed failures on platforms that do not support ray tracing due to an engine behavior change.
    
*   HDRP: Fixed for allowing to change dynamic resolution upscale filter via script.
    
*   HDRP: Fixed for discrepancies in intensity and saturation between screen space refraction and probe refraction.
    
*   HDRP: Fixed for wrong cached area light initialization.
    
*   HDRP: Fixed Force RGBA16 when scene filtering is active. (1228736)
    
*   HDRP: Fixed GBuffer clear option in FrameSettings not working.
    
*   HDRP: Fixed gbuffer depth debug mode for materials not rendered during the prepass.
    
*   HDRP: Fixed GC allocations from XR occlusion mesh when using multipass.
    
*   HDRP: Fixed ghosting issues if the exposure changed too much (RTGI).
    
*   HDRP: Fixed gizmo rendering when wireframe mode is selected.
    
*   HDRP: Fixed HDAdditionalLightData's CopyTo and HDAdditionalCameraData's CopyTo missing copy.
    
*   HDRP: Fixed HDRP material being constantly dirty.
    
*   HDRP: Fixed HDRP material upgrade failing when there is a texture inside the builtin resources assigned in the material. ([1339865](https://issuetracker.unity3d.com/issues/copying-file-failed-copying-resources-slash-unity-builtin-extra-to-temp-slash-copyassets-slash-unity-builtin-extra))
    
*   HDRP: Fixed HDRP's ShaderGraphVersion migration management which was broken.
    
*   HDRP: Fixed impossibility to release the cursor in the template.
    
*   HDRP: Fixed incorrect debug wireframe overlay on tessellated geometry (using littessellation), caused by the picking pass using an incorrect camera matrix.
    
*   HDRP: Fixed incorrect light list indexing when TAA is enabled. ([1352444](https://issuetracker.unity3d.com/issues/hdrp-planar-reflections-flicker-from-a-distance-when-taa-is-enabled))
    
*   HDRP: Fixed incorrect RTHandle scale in DoF when TAA is enabled.
    
*   HDRP: Fixed infinite propagation of nans for RTGI and SSGI. ([1349738](https://issuetracker.unity3d.com/issues/setting-particle-emission-intensity-to-infinity-makes-the-whole-scene-view-black))
    
*   HDRP: Fixed Intensity Multiplier not affecting realtime global illumination.
    
*   HDRP: Fixed invalid cast exception on HDProbe.
    
*   HDRP: Fixed invalid pass index 1 in DrawProcedural error.
    
*   HDRP: Fixed issue in Probe Reference Volume authoring component triggering an asset reload on all operations.
    
*   HDRP: Fixed issue in wizard when resource folder don't exist.
    
*   HDRP: Fixed issue of accessing default frame setting stored in current HDRPAsset instead fo the default HDRPAsset.
    
*   HDRP: Fixed issue that caused a rebake of Probe Volume Data to see effect of changed normal bias.
    
*   HDRP: Fixed issue were the final image is inverted in the Y axis. Occurred only on final Player (non-dev for any platform) that use Dynamic Resolution Scaling with Contrast Adaptive Sharpening filter.
    
*   HDRP: Fixed issue were the final image is inverted in the Y axis. Occurred only on final Player (non-dev for any platform) that use Dynamic Resolution Scaling with Contrast Adaptive Sharpening filter.
    
*   HDRP: Fixed issue when debug full screen 'Transparent Screen Space Reflection' do not take in consideration debug exposure
    
*   HDRP: Fixed issue when switching between non-persistent cameras when path tarcing is enabled. ([1337843](https://issuetracker.unity3d.com/issues/hdrp-dxr-game-view-becomes-black-when-switching-between-cameras-while-path-tracing-is-enabled))
    
*   HDRP: Fixed issue with a compute dispatch being with 0 threads on extremely small resolutions.
    
*   HDRP: Fixed issue with an assert getting triggered with OnDemand shadows.
    
*   HDRP: Fixed issue with automatic exposure settings not updating scene view.
    
*   HDRP: Fixed issue with change in lens model (perfect or imperfect) wouldn't be taken into account unless the HDRP asset was rebuilt.
    
*   HDRP: Fixed issue with constant buffer being stomped on when async tasks run concurrently to shadows.
    
*   HDRP: Fixed issue with Depth of Field CoC debug view.
    
*   HDRP: Fixed issue with depth slope scale depth bias when a material uses depth offset.
    
*   HDRP: Fixed issue with fading in SSR applying fade factor twice, resulting in darkening of the image in the transition areas.
    
*   HDRP: Fixed issue with faulty shadow transition when view is close to an object under some aspect ratio conditions
    
*   HDRP: Fixed issue with gbuffer debug view when virtual texturing is enabled.
    
*   HDRP: Fixed issue with hierarchy object filtering.
    
*   HDRP: Fixed issue with history buffer allocation for AOVs when the request does not come in first frame.
    
*   HDRP: Fixed issue with NaNs in Volumetric Clouds on some platforms.
    
*   HDRP: Fixed issue with on-demand directional shadow maps looking broken when a reflection probe is updated at the same time.
    
*   HDRP: Fixed issue with physically-based DoF computation and transparent materials with depth-writes ON.
    
*   HDRP: Fixed issue with RAS build fail when LOD was missing a renderer.
    
*   HDRP: Fixed issue with shadow mask and area lights.
    
*   HDRP: Fixed issue with the LayerMaskParameter class storing an erroneous mask value. ([1345515](https://issuetracker.unity3d.com/issues/hdrp-dxr-a-gameobject-is-not-rendered-when-its-layer-is-4th-or-higher-and-path-tracing-layer-mask-has-one-layer-disabled))
    
*   HDRP: Fixed issue with velocity rejection when using physically-based DoF.
    
*   HDRP: Fixed issue with vertex color defaulting to 0.0 when not defined, in ray/path tracing. ([1348821](https://issuetracker.unity3d.com/issues/hdrp-probuilder-meshs-texture-disappears-after-enabling-path-tracing))
    
*   HDRP: Fixed label style in pbr sky editor.
    
*   HDRP: Fixed LayerMask editor for volume parameters.
    
*   HDRP: Fixed lens flare not rendering correctly with TAAU or DLSS.
    
*   HDRP: Fixed lens flare occlusion issues with TAA.
    
*   HDRP: Fixed lens flare occlusion issues with transparent depth. It had the wrong depth bound. (1365098)
    
*   HDRP: Fixed light anchor min distance value + properties not working with prefabs. (1345509)
    
*   HDRP: Fixed light gizmo showing shadow near plane when shadows are disabled.
    
*   HDRP: Fixed light layer issue when performing editing on multiple lights.
    
*   HDRP: Fixed LightCluster debug view for ray tracing.
    
*   HDRP: Fixed lights shadow frustum near and far planes.
    
*   HDRP: Fixed LookDev environment library assignement after leaving playmode.
    
*   HDRP: Fixed material inspector that allowed setting intensity to an infinite value.
    
*   HDRP: Fixed material keywords with fbx importer.
    
*   HDRP: Fixed memory leak with XR combined occlusion meshes.
    
*   HDRP: Fixed migration step overriden by data copy when creating a HDRenderPipelineGlobalSettings from a HDRPAsset.
    

*   HDRP: Fixed misc TAA issue: Slightly improved TAA flickering, Reduced ringing of TAA sharpening, tweak TAA High quality central color filtering.
    
*   HDRP: Fixed misleading text and improving the eye scene material samples. ([1368665](https://issuetracker.unity3d.com/issues/hdrp-missmatch-of-information-in-eye-sample-project))
    
*   HDRP: Fixed missing API documentation for LTC area light code.
    
*   HDRP: Fixed missing BeginCameraRendering call for custom render mode of a Camera.
    
*   HDRP: Fixed missing context menu for "Post Anti-Aliasing" in Camera. (1357283)
    
*   HDRP: Fixed missing DisallowMultipleComponent annotations in HDAdditionalReflectionData and HDAdditionalLightData. (1365879)
    
*   HDRP: Fixed missing global wind parameters in the visual environment.
    
*   HDRP: Fixed Missing lighting quality settings for SSGI. (1312067)
    
*   HDRP: Fixed missing option to use POM on emissive for tessellated shaders.
    
*   HDRP: Fixed missing Update in Wizard's DXR Documentation.
    
*   HDRP: Fixed model import by adding additional data if needed.
    
*   HDRP: Fixed motion vector for custom meshes loaded from compute buffer in shader graph (like Hair).
    
*   HDRP: Fixed multi cameras using cloud layers shadows.
    
*   HDRP: Fixed multicamera rendering for Dynamic Resolution Scaling using dx12 hardware mode. Using a planar reflection probe (another render camera) should be safe.
    
*   HDRP: Fixed multiple any hit occuring on transparent objects. ([1294927](https://issuetracker.unity3d.com/issues/dxr-ray-traced-shadows-cast-by-semi-transparent-objects-receive-artifacts))
    
*   HDRP: Fixed multiple HDRP Frame Settings panel issues: missing "Refraction" Frame Setting. Fixing ordering of Rough Distortion, it should now be under the Distortion setting.
    
*   HDRP: Fixed normals provided in object space or world space, when using double sided materials.
    
*   HDRP: Fixed null reference exception in Raytracing SSS volume component.
    
*   HDRP: Fixed nullref in layered lit shader editor.
    
*   HDRP: Fixed nullref when enabling fullscreen passthrough in HDRP Camera.
    
*   HDRP: Fixed object outline flickering with TAA.
    
*   HDRP: Fixed objects disappearing from Lookdev window when entering playmode. (1309368)
    
*   HDRP: Fixed off by 1 error when calculating the depth pyramid texture size when DRS is on.
    
*   HDRP: Fixed overdraw in custom pass utils blur and Copy functions ([1333648](https://issuetracker.unity3d.com/issues/hdrp-custom-pass-utils-function-blit-two-full-screen-triangles-instead-of-one))
    
*   HDRP: Fixed override camera rendering custom pass API aspect ratio issue when rendering to a render texture.
    
*   HDRP: Fixed parameter ranges in HDRP Asset settings.
    
*   HDRP: Fixed path traced subsurface scattering for transmissive surfaces. (1329403)
    
*   HDRP: Fixed path traced transparent unlit material ([1335500](https://issuetracker.unity3d.com/issues/hdrp-unlit-transparent-material-shows-multiple-reflection-of-the-same-gameobject-and-itself-when-path-tracing-is-enabled))
    
*   HDRP: Fixed path tracing accumulation not being reset when changing to a different frame of an animation.
    
*   HDRP: Fixed PCSS filtering issues with cached shadow maps.
    
*   HDRP: Fixed performance issue with ShaderGraph and Alpha Test.
    
*   HDRP: Fixed Pixel Displacement that could be set on tessellation shader while it's not supported.
    
*   HDRP: Fixed pixelated appearance of Contrast Adaptive Sharpen upscaler and several other issues when Hardware DRS is on.
    
*   HDRP: Fixed possible QNANS during first frame of SSGI, caused by uninitialized first frame data.
    
*   HDRP: Fixed potential NaN on apply distortion pass.
    
*   HDRP: Fixed Probe volume debug exposure compensation to match the Lighting debug one.
    
*   HDRP: Fixed pyramid color being incorrect when hardware dynamic resolution is enabled.
    
*   HDRP: Fixed ray traced reflections that were too dark for unlit materials. Reflections are now more consistent with the material emissiveness.
    
*   HDRP: Fixed Realtime lightmap not working correctly in player with various lit shader.
    
*   HDRP: Fixed recursive rendering transmittance over the sky. (1323945)
    
*   HDRP: Fixed reflection probes being injected into the ray tracing light cluster even if not baked ([1329083](https://issuetracker.unity3d.com/issues/editor-crashes-on-gfxdeviced3d12base-drawbufferscommon-when-switching-between-scenes))
    
*   HDRP: Fixed register spilling on FXC in light list shaders.
    
*   HDRP: Fixed regression in the ambient probe intensity for volumetric clouds.
    
*   HDRP: Fixed regression in the clouds presets.
    
*   HDRP: Fixed remapping of depth pyramid debug view.
    
*   HDRP: Fixed remove of the Additional Camera Data when removing the Camera Component.
    
*   HDRP: Fixed remove of the Additional Light Data when removing the Light Component.
    
*   HDRP: Fixed Render Graph Debug UI not refreshing correctly in the Render Pipeline Debugger.
    
*   HDRP: Fixed Render Graph Debug UI not refreshing correctly in the Rendering Debugger.
    
*   HDRP: Fixed rendering of objects just after the TAA pass (before post process injection point).
    
*   HDRP: Fixed ResourceReloader that was not call anymore at pipeline construction.
    
*   HDRP: Fixed Rough Distortion frame setting not greyed out when Distortion is disabled in HDRP Asset.
    
*   HDRP: Fixed rounding issue when accessing the color buffer in the DoF shader.
    
*   HDRP: Fixed sceneview debug mode rendering. ([1211436](https://issuetracker.unity3d.com/issues/hdrp-terrain-is-not-visible-in-baked-lightmap-scene-debug-view))
    
*   HDRP: Fixed screen being over-exposed when changing very different skies.
    
*   HDRP: Fixed screen-space shadows with XR single-pass and camera relative rendering. ([1348260](https://issuetracker.unity3d.com/issues/xr-sdk-openxr-hdrp-screen-space-shadows-dont-align-when-single-pass-instanced-stereo-rendering-mode-is-used))
    
*   HDRP: Fixed Shader advanced options for lit shaders.
    
*   HDRP: Fixed shadow matte not working with ambient occlusion when MSAA is enabled
    
*   HDRP: Fixed shadow sampling artifact when using the spot light shadow option 'custom spot angle'.
    
*   HDRP: Fixed shadowmask editable when not supported.
    
*   HDRP: Fixed side effect on styles during compositor rendering.
    
*   HDRP: Fixed silhouette issue with emissive decals.
    
*   HDRP: Fixed skybox for ortho cameras.
    
*   HDRP: Fixed some aliasing ussues with the volumetric clouds.
    
*   HDRP: Fixed some depth comparison instabilities with volumetric clouds.
    
*   HDRP: Fixed some labels being clipped in the Render Graph Viewer
    
*   HDRP: Fixed some of the extreme ghosting in DLSS by using a bit mask to bias the color of particles. VFX tagged as Exclude from TAA will be on this pass.
    
*   HDRP: Fixed some reference to old frame settings names in HDRP Wizard.
    
*   HDRP: Fixed some render texture leaks.
    
*   HDRP: Fixed some resolution aliasing for physically based depth of field. (1340551)
    
*   HDRP: Fixed sorting for mesh decals.
    
*   HDRP: Fixed spacing on LayerListMaterialUIBlock.
    
*   HDRP: Fixed specular anti aliasing for layeredlit shader.
    
*   HDRP: Fixed specular occlusion sharpness and over darkening at grazing angles.
    
*   HDRP: Fixed spot light radius not changed when editing the inner or outer angle of a multi selection. ([1345264](https://issuetracker.unity3d.com/issues/same-radius-value-is-overwritten-to-all-of-the-selected-lights-when-outer-or-inner-angle-value-is-changed-while-multi-editing))
    
*   HDRP: Fixed SSGI frame setting not greyed out while SSGI is disabled in HDRP Asset.
    
*   HDRP: Fixed SSR Accumulation with Offset with Viewport Rect Offset on Camera.
    
*   HDRP: Fixed SSR Precision for 4K Screen.
    
*   HDRP: Fixed SSS on console platforms.
    
*   HDRP: Fixed sub-shadow rendering for cached shadow maps.
    
*   HDRP: Fixed support for instanced motion vector rendering.
    
*   HDRP: Fixed support for light/shadow dimmers (volumetric or not) in path tracing.
    
*   HDRP: Fixed support for ray binning for ray tracing in XR (case ). (1346374)
    
*   HDRP: Fixed support of directional light coloring from physical sky in path tracing.
    
*   HDRP: Fixed support of Distortion with MSAA
    
*   HDRP: Fixed support of multi-editing on custom pass volumes.
    
*   HDRP: Fixed TAA upsampling algorithm, now work properly.
    
*   HDRP: Fixed TAA upsampling algorithm, now work properly.
    
*   HDRP: Fixed tessellation displacement with planar mapping.
    
*   HDRP: Fixed texture fields for volume parameters accepting textures with wrong dimensions.
    
*   HDRP: Fixed the APV UI loosing focus when the helpbox about baking appears in the probe volume.
    
*   HDRP: Fixed the camera near plane not being taken into account when rendering the clouds. (1353548)
    
*   HDRP: Fixed the clouds missing in the ambient probe and in the static and dynamic sky.
    
*   HDRP: Fixed the double sided option moving when toggling it in the material UI (1328877)
    
*   HDRP: Fixed the earth curvature not being properly taken into account when evaluating the sun attenuation. (1357927)
    
*   HDRP: Fixed the emissive being overriden by ray traced sub-surface scattering.
    
*   HDRP: Fixed the fallback sun for volumetric clouds having a non null intensity. ([1353955](https://issuetracker.unity3d.com/issues/volumetric-clouds-illuminated-when-no-directional-lights-are-present-in-the-scene))
    
*   HDRP: Fixed the fallback to custom went changing a quality settings not workings properly (1338657)
    
*   HDRP: Fixed the FreeCamera and SimpleCameraController mouse rotation unusable at low framerate. (1352679)
    
*   HDRP: Fixed the incorrect value written to the VT feedback buffer when VT is not used.
    
*   HDRP: Fixed the LensFlare flicker with TAA on SceneView. ([1356734](https://issuetracker.unity3d.com/issues/flickering-for-partially-occluded-lens-flares))
    
*   HDRP: Fixed the missing parameter to control the sun light dimmer. (1364152)
    
*   HDRP: Fixed the performance of the volumetric clouds in non-local mode when large occluders are on screen.
    
*   HDRP: Fixed the possibility to hide custom pass from the create menu with the HideInInspector attribute.
    
*   HDRP: Fixed the ray traced sub subsurface scattering debug mode not displaying only the RTSSS Data (1332904)
    
*   HDRP: Fixed the RTAO debug view being broken.
    
*   HDRP: Fixed the shader graph files that was still dirty after the first save. ([1342039](https://issuetracker.unity3d.com/issues/hdrp-sg-new-graph-remains-dirty-after-the-first-save))
    
*   HDRP: Fixed the sun leaking from behind fully opaque clouds.
    
*   HDRP: Fixed the transparent cutoff not working properly in semi-transparent and color shadows. (1340234)
    
*   HDRP: Fixed the various history buffers being discarded when the fog was enabled/disabled. (1316072)
    
*   HDRP: Fixed the volume not being assigned on some scene templates.
    
*   HDRP: Fixed the volumetric clouds cloud map not being centered over the world origin.
    
*   HDRP: Fixed the volumetric clouds having no control over the vertical wind. (1354920)
    
*   HDRP: Fixed ThreadMapDetail to saturate AO & smoothness strength inputs to prevent out-of-bounds values set by users. (1357740)
    
*   HDRP: Fixed tiled artifacts in refraction at borders between two reflection probes.
    
*   HDRP: Fixed timing issues with accumulation motion blur
    
*   HDRP: Fixed undo of some properties on light editor.
    
*   HDRP: Fixed undo on light anchor.
    
*   HDRP: Fixed undo-redo on layered lit editor.
    
*   HDRP: Fixed Undo/Redo instability of light temperature.
    
*   HDRP: Fixed unexpected rendering of 2D cookies when switching from Spot to Point light type ([1333947](https://issuetracker.unity3d.com/issues/hdrp-non-descriptive-errors-and-unexpected-rendering-when-unsupported-texture-type-is-assigned-as-a-cookie))
    
*   HDRP: Fixed unexpectedly strong contribution from directional lights in path-traced volumetric scattering. (1304688)
    
*   HDRP: Fixed update order in Graphics Compositor causing jumpy camera updates. ([1345566](https://issuetracker.unity3d.com/issues/gameobject-culled-in-the-graphics-compositor-is-jumpy-when-the-main-camera-moves-too-fast))
    
*   HDRP: Fixed update upon light movement for directional light rotation.
    
*   HDRP: Fixed usage of Panini Projection with floating point HDRP and Post Processing color buffers.
    
*   HDRP: Fixed various issues with non-temporal SSAO and rendergraph.
    
*   HDRP: Fixed various SSGI issues. (1327919, [1339297](https://issuetracker.unity3d.com/issues/hdrp-gameobjects-sides-not-affected-by-directional-light-are-pitch-black-when-ssgi-is-used), [1340851](https://issuetracker.unity3d.com/issues/hdrp-ghosting-artifacts-are-shown-in-the-game-view-when-ssgi-is-enabled))
    
*   HDRP: Fixed Vertex Color Mode documentation for layered lit shader.
    
*   HDRP: Fixed VFX flag "Exclude From TAA" not working for some particle types.
    
*   HDRP: Fixed VfX lit particle AOV output color space.
    
*   HDRP: Fixed viewport size when TAA is executed after dynamic res upscale. (1348541)
    
*   HDRP: Fixed volume interpolation issue with ScalableSettingLevelParameter.
    
*   HDRP: Fixed Volumetric Clouds not updated when using RenderTexture as input for cloud maps.
    
*   HDRP: Fixed volumetric fog being visually chopped or missing when using hardware Dynamic Resolution Scaling.
    
*   HDRP: Fixed volumetric fog being visually chopped or missing when using hardware Dynamic Resolution Scaling.
    
*   HDRP: Fixed volumetric fog in planar reflections.
    
*   HDRP: Fixed warning "Releasing render texture that is set to be RenderTexture.active!" on pipeline disposal / hdrp live editing.
    
*   HDRP: Fixed warning fixed on ShadowLoop include (HDRISky and Unlit+ShadowMatte).
    
*   HDRP: Fixed Warnings about "SceneIdMap" missing script in eye material sample scene
    
*   HDRP: Fixed white flash when camera is reset and SSR Accumulation mode is on.
    
*   HDRP: Fixed white flash with SSR when resetting camera history. (1335263)
    
*   HDRP: Fixed white flashes on camera cuts on volumetric fog.
    
*   HDRP: Fixed white flashes when history is reset due to changes on type of upsampler.
    
*   HDRP: Fixed wizard checking FrameSettings not in HDRP Default Settings.
    
*   HDRP: Fixed wobbling/tearing-like artifacts with SSAO.
    
*   HDRP: Fixed WouldFitInAtlas that would previously return wrong results if any one face of a point light would fit (it used to return true even though the light in entirety wouldn't fit).
    
*   HDRP: Fixed wrong color buffer being bound to pre refraction custom passes.
    
*   HDRP: Fixed wrong LUT initialization in Wireframe mode.
    
*   HDRP: Fixed wrong ordering in FrameSettings (Normalize Reflection Probes).
    
*   HDRP: Fixed XR depth copy ([1286908](https://issuetracker.unity3d.com/issues/xr-sdk-hdrp-depth-buffer-is-not-properly-copied-for-each-view-when-two-pass-rendering-mode-is-used))
    
*   HDRP: Fixed XR depth copy when using MSAA.
    
*   HDRP: Generating a GUIContent with an Icon instead of making MaterialHeaderScopes drawing a Rect every time.
    
*   HDRP: HDRP Wizard can still be opened from Windows >; Rendering, if the project is not using a Render Pipeline.
    
*   HDRP: Indentation of the HDRenderPipelineAsset inspector UI for quality.
    
*   HDRP: MaterialReimporter.ReimportAllMaterials and MaterialReimporter.ReimportAllHDShaderGraphs now batch the asset database changes to improve performance.
    
*   HDRP: Mitigate ghosting / overbluring artifacts when TAA and physically-based DoF are enabled by adjusting the internal range of blend factor values. (1340541)
    
*   HDRP: Only display HDRP Camera Preview if HDRP is the active pipeline. (1350767)
    
*   HDRP: Prevent any unwanted light sync when not in HDRP. ([1217575](https://issuetracker.unity3d.com/issues/hdrp-switching-from-hdrp-to-urp-causes-all-lights-to-have-their-intensity-reset-upon-entering-play-mode))
    
*   HDRP: Prevented user from spamming and corrupting installation of nvidia package.
    
*   HDRP: Reduced the number shader variants for the volumetric clouds.
    
*   HDRP: Reduced the volumetric clouds pattern repetition frequency. (1358717)
    
*   HDRP: Removed DLSS keyword in settings search when NVIDIA package is not installed. ([1358409](https://issuetracker.unity3d.com/issues/hidden-parameters-shouldnt-appear-in-the-search))
    
*   HDRP: Significantly improved performance of APV probe debug.
    
*   HDRP: Support undo of HDRP Global Settings asset assignation.
    
*   HDRP: The default LookDev volume profile is now copied and referenced in the Asset folder instead of the package folder.
    
*   HDRP: The HDRP Wizard is only opened when a SRP in use is of type HDRenderPipeline.
    
*   HDRP: VFX : Debug material view incorrect depth test. ([1293291](https://issuetracker.unity3d.com/issues/hdrp-vfx-debug-material-override-blending))
    
*   HDRP: VFX : Debug material view were rendering pink for albedo. (1290752)
    
*   HDRP: VFX: Fixed LPPV with lit particles in deferred. ([1293608](https://issuetracker.unity3d.com/issues/hdrp-lightprobe-vfx-doesnt-work-with-light-probe-proxy-volumes))
    
*   HDRP: Viewport and scaling of Custom post process when TAAU or DLSS are enabled. ([1352407](https://issuetracker.unity3d.com/issues/hdrp-game-view-gets-clipped-in-play-mode-when-using-custom-global-post-processing-volume-with-dlss-enabled))
    
*   HDRP: When the HDProjectSettings was being loaded on some cases the load of the ScriptableObject was calling the method `Reset` from the HDProjectSettings, simply rename the method to avoid an error log from the loading.
    
*   IL2CPP: Added support for array values as custom attribute arguments. (1174903)
    
*   IL2CPP: Allow blittable, generic value types to be marshaled as delegate parameters. ([1348863](https://issuetracker.unity3d.com/issues/il2cpp-does-not-support-marshaling-of-blittable-generic-structs))
    
*   IL2CPP: Allow the debugger to grow the frame capacity on-demand. ([1360149](https://issuetracker.unity3d.com/issues/player-crashes-when-running-a-recursive-function-with-script-debugging-enabled))
    
*   IL2CPP: Fix parsing of --custom-step command line argument to UnityLinker. ([1351726](https://issuetracker.unity3d.com/issues/it-is-not-possible-to-add-custom-linker-steps-due-to-a-problem-with-the-options-parser))
    
*   IL2CPP: Fixed "Unexpected generic parameter." exception when a generic method had a function pointer parameter. (1364482)
    
*   IL2CPP: Fixed compiler error calling Enum.GetHashCode with System.Enum arguments. ([1354855](https://issuetracker.unity3d.com/issues/il2cpp-fails-code-conversion-for-enum-dot-hasflag-case))
    
*   IL2CPP: Fixed issue that could cause finally blocks to run more than once.
    
*   IL2CPP: Fixed issue with non-ASCII characters in installation path or project path that could cause builds to fail. (1322529)
    
*   IL2CPP: Fixed issue with UnityLinker that would cause Windows Runtime assemblies to be incorrectly loaded and parsed, causing builds to fail. (1315830)
    
*   IL2CPP: Fixed UnityLinker bug that caused callvirt instruction to be removed without removing the corresponding constrained instruction. ([1297609](https://issuetracker.unity3d.com/issues/project-tiny-wasm-build-fails-with-exception-constrained-opcode-was-followed-a-call-rather-than-a-callvirt-in-method))
    
*   IL2CPP: UnityLinker will now respect --unity-root-strategy if defined on the command line. ([1351728](https://issuetracker.unity3d.com/issues/unneccessary-monobehaviours-included-because-unityrootstrategy-command-line-parameter-is-ignored))
    
*   IMGUI: Fixed an issue where custom editor without CanEditMultipleObjects attribute is not displaying the script fields. ([1279145](https://issuetracker.unity3d.com/issues/custom-editor-selected-objects-fields-not-displayed-after-selecting-multiple-objects-without-caneditmultipleobjects))
    
*   IMGUI: Fixed an issue where the layers dropdown menu window is not closed while dragging the editor window. ([1308381](https://issuetracker.unity3d.com/issues/popupwindow-stays-open-when-moving-the-editor-window))
    
*   IMGUI: Fixed Gridview image of Texture not updating in ProjectBrowser when color space is updated in PlayerSettings. ([1198127](https://issuetracker.unity3d.com/issues/preview-icons-in-project-window-are-different-from-inspector-preview-window-when-switching-between-gamma-slash-linear-color-space))
    
*   IMGUI: Fixed Project Window going blank when the objects are dragged between folders in Favourites. ([1206532](https://issuetracker.unity3d.com/issues/dragging-an-object-from-one-project-window-to-another-makes-them-blank-when-the-objects-are-dragged-between-folders-in-favorites))
    
*   IMGUI: Hide the MaterialEditor in inspector when a MeshRenderer is hidden. ([1289980](https://issuetracker.unity3d.com/issues/material-assets-settings-are-displayed-in-the-inspector-window-when-meshrenderer-component-is-hidden-in-the-scene))
    
*   iOS: Added missing API file updates.
    
*   iOS: Disabled audio output on pre-iOS14 simulators, as audio is broken here completely and causes a crash on startup. ([1325806](https://issuetracker.unity3d.com/issues/ios-cannot-run-any-unity-build-on-ios-simulator-for-ios-14-on-big-sur))
    
*   iOS: EditorUserBuildSettings.symlinkLibraries will affect sources in packages which are referenced by file tag in Packages/manifest.json (1301157)
    
*   iOS: Fixed an issue where display length is not updated when external display is disconnected. Users now can access only active displays (previously there was a possibility of caching known but inactive display indices). ([1330759](https://issuetracker.unity3d.com/issues/ios-display-dot-displays-does-not-update-when-disconnecting-a-display))
    
*   iOS: Fixed crash when performing two Microphone/WebCam permission requests at the same time. ([1330126](https://issuetracker.unity3d.com/issues/ios-crash-on-scriptinggchandle-acquire-when-calling-requestuserauthorization-without-using-yield-for-pending-authorization))
    
*   iOS: Fixed SystemInfo returning incorrect values for max compute buffer inputs on Metal ([1299759](https://issuetracker.unity3d.com/issues/metal-unity-returns-that-it-only-supports-8-compute-buffers-with-metal-graphics-api-when-it-actually-supports-32))
    
*   iOS: Fixed tweaking WebCamTexture sampler setup resulting in GPU error on older devices. ([1309523](https://issuetracker.unity3d.com/issues/ios-metal-gpu-errors-on-older-devices-when-webcamtexture-dot-wrapmode-is-set-to-clamp))
    
*   iOS: Provide Compass.headingAccuracy data. ([1338663](https://issuetracker.unity3d.com/issues/ios-input-dot-compass-dot-headingaccuracy-is-always-set-to-0))
    
*   iOS: Updated the list of available frameworks in Plugin Inspector. ([1194821](https://issuetracker.unity3d.com/issues/ios-incomplete-ios-system-framework-list-in-plugin-importers-platform-settings))
    
*   iOS: When selected XCode project build destination is not allowed (root project folder, Assets folder, etc.) warning is displayed.
    
*   Kernel: Atomic 64-bit Load/Store on Win32/UWP x86 fixed (Reads and writes to 64-bit values are not guaranteed to be atomic on 32-bit Windows).
    
*   Kernel: Fixed issue where running player with auto connect on mobile device with disabled WiFi, disabling player connection. Then any attempt to connect to device manually will fail. (1311781)
    
*   Kernel: Fixed potential crash while extracting detangled name on OSX. (1308423)
    
*   Kernel: Stop using recently deprecated timer native functions on Mac/iOS/tvOS and replace with current official recommendation.
    
*   License: Added Licensing Client version into Editor Analytics.
    
*   License: Fixed memory leak in Licensing Module.
    
*   License: Fixed serverDirectory in license server configuration file.
    
*   Linux: Added handling for Norwegian Bokmal and Nynorsk in SystemInfo for macOS and Linux, and to SystemInfo in Runtime/Misc used by WebGL and MetroPlayer.
    
*   Linux: Fix "Not Responding" dialog window opens up in the Player when the splash screen's logo duration is set to 4.65 or higher. ([1249666](https://issuetracker.unity3d.com/issues/linux-a-not-responding-dialog-window-opens-up-in-the-player-when-the-splash-screens-logo-duration-is-set-to-4-dot-65-or-higher))
    
*   Linux: Fix crash under Wayland when opening Keyboard window from New Input System debug window. (1319311)
    
*   Linux: Fix recognition of game controllers with same usd product id. ([1300415](https://issuetracker.unity3d.com/issues/linux-input-system-xbox-one-controller-is-detected-as-a-playstation-3-memory-card-adapter))
    
*   Linux: Fixed automated batch mode test from failing due to Unity exiting with error code 133 before all it's threads have shut down. (1303886)
    
*   Linux: Fixed gizmo dropdown not closing when clicking on the scene or game view. ([1289590](https://issuetracker.unity3d.com/issues/linux-scene-view-gizmos-dropdown-list-does-not-close-on-clicking-in-the-scene-view))
    
*   Linux: Fixed inspector prefab overrides window from drawing beyond the usable workarea ([1119679](https://issuetracker.unity3d.com/issues/if-the-overrides-screen-is-taller-than-screen-part-of-the-screen-goes-out-of-display))
    
*   Linux: Fixed main editor window from scrolling when using larger Gnome font sizes. (1311302)
    
*   Linux: Fixed main menu disappearing after certain layout change events. ([1362449](https://issuetracker.unity3d.com/issues/xr-linux-editor-menu-disappears-when-opening-new-ar-or-vr-template-project-or-when-pressing-show-tutorials))
    
*   Linux: Fixed mismatch BeginSample/EndSample profiler errors when using a modal file save dialog while profiling. ([1322750](https://issuetracker.unity3d.com/issues/linux-profiler-missing-profiler-endsample-errors-thrown-clicking-cancel-button-the-save-current-profiling-information-windows))
    
*   Linux: Fixed mismatch profiler BeginSample/EndSample errors when interacting with a modal dialog while the profiler is active in Editor mode. ([1306180](https://issuetracker.unity3d.com/issues/linux-non-matching-profiler-error-thrown-on-clicking-the-restore-defaults-option-when-target-selection-is-editor))
    
*   Linux: Fixed mouse clicks incrementing scroll x/y. ([1308873](https://issuetracker.unity3d.com/issues/linux-inputsystem-mouse-button-clicks-interpreted-as-vertical-scrollwheel-inputs))
    
*   Linux: Fixed plugin header files not being copied to the editor installer. (1345891)
    
*   Linux: Fixed shifted key events in the old input system. (1316748)
    
*   Linux: Input when using WASD does not get stuck when using the shift key in Play Mode. ([1333044](https://issuetracker.unity3d.com/issues/linux-input-system-pressandrelease-trigger-behavior-causes-unexpected-behavior-when-in-play-mode))
    
*   Linux: Keep the window that had focus last in focus after a modal dialog closes. ([1319180](https://issuetracker.unity3d.com/issues/linux-profiler-module-editor-window-gets-closed-when-deleting-a-custom-profiler-module))
    
*   Linux: Keyboard API now correctly displays non-US keyboard displaynames when using Keyboard.current.<;key>;.displayName ([1266943](https://issuetracker.unity3d.com/issues/inputsystem-keyboard-dot-current-dot-akey-dot-displayname-returns-an-incorrect-value-when-using-a-french-keyboard-with-french-locale))
    
*   Linux: Made updates to min/max size blocking if it results in a resized window to help ensure a window is ready after it's size has been changed. (1319323)
    
*   Linux: Make GUIViews obey the min/max constraints of the window they are in. ([1327222](https://issuetracker.unity3d.com/issues/linux-popup-windows-are-not-able-to-shrink))
    
*   Linux: NullReferenceException no longer appears when clicking the "Setting icon" under the "Profiler Module" dropdown. ([1290647](https://issuetracker.unity3d.com/issues/linux-profiler-nullreferenceexception-appear-on-clicking-the-setting-icon-under-the-profiler-module-dropdown))
    
*   Linux: Removed broken gamepad auto mapping from SDL 2.0.14. (1322165)
    
*   Linux: Updated from SDL 2.0.12 to 2.0.14
    
*   macOS: Added support for Apple silicon Editor plugins. Fixed error where x64 plugins report a naming conflict with Apple silicon plugins. ([1332566](https://issuetracker.unity3d.com/issues/plugin-inspector-in-the-editor-doesnt-allow-selecting-cpu-architecture-for-editor-plugins))
    
*   macOS: Dock is no longer ignored when exiting fullscreen and moving the window ([1354879](https://issuetracker.unity3d.com/issues/macos-movemainwindowto-ignores-dock-space-when-changing-resolution-and-moving-app-to-given-coordinates-from-fullscreen-mode))
    
*   macOS: Fix Screen.resolutions refreshRate property. ([1284854](https://issuetracker.unity3d.com/issues/macos-wrong-refresh-rate-is-returned-on-macbook-pro-2019-when-using-screen-dot-resolution-method))
    
*   macOS: Fixed a bug related to 8 monitors connected at one time. ([1272030](https://issuetracker.unity3d.com/issues/osx-player-with-8-displays-connected-returns-0-connected-displays-with-uninitialized-displaydevice-on-default-display))
    
*   macOS: Fixed crash if user unplugs a secondary display while running player. (1325384)
    
*   macOS: Fixed IMGUI mouse position when using the New Input System. ([1298110](https://issuetracker.unity3d.com/issues/input-system-does-not-set-the-correct-mouse-position-in-the-mac-standalone-build))
    
*   macOS: Fixed incorrect workArea size when changing the dock at runtime. ([1354356](https://issuetracker.unity3d.com/issues/mac-displayinfo-dot-workarea-ignores-changes-to-dock-size-at-runtime))
    
*   macOS: Fixed incorrect workArea size when changing the screen scaling at runtime. ([1354329](https://issuetracker.unity3d.com/issues/macos-displayinfo-dot-workarea-is-incorrect-after-scaling-any-display-while-having-app-in-fullscreen-mode))
    
*   macOS: Fixed Input.inputString doesn't convert input to the suggestions from IME. ([1305843](https://issuetracker.unity3d.com/issues/macos-linux-input-dot-inputstring-doesnt-convert-input-to-the-suggestions-from-ime))
    
*   macOS: Fixed Input.inputString not updating when cmd key is held down ([1296862](https://issuetracker.unity3d.com/issues/macos-no-input-when-meta-key-is-pressed-down-with-another-key-in-build))
    
*   macOS: Fixed install path regression that resulted in iOS support not being able to be installed. (1337753)
    
*   macOS: Fixed memory leak in HDR Display related code
    
*   macOS: Fixed scene view lagging when the tile palette window was focused. ([1316068](https://issuetracker.unity3d.com/issues/macos-2d-tile-placement-lags-when-editor-is-not-focused))
    
*   macOS: Fixed Screen.currentResolution when Mac Retina Support Player Setting is off. ([1286140](https://issuetracker.unity3d.com/issues/mac-retina-support-setting-is-not-disabled-when-display-resolution-dialogue-is-disabled))
    
*   macOS: Force to use GPU Lightmapper instead of CPU Lightmapper on Apple silicon. ([1341489](https://issuetracker.unity3d.com/issues/m1-crash-when-baking-with-cpu-lightmapper-on-apple-silicon-machine))
    
*   macOS: If running under Rosetta 2, <;Rosetta>; will appear in the title bar next to the graphics mode. ([1329708](https://issuetracker.unity3d.com/issues/macos-there-is-no-way-to-tell-if-you-are-running-under-rosetta))
    
*   macOS: We now log basic system information when launching the Editor to the log file.
    
*   macOS: We now prompt for to save changes even when the window is minimized. ([1320569](https://issuetracker.unity3d.com/issues/macos-editor-doesnt-show-unsaved-changes-pop-up-if-editor-is-being-closed-when-window-with-unsaved-changes-is-minimized))
    
*   macOS: When selected XCode project build destination is not allowed (root project folder, Assets folder, etc.) warning is displayed.
    
*   Mobile: No more MSAA and Pixel Light count warnings when building URP on Mobile platforms ([1300605](https://issuetracker.unity3d.com/issues/ios-using-more-than-1-pixel-lights-on-a-mobile-device-warning-is-thrown-when-building-urp-project-with-high-quality-setting))
    
*   Mobile: Show provider icon and info text correctly.
    
*   Mono: Added missing facade dlls for Unity profiles. ([1367105](https://issuetracker.unity3d.com/issues/dot-netstandard-2-dot-1-in-the-editor-is-missing-system-dot-memory-system-dot-buffers-at-runtime))
    
*   Mono: Assembly.Load now loads distinct assemblies correctly. ([1073523](https://issuetracker.unity3d.com/issues/calling-the-loadassembly-method-does-not-load-the-given-assembly))
    
*   Mono: Fixed "Loading assembly failed. File does not contain a valid CIL image" errors. ([1336618](https://issuetracker.unity3d.com/issues/managed-assembly-load-failure))
    
*   Mono: Fixed FileSystemEventArgs.Name to be a relative path. ([1344552](https://issuetracker.unity3d.com/issues/filesystemwatcher-filesystemwatcherargs-dot-name-variable-is-returning-the-full-file-path-instead-of-the-relative-file-name))
    
*   Mono: Fixed issue in the mono web request stack where it would incorrectly wait on the Unity synchronization context for an asynchronous call to complete leading to the request being aborted on timeout. (1338465)
    
*   Mono: Fixed issue where the timeout of a HttpClient handler was not being used for requests. ([1365107](https://issuetracker.unity3d.com/issues/timeout-value-does-not-propagate-when-using-a-delegatinghandler-as-the-main-httpclient-handler))
    
*   Mono: Fixed missing .NET Standard 2.1 assemblies (System.Memory, System.Buffers...). ([1367105](https://issuetracker.unity3d.com/issues/dot-netstandard-2-dot-1-in-the-editor-is-missing-system-dot-memory-system-dot-buffers-at-runtime))
    
*   Mono: Fixed regression where a MissingMethodException would be thrown when IsComObject was called. ([1346334](https://issuetracker.unity3d.com/issues/mono-upgrade-missingmethodexception-thrown-when-attempting-to-use-iscomobject))
    
*   Mono: Prevent unnecessary files from being copied into the Managed directory when managed code stripping is enabled. ([1302474](https://issuetracker.unity3d.com/issues/unitylinker-files-are-left-in-the-build-directory-when-building-the-project-with-mono-backend))
    
*   Multiplayer: Marked uNET HLAPI as deprecated.
    
*   N/A (internal): Fixed exception caused by EmbeddedLinuxPreProcessor, by only executing checks when EmbeddedLinux platform is selected.  
    Fixes the removal of unneeded EmbeddedLinux support files (e.g. unstripped debug symbols), to minimize the resulting archive size.
    
*   N/A (internal): Fixed native test instability CanLoadMesh. (1330725)
    
*   Networking: mbed tls High Vulnerable reported on the Unity 2019.4 LTS Stream for iOS, Android and UWP by SAP. (1370568)
    
*   Networking: Security Issues for mbed tls (CVE-2020-36423, CVE-2020-36426) resolved. (1356067)
    
*   Package: (ml-agents) Removed unnecessary allocations and garbage collections during runtime.
    
*   Package: (Recorder) (macOS) Fixed an image stride issue for ProRes formats 4444 and 4444XQ.
    
*   Package: (Recorder) Do not perform the color space conversion from linear to sRGB for RenderTextures that are already sRGB.
    
*   Package: (Recorder) Ensured that the color space conversion from sRGB to linear is performed when required for EXR files
    
*   Package: (Recorder) Ensured that the Image Recorder encodes in sRGB when requested, even if the scripted render pipeline provides linear data.
    
*   Package: (Recorder) Fixed a memory leak in the AOV Recorder.
    
*   Package: (Recorder) Fixed an exception that occurred when sending a RenderTexture to a Recorder before creating this RenderTexture.
    
*   Package: (Recorder) Fixed an exception that occurred when the user performed the undo action after deleting a Recorder.
    
*   Package: (Recorder) Fixed audio recording issue when the frame interval is not starting at 0.
    
*   Package: (Recorder) Fixed invalid values in the alpha channel when performing texture sampling for different rendering and output resolutions.
    
*   Package: (Recorder) Fixed issues with the Recorder samples about synchronizing multiple recordings and resetting the Game view resolution.
    
*   Package: (Recorder) Fixed the Tagged Camera capture process to follow any camera changes that might occur.
    
*   Package: (Recorder) Fixed vertically flipped outputs on OpenGL hardware.
    
*   Package: (Recorder) Perform the appropriate color space conversion for Texture Sampling sources when required.
    
*   Package: Fixed bug that causes searcher window to be offset too far when accounting for host window boundaries.\].
    
*   Package: Visual Scripting :  
    
    *   Fixed long values not preserved in literal nodes.  
        
    *   Fixed root icons in breadcrumbs in the graph editor window.  
        
    *   Fixed graph nodes icons  
        
    *   Fixed project settings will not show when looking for graphs  
        
    *   Fixed exception when user double clicks on a graph  
        
    *   Raised warnings at edit time when a MouseEvent node is used when targeting handheld devices instead of build time.
*   Package: \[VisualScripting\] "Restore to Defaults" buttons in the Project Settings window
    
*   Package: \[VisualScripting\] Console errors when deleting a Prefab with a Visual Script
    
*   Package: \[VisualScripting\] Console errors when editing nested graphs during Play Mode
    
*   Package: \[VisualScripting\] Dropdown icon is not clipped with TextField under "Get Variable"
    
*   Package: \[VisualScripting\] Error message when custom inspectors are generated
    
*   Package: \[VisualScripting\] Error when executing "Fix Missing Scripts" in a HDRP project
    
*   Package: \[VisualScripting\] FlowMachine type is now back in usable types.
    
*   Package: \[VisualScripting\] Fuzzy finder no longer blinks when trying to add a node \[BOLT-1157\]
    
*   Package: \[VisualScripting\] Fuzzy finder search window no longer remains above all other windows \[BOLT-1197\]
    
*   Package: \[VisualScripting\] Fuzzy search no longer drops keyboard inputs and respond slowly \[BOLT-1214\]
    
*   Package: \[VisualScripting\] Generated folder is removed when removing the VisualScripting package.
    
*   Package: \[VisualScripting\] Graph getting corrupted when adding "Get Action Map" unit
    
*   Package: \[VisualScripting\] GraphPointerException occurs when nesting graph within itself \[BOLT-1257\]
    
*   Package: \[VisualScripting\] Help button in the visual scripting Assets and Behaviours inspector now link to the package documentation.
    
*   Package: \[VisualScripting\] Missing succession for Cooldown. Output of Cooldown completed is treated as unentered. \[BOLT-725\]
    
*   Package: \[VisualScripting\] Node description being sometimes clipped
    
*   Package: \[VisualScripting\] Object Variables tabs not updated when creating a Prefab
    
*   Package: \[VisualScripting\] Open the graph window no longer causes Unity UI stop processing mouse click \[BOLT-1159\]
    
*   Package: \[VisualScripting\] Preferences being searchable \[BOLT-1218\]
    
*   Package: \[VisualScripting\] Preferences spacing has been adjusted to avoid overlaps
    
*   Package: \[VisualScripting\] RenamedFrom attribute does not function correctly on array references to a renamed type \[BOLT-1149\]
    
*   Package: \[VisualScripting\] Rendering of inactive ObjectFields
    
*   Package: \[VisualScripting\] Resize cursor rect on group when graph window is zoomed
    
*   Package: \[VisualScripting\] ScalarAdd unit migration from 1.4.13 to 1.4.14 and above
    
*   Package: \[VisualScripting\] Scale groups when zoom is not at 1x
    
*   Package: \[VisualScripting\] Sidebar (graph inspector/blackboard) resize when a vertical scrollbar is needed
    
*   Package: \[VisualScripting\] ThreadAbortException when entering Play Mode while searching in the Fuzzy Finder
    
*   Package: \[VisualScripting\] Variable type reset to Enum when changing from Enum to GameObject when both Blackbaord and Variables inspector are displayed
    
*   Package: \[VisualScripting\] Warnings overflow in the console when deleting and adding a boolean variable in the blackboard
    
*   Package: \[VisualScripting\] Warnings when entering play mode when the "Script Changes While Playing" is set to Recompile And Continue Playing
    
*   Package Manager: Added an info icon will warn users when the package version they are using is not recommended for their Unity version.
    
*   Package Manager: Added missing tooltip to the refresh icon.
    
*   Package Manager: Deletion of root package folders from Project Browser is now prohibited. Users should use Package Manager Window to ensure proper removal of packages from their projects. ([1285197](https://issuetracker.unity3d.com/issues/data-loss-local-package-is-deleted-from-disk-when-it-is-removed-from-project-window))
    
*   Package Manager: Dependencies' state is automatically refreshed in the list when installed or removed by default. (1360937)
    
*   Package Manager: Documentation links are now secure or, if un-secure and not generated by Unity, a warning will show up letting users know they have to enable un-secure requests in "Player Setting". ([1356909](https://issuetracker.unity3d.com/issues/insecure-connection-is-not-allowed-error-is-shown-when-view-documentation-button-is-pressed-in-package-manager))
    
*   Package Manager: Enabled Update button for packages installed from Git, will check if any updates are available and update the Git package.
    
*   Package Manager: Errors are now automatically refreshed once packages are updated to fix the issue. (1342141)
    
*   Package Manager: Fix the button text being clipped and properties going out of panel under the foldout of Scoped Registries in Project Settings window.
    
*   Package Manager: Fixed a bug where a non-discoverable package is displayed as released on the user's Editor version. ([1335740](https://issuetracker.unity3d.com/issues/packages-under-v2-lifecycle-are-incorrectly-labeled-as-pre-release-or-release))
    
*   Package Manager: Fixed a bug where the Package Manager UI did not refresh after manually editing the package.json of an embedded package.
    
*   Package Manager: Fixed an issue where either no submodules or the wrong submodules could be cloned when using a Git-based dependency with both a path and a revision.
    
*   Package Manager: Fixed an issue where if the user has many asset store packages loaded in My Assets view, selecting the last package and scrolls up list show items with empty package name.
    
*   Package Manager: Fixed an issue where manually embedded packages from the project cache are not added in Perforce. ([1314073](https://issuetracker.unity3d.com/issues/manually-embedded-packages-are-not-added-in-perforce))
    
*   Package Manager: Fixed an issue which could sometimes cause package resolution errors due to `EMFILE` errors in projects with a large number of packaged assets.
    
*   Package Manager: Fixed an issue which could sometimes lead to missing files in successfully resolved packages in projects with a large number of packaged assets.
    
*   Package Manager: Fixed confusing error message when 'View changelog' not available (1282094)
    
*   Package Manager: Fixed random stack overflow issue when installing and uninstalling packages. (1327700)
    
*   Package Manager: Fixed sample display name error info box when package is not in development and package manager set to lowest width.
    
*   Package Manager: Fixed size of add bouton.
    
*   Package Manager: Fixed tests compilation warnings.
    
*   Package Manager: Fixed the issue when sorting by "Update date" and filtering by "Downloaded", the order of the assets is inconsistent in My Assets tab. (1343200)
    
*   Package Manager: Fixed the issue where modifying sort option breaks package list ordering in the My Assets tab. (1343198)
    
*   Package Manager: Fixed the issue where sync code is not unregistered when the Package Manager window is closed. (1368318)
    
*   Package Manager: Fixed the issue where the ads packages license link takes you to a wrong url. (1350621)
    
*   Package Manager: Fixed the issue where `Open in Unity` from the asset store website does not always work the first time. (1355418)
    
*   Package Manager: Fixed the UX issue where after a user installs a version of a package that does not match the version used after dependency resolution, it looks like the install did not happen. (1271576)
    
*   Package Manager: Hide reset feature button if the installed version is a patch of the lifecycle version. (1360446)
    
*   Package Manager: If user install same version as feature set required locally, we don't show it as customized. (1342339)
    
*   Package Manager: Implemented undo/redo in Scoped Registries Management. ([1285075](https://issuetracker.unity3d.com/issues/package-manager-undo-functionality-does-not-work-on-making-any-changes-in-scoped-registries))
    
*   Package Manager: Put a descriptive error message when open asset with different account.
    
*   Package Manager: Release Candidate packages will just be tagged as 'RC' again. Users on alpha/beta versions will no longer see packages tagged as 'Pre' if they don't have 'Enable Pre-release' setting enabled. ([1297779](https://issuetracker.unity3d.com/issues/packman-pre-release-packages-are-visible-in-package-manager-regardless-of-whether-pre-release-packages-are-enabled-or-not))
    
*   Package Manager: Show package update icon and update button when there is a latest update available. Remove update icon and update button when there is a recommended update available that is not the latest update.
    
*   Package Manager: Show proper error message when user try to download an asset he doesn't have a paid for (free asset, wrong account) ([1299159](https://issuetracker.unity3d.com/issues/packman-shows-error-unable-to-get-purchase-details-because-you-may-not-have-purchased-this-package-when-package-is-free))
    
*   Package Manager: The expanded/collapsed state of Packages folder in Project Browser will now persist on Editor restart. ([1307883](https://issuetracker.unity3d.com/issues/packages-folder-fold-slash-unfold-state-doesnt-save-between-editor-sessions))
    
*   Package Manager: There are no more missing packages in a Feature's dependencies list. ([1344819](https://issuetracker.unity3d.com/issues/packagemanager-package-is-missing-from-mobile-feature-included-packages-set))
    
*   Particles: Add texel size and mask interaction shader properties to particle system renderer. ([1296392](https://issuetracker.unity3d.com/issues/texelsize-is-always-1-for-particle-systems-renderer-when-using-shader-graph-material-which-draws-texelsize-value-in-rg-channels))
    
*   Particles: Added missing tooltips to + and - buttons. ([1332732](https://issuetracker.unity3d.com/issues/tooltip-is-missing-for-add-plus-button-in-particle-system))
    
*   Particles: Apply Start Delay to Rate over Distance emission. ([1314672](https://issuetracker.unity3d.com/issues/particle-system-start-delay-will-not-work-when-using-rate-over-distance-emmsion))
    
*   Particles: Disable error dialog for incorrect Vertex Stream setup, because it is not possible to provide accurate information. ([1304215](https://issuetracker.unity3d.com/issues/urp-infinite-vertex-streams-error-loop-appear-when-particle-sytstem-renderer-material-is-set-to-urp-slash-particles-shader))
    
*   Particles: Ensure ParticleSystem.Particle.angularVelocity gets applied properly when set via script. ([1322645](https://issuetracker.unity3d.com/issues/particles-dot-angularvelocity-function-doesnt-change-particles-angular-velocity-when-changed-via-the-script))
    
*   Particles: Fix incorrect evaluation of the end of stepped curves in Particle Systems. ([1314389](https://issuetracker.unity3d.com/issues/editor-crashes-while-openning-scene))
    
*   Particles: Fixed Mesh (+) button overlapping in Renderer Material field. ([1332484](https://issuetracker.unity3d.com/issues/add-mesh-plus-button-is-overlapping-with-material-field-for-the-particle-system))
    
*   Particles: Fixed misplaced object selector buttons under Trigger, Collision, and External Force modules. ([1331893](https://issuetracker.unity3d.com/issues/shuriken-selector-buttons-of-properties-are-misplaced-under-trigger-collision-and-external-force-modules))
    
*   Particles: Fixed orientation of GPU instanced mesh particle shadows. ([1036174](https://issuetracker.unity3d.com/issues/renderer-particle-alignment-affected-by-directional-light-when-casting-slash-receiving-shadows-is-enabled))
    
*   Particles: Fixed shortcuts when particle overlay is collapsed. ([1340675](https://issuetracker.unity3d.com/issues/particle-system-shortcuts-dont-work-when-particle-playback-controls-are-collapsed))
    
*   Particles: Keep Particle System curve editor labels within the GUI box, to avoid any clipping. ([1323617](https://issuetracker.unity3d.com/issues/particle-system-curves-point-time-and-value-info-box-clips-when-moved-to-the-right-edge-of-the-curves-window))
    
*   Particles: Prevent errors and invalid particle simulations, when using an Arc of 0 and Ping-Pong mode in the Shape module. ([1278594](https://issuetracker.unity3d.com/issues/particle-system-throws-errors-when-the-shapes-arc-is-set-to-0-and-mode-is-set-to-ping-pong))
    
*   Particles: Run the Trigger Module on newly spawned particles in case they need removing, or a callback firing. ([1328141](https://issuetracker.unity3d.com/issues/shuriken-particle-flicker-outside-the-collider-when-outside-trigger-is-set-to-kill))
    
*   Particles: The create button("+") is now hidden in the Particles Window when editing a Prefab Asset. ([1287185](https://issuetracker.unity3d.com/issues/shuriken-prefab-asset-is-disabled-to-prevent-data-corruption-error-is-thrown-on-adding-particle-system-from-its-prefabs-editor))
    
*   Particles: Updated emitter velocity as soon as the property is changed, not on the next frame. ([1342626](https://issuetracker.unity3d.com/issues/particlesystem-dot-mainmodule-dot-emittervelocity-from-the-previous-frame-is-used-in-particlesystem-dot-emit))
    
*   Physics: Added better error message when trying to set an invalid mesh on a MeshCollider ([1282750](https://issuetracker.unity3d.com/issues/physics-dot-raycast-throws-errors-when-used-on-a-navmesh))
    
*   Physics: Anchored prismatic limit handles in screen space to avoid them occluding small Articulation Body links.
    
*   Physics: Changed the PhysX PVD connection code so that it can connect to a running PVD instance, and does set the visualization flags correctly.
    
*   Physics: Ensure that a Rigidbody2D never alters current Transform Z position at the point we perform interpolation write-back to the Transform position. (1362840)
    
*   Physics: Fixed a crash when accessing RaycastHit.lightmapCoord of a hit agains a Mesh that does not have texture channel 1 ([1361884](https://issuetracker.unity3d.com/issues/editor-crashes-when-accessing-raycasthit-dot-lightmapcoord-and-the-hit-mesh-does-not-have-texture-channel-1))
    
*   Physics: Fixed a crash when adding more than 65534 Colliders to a Rigidbody or an Articulation Body. ([1325575](https://issuetracker.unity3d.com/issues/crash-in-physx-npshape-updatesq-when-setting-lots-of-colliders-under-a-rigidbody-parent))
    
*   Physics: Fixed an issue where, when using "Collision2D.GetContacts(List<;ContactPoint2D>;)", the list size was incorrectly set the same as the list capacity rather than the number of results returned. (1352777)
    
*   Physics: Fixed Articulation Bodies not changing collision detection mode via Script. ([1330429](https://issuetracker.unity3d.com/issues/setting-articulationbody-dot-collisiondetectionmode-at-runtime-via-script-to-discrete-does-not-work-if-its-being-set-from-continuous))
    
*   Physics: Fixed Character Controller returning incorrect closest points when the center is offset. ([1339454](https://issuetracker.unity3d.com/issues/character-controller-closest-point-returns-incorrect-position-when-the-center-is-offsetted))
    
*   Physics: Fixed crash when trying to read texture coordinates from a RaycastHit when the mesh was unreadable. ([1006742](https://issuetracker.unity3d.com/issues/editor-crashes-when-access-to-raycasthit-dot-texturecoord2-collider-is-meshcollider-and-mesh-dot-isreadable-equals-false))
    
*   Physics: Fixed Physics Debugger not showing up in Prefab Mode. ([1158611](https://issuetracker.unity3d.com/issues/physics-debug-visualization-does-not-work-when-in-prefab-edit-mode))
    
*   Physics: Fixed Rigidbody falling asleep when fixed joint is removed ([963368](https://issuetracker.unity3d.com/issues/gravity-not-affecting-object-after-removing-fixed-joint))
    
*   Physics: Fixed Rigidbody.angularVelocity setter that constrained the velocity wrongly; it's now doing it in mass-space to match what should happen actually. ([1083573](https://issuetracker.unity3d.com/issues/rigidbody-rotates-around-world-z-axis-instead-of-local-z-axis-when-constraints-are-applied))
    
*   Physics: Prevented the ConnectedAnchor to be detected as property modification when AutoConfigureConnectedAnchor is set and ConnectedAnchor gets a generated value than happens to be different than the corresponding ConnectedAnchor value in the prefab. ([1308880](https://issuetracker.unity3d.com/issues/prefab-instances-detect-and-cant-revert-an-override-when-a-joint-components-connected-anchor-is-changed-in-a-prefab))
    
*   Prefabs: A component added to a Prefab in Prefab Mode which is found to conflict with a pre-existing component on an instance is now suppressed so the Inspector displays only the pre-existing component instead of both. ([1148404](https://issuetracker.unity3d.com/issues/two-incompatible-components-can-be-added-to-a-gameobject-when-using-the-prefab-mode))
    
*   Prefabs: Added error message to prevent entering playmode when the scene contains missing Prefabs instances. Added option to Unpack Prefabs when deleting them.
    
*   Prefabs: An open ComparisonViewPopup is now closed if undo operations cause selection changes which affect the content of the Overrides Window's tree view and render the popup's visibility redundant. ([1325826](https://issuetracker.unity3d.com/issues/undo-improved-prefabs-errors-are-thrown-on-performing-the-undo-operation-over-the-prefab-override-window))
    
*   Prefabs: Calling UnloadUnusedAssetsImmediate in OnWillCreateAsset/OnWillSaveAsset during prefab save no longer crashes. ([1303644](https://issuetracker.unity3d.com/issues/unity-crashes-when-editorutility-dot-unloadunusedassetsimmediate-is-called-inside-of-onwillcreateasset-slash-onwillsaveasset))
    
*   Prefabs: Checked that the GameObject pointed by a component, during scene loading, is actually a valid GameObject. ([1333374](https://issuetracker.unity3d.com/issues/corrupted-prefab-crashes-the-editor-when-opening-scene-containing-it))
    
*   Prefabs: Components that are suppressed on a Prefab instance by added components, now reappear when the suppressor is destroyed. ([1295687](https://issuetracker.unity3d.com/issues/prefab-rigidbody-component-is-shown-in-prefab-but-not-in-its-instance-when-unapplied-joint-component-is-removed))
    
*   Prefabs: Corrected API documentation for SceneManager.activeSceneChanged. ([1038093](https://issuetracker.unity3d.com/issues/several-scene-management-events-are-not-called-when-performing-normal-scene-functions))
    
*   Prefabs: Fixed an issue where OnValidate() could be called on an inactive Prefab. ([1271820](https://issuetracker.unity3d.com/issues/onvalidate-called-when-monobehaviour-inside-prefab-changes))
    
*   Prefabs: Fixed case 1085603: Undoing the 'Create/Replace prefab' action does not revert the Prefab to its previous state'. ([1085603](https://issuetracker.unity3d.com/issues/undoing-the-create-slash-replace-prefab-action-does-not-revert-the-prefab-to-its-previous-state))
    
*   Prefabs: Fixed Crash when Exiting Play mode with Multiple scenes loaded ([1298007](https://issuetracker.unity3d.com/issues/crash-when-exiting-play-mode-with-multiple-scenes-loaded))
    
*   Prefabs: Fixed FindAllInstancesOfPrefab to filter persistent instances.
    
*   Prefabs: Fixed multiple selection of added GameObjects not being applied to Prefabs (or reverted) via the Hierarchy context menu. (1313939)
    
*   Prefabs: Fixed prefabs don't visually show their HideFlags.NotEditable state in the Hierarchy window. ([1324446](https://issuetracker.unity3d.com/issues/prefabs-dont-visually-show-their-hideflags-dot-noteditable-state-in-the-hierarchy-window))
    
*   Prefabs: Fixed Recovery GameObject is created when opening scene with missing Prefab as a child of other GameObject ([1299744](https://issuetracker.unity3d.com/issues/recovery-gameobject-is-created-when-opening-scene-with-missing-prefab))
    
*   Prefabs: Fixed that changes to Prefab instances in the Scene are not reflected when dragging Materials/Scripts onto the Asset in the Project Window. ([1311622](https://issuetracker.unity3d.com/issues/changes-to-prefab-in-the-scene-are-not-reflected-when-dragging-materials-slash-scripts-onto-the-asset-in-the-project-window))
    
*   Prefabs: Fixed that creating a Prefab by dragging did not handle missing scripts gracefully. ([1259961](https://issuetracker.unity3d.com/issues/create-original-prefab-operation-does-not-handle-exception-gracefully))
    
*   Prefabs: Fixed that Overrides window does not refresh state after changing GameObject name in the comparison popup. ([1300152](https://issuetracker.unity3d.com/issues/override-window-does-not-repaint-after-changing-prefab-name-in-the-prefab-override-dropdown))
    
*   Prefabs: Fixed undo not working when Renaming a Missing Prefab in the Hierarchy. ([1165052](https://issuetracker.unity3d.com/issues/undo-is-not-working-when-renaming-a-missing-prefab-in-the-hierarchy))
    
*   Prefabs: Improved error logging when importing Prefab files. The import errors are now collected and logged as one message instead of individual errors and most importantly the Prefab asset path is made clear to the user. Also clicking the message will frame the Prefab in the Project Browser. Also missing Prefabs will now be logged as an error. (1298338)
    
*   Prefabs: PrefabUtility.SavePrefabAsset is now robust against supplied objects being reloaded during AssetModificationProcessor.OnWillSaveAssets. ([1276013](https://issuetracker.unity3d.com/issues/crash-on-scripting-scriptingwrapperfor-slash-saveprefab-internal-when-saving-a-prefab-asset-using-assetmodificationprocessor))
    
*   Prefabs: Removed wrong error message. ([1287903](https://issuetracker.unity3d.com/issues/the-prefab-instance-was-disconnected-during-deactivation-while-merging-dot-error-is-thrown-when-modifying-and-saving-a-prefab))
    
*   Prefabs: Set as first/last sibling cannot be undone to reorder the Prefab hierarchy. ([1296698](https://issuetracker.unity3d.com/issues/prefab-set-as-first-slash-last-sibling-cannot-be-undone-to-reorder-the-prefab-hierarchy))
    
*   Prefabs: Updated documentation for OnPostprocessPrefab to reflect better the behavior. ([1304102](https://issuetracker.unity3d.com/issues/dontsaveineditor-and-noteditable-flags-are-not-automatically-added-to-the-asset-when-using-onpostprocessprefab-method))
    
*   Prefabs: Updated documentation that scripts using OnValidate can only modify data on itself. ([1333052](https://issuetracker.unity3d.com/issues/value-set-to-serialized-fields-in-onvalidate-method-doesnt-get-displayed-correctly-in-the-inspector-window))
    
*   Profiler: Enabled GPU profiling in the Editor ([1315474](https://issuetracker.unity3d.com/issues/gpu-profiler-does-not-work-in-editmode))
    
*   Profiler: Fixed a material leak in the UISystemProfiler UI ([1280162](https://issuetracker.unity3d.com/issues/hidden-slash-preview-transparent-materials-uses-additional-memory-each-time-when-scripts-are-reimported))
    
*   Profiler: Fixed an issue where creating a Memory snapshot file writer with a null or empty string would crash the Editor. ([1296217](https://issuetracker.unity3d.com/issues/crash-in-filesystementry-set-when-creating-or-opening-a-memorysnapshotfilewriter-with-a-null-argument))
    
*   Profiler: Fixed an issue where we could no longer connect to tethered Android devices after they have been disconnected, without manually calling adb commands from the CLI. ([1268987](https://issuetracker.unity3d.com/issues/removing-the-usb-from-a-device-whilst-profiling-leaves-you-unable-to-capture-until-you-restart-or-rebuild-the-app))
    
*   Profiler: Fixed Application.targetFrameRate frames visualization in the Editor when profiling Play mode. ([1355826](https://issuetracker.unity3d.com/issues/play-mode-profiler-does-not-wait-for-application-dot-targetframerate))
    
*   Profiler: Fixed crash due to Profiler code during Editor Shutdown
    
*   Profiler: Fixed gaps in script-driven profiler counters in the Editor when profiling Play mode. ([1343692](https://issuetracker.unity3d.com/issues/profiler-adaptiveperformance-profiling-adaptive-performance-project-in-editor-hhas-some-profiling-holes))
    
*   Profiler: Fixed HDRP/URP GPU statistics in Editor showing zeroes (1299569)
    
*   Profiler: Fixed performance test instability. (1351859)
    
*   Profiler: Fixed player name label width in Player Connection dropdown to accommodate long strings. Fixed player name reported in Console window on connection to be consistent with Player Connection dropdown. Values in columns will now truncate with elipses if they are too large too fit in the column. When a player is selected the dropdown will now close to mimic the old dropdown behaviour.
    
*   Profiler: Fixed Recorder reporting invalid data after being disabled and re-enabled. (1321813)
    
*   Profiler: Fixed selection of RestoreManagedReferences sample and its children in Profiler Window ([1330206](https://issuetracker.unity3d.com/issues/argumentexception-is-thrown-when-selecting-restoremanagedreferences-in-the-profiler))
    
*   Profiler: Fixed standalone profiler shows editor update check dialogue on start. (1334264)
    
*   Profiler: Fixed systrace captures producing corrupted data when started in middle of frame, mismatch begin and end samples. (1270929)
    
*   Profiler: Fixed the Thread Selection Dropdown in Hierarchy view showing multiple threads as selected if they all share the same name.
    
*   Profiler: Player names are no longer aggresively cut off. (1345540)
    
*   Profiler: Profiler charts now correctly render user-defined Profiler Counters in the Network category captured when UNet is disabled. ([1360925](https://issuetracker.unity3d.com/issues/charts-do-not-render-when-a-counter-is-marked-as-network-category))
    
*   Profiler: Profiler will now clear when entering playmode with the game view maximised. ([1307042](https://issuetracker.unity3d.com/issues/profiler-clear-on-play-does-not-clear-frames-when-game-view-is-set-to-maximize-on-play))
    
*   Profiler: Removed Total Time from GI Profiler Module chart as it duplicated time in the stacked chart (1305568)
    
*   Profiler: Text is now selectable in a custom Profiler module's default Details View. ([1336943](https://issuetracker.unity3d.com/issues/text-is-not-selectable-in-profilers-custom-modules-default-details-view))
    
*   Profiler: The Profiler window can no longer be shrunk small enough to hide some of the toolbar options. ([1354357](https://issuetracker.unity3d.com/issues/profiler-window-can-be-shrunk-to-the-point-where-some-top-menu-options-become-hidden))
    
*   Profiler: Truncated project name in the profiler broadcast to fit within the message buffer. ([1322888](https://issuetracker.unity3d.com/issues/connection-does-not-appear-in-the-profiler-target-player-selection-dropdown-when-product-name-is-equals-69-symbols))
    
*   Profiler: When disconnecting from and autoconnected device the profiler will now default back to playmode instead of the previous connection. (1268887)
    
*   Scene Manager: Added debouncing to the search field in the Hierarchy and Scene view for better search input experience in large scenes. Is also now consistent with Project Browser searching behavior. (1315731)
    
*   Scene Manager: Fix rename overlay in Hierarchy to support hierarchy changes while renaming. (1296235)
    
*   Scene Manager: Fix that prevent dragging gameobject in a scene that is not loaded ([1291614](https://issuetracker.unity3d.com/issues/dragging-a-game-object-into-a-scene-that-is-not-loaded-causes-other-not-loaded-scenes-to-disappear))
    
*   Scene Manager: Fixed "PlayerLoop internal function has been called recursively" error is thrown when calling NewScene() from the Update function. ([1258244](https://issuetracker.unity3d.com/issues/playerloop-internal-function-has-been-called-recursively-error-is-thrown-when-loading-a-new-scene-from-the-update-function))
    
*   Scene Manager: Fixed focus issue when using a secondary hidden Hierarchy. When creating a new GameObject a visible Hierarchy tab is focused, prioritizing the last interacted Hierarchy if visible. Focusing a hidden Hierarchy tab is therefore now prevented in this situation. ([1190664](https://issuetracker.unity3d.com/issues/secondary-hidden-hierarchy-windows-pop-up-when-a-new-gameobject-is-created-in-another-hierarchy-window))
    
*   Scene Manager: Fixed GameObjects in Hierarchy window not hidden when using HideFlags.HideInHierarchy until next Hierarchy rebuild. ([1167675](https://issuetracker.unity3d.com/issues/gameobjects-in-hierarchy-window-are-not-hidden-when-using-hideflags-dot-hideinhierarchy))
    
*   Scene Manager: Fixed SceneManager.GetSceneByName() returning null when buildsettings path to the Scene is given as a parameter. ([1155473](https://issuetracker.unity3d.com/issues/scenemanager-dot-getscenebyname-returns-null-when-path-to-the-scene-is-specified))
    
*   Scene Manager: Improved performance of updates on large arrays. ([1272309](https://issuetracker.unity3d.com/issues/performance-issues-when-quickly-changing-values-of-tens-of-thousands-array-elements))
    
*   Scene Manager: Paste as Child' now supports pasting gameObjects to SubScenes. (1316660)
    
*   Scene Manager: Updated dirtiness logic for undoing after save. (1221800)
    
*   Scene/Game View: Added a verification of the current mode (edit/play) to only display FPS when in playmode as the measured value does not mean anything in edit mode and can confuse some users. ([1285123](https://issuetracker.unity3d.com/issues/statistics-window-updates-outside-of-the-play-mode-when-the-scene-is-updated))
    
*   Scene/Game View: Added an option to disable the hide of the gizmos. ([1313974](https://issuetracker.unity3d.com/issues/hdrp-volume-gizmo-continuously-reenabled-following-manual-deactivation-makes-scene-interaction-very-challenging))
    
*   Scene/Game View: Added check before recursion that the gizmo is not already active. ([1326407](https://issuetracker.unity3d.com/issues/nested-objects-draw-gizmos-twice))
    
*   Scene/Game View: Bugfix for Instability in picking tests failure. (1329183)
    
*   Scene/Game View: Fix for built-in tool buttons toggling highlighted state when clicked consecutively. ([1344813](https://issuetracker.unity3d.com/issues/tool-from-the-scene-view-toolbar-is-visually-turned-off-but-still-active-when-clicking-the-active-tool-again))
    
*   Scene/Game View: Fixed Camera Overlay lost when entering play mode. (1340455)
    
*   Scene/Game View: Fixed case where clicking on a popup button while the popup was open would not close the existing window. ([1335070](https://issuetracker.unity3d.com/issues/scene-view-grid-and-snap-toolbars-dropdown-window-do-not-close-on-clicking-on-it))
    
*   Scene/Game View: Fixed clicking on a non-prefab child of a prefab instance incorrectly selecting prefab root. (1305433)
    
*   Scene/Game View: Fixed custom tool button incorrectly showing a built-in tool in certain cases where EditorToolContext is active. (1339433)
    
*   Scene/Game View: Fixed fading between 2D and 3D modes with overlays. (1339978)
    
*   Scene/Game View: Fixed for IMGUI content not being displaced by overlay toolbars. (1339990)
    
*   Scene/Game View: Fixed for the default Overlays' preset not matching the intended design. (1339964)
    
*   Scene/Game View: Fixed for translation tools offsetting object when cursor moved off-screen. ([1360113](https://issuetracker.unity3d.com/issues/the-object-can-get-offset-from-the-mouse-cursor-when-using-move-tools-and-the-cursor-hits-the-edge-of-the-screen))
    
*   Scene/Game View: Fixed Gameview focus inconsistent when re-docking. (1272795)
    
*   Scene/Game View: Fixed Grid Axis field in the Grid Settings Overlay not accepting input. (1345036)
    
*   Scene/Game View: Fixed Hierarchy context menu showing empty submenu entries. ([1319505](https://issuetracker.unity3d.com/issues/scene-header-context-menu-has-extra-menu-items))
    
*   Scene/Game View: Fixed issue where some Overlay windows would throw exception after domain reload. (1345651)
    
*   Scene/Game View: Fixed issue with scene view overlay in some packages ([1339984](https://issuetracker.unity3d.com/issues/probuilder-overlay-windows-do-not-render-in-the-scene-view))
    
*   Scene/Game View: Fixed possible exception when removing a collider component while the collider editor tool is active. ([1259502](https://issuetracker.unity3d.com/issues/missingreferenceexception-and-gui-errors-are-thrown-when-removing-collider-component-while-editting-collider-bounds))
    
*   Scene/Game View: Fixed Scene Hierarchy context menu not showing separators in submenus. ([1247305](https://issuetracker.unity3d.com/issues/menuitems-are-not-separated-with-a-separator-in-the-hierarchy-context-menu))
    
*   Scene/Game View: Fixed Scene View camera zooming too far when using middle mouse wheel scroll with a very small object framed. ([1300336](https://issuetracker.unity3d.com/issues/scene-camera-zoom-sensitivity-is-not-high-enough))
    
*   Scene/Game View: Fixed shortcut conflict between Scene View "Nudge Grid" and 2D "Flip X Y" axis. ([1309850](https://issuetracker.unity3d.com/issues/grid-painting-slash-flip-shortcuts-conflict-with-the-grid-slash-nudge-grid-shortcuts))
    
*   Scene/Game View: Fixed some Scene View Overlays incorrectly registering as applicable to any Editor Window. (1337371)
    
*   Scene/Game View: Fixing MissingReferenceException in the Scene overlay when deleting a selected Particle System. ([1295035](https://issuetracker.unity3d.com/issues/editor-missingreferenceexception-when-deleting-a-selected-particle-system-while-the-scene-view-is-in-focus))
    
*   Scene/Game View: Fixing overlay placement when scene view is resizing (1341038)
    
*   Scene/Game View: Fixing selection outline not drawn for SRP objects in scene view ([1294951](https://issuetracker.unity3d.com/issues/selection-outline-is-not-drawn-for-gameobjects-that-are-using-the-hdrp-shaders))
    
*   Scene/Game View: Fixing selection outline not fading when behind other objects ([1119607](https://issuetracker.unity3d.com/issues/game-objects-selection-outline-doesnt-clip-behind-other-objects))
    
*   Scene/Game View: Fixing Slider1D Handle
    
*   Scene/Game View: Global tool buttons are disabled when not useable. (1310614)
    
*   Scene/Game View: Improved performance when opening `Scene View` window. (1343564)
    
*   Scene/Game View: Increased maximum Scene Camera fly speed to 1e+5. ([1287220](https://issuetracker.unity3d.com/issues/speed-does-not-further-increase-when-setting-camerasettings-dot-speedmax-value-above-99))
    
*   Scene/Game View: Overlay positioning optimization by using transform position and usageHints (1339973)
    
*   Scene/Game View: Scene/Game View: Fixed an exception when loading an Overlay preset with invalid window type. (1337897)
    
*   Scene/Game View: The Scene view camera was snapping back or forward when zooming in while holding the Alt key.  
    This was due to a small error in the formula.  
    There is no more jump in the zoom with this fix. ([1293718](https://issuetracker.unity3d.com/issues/scene-view-camera-snapping-back-or-forward-when-zooming-in-while-holding-the-alt-key))
    
*   Scripting: Added support for custom attribute types inheriting from RuntimeInitializeOnLoadMethodAttribute. (1334599)
    
*   Scripting: Added type and method information to exceptions raised by the assembly reference checker. ([1307194](https://issuetracker.unity3d.com/issues/build-fails-with-object-reference-not-set-exception-when-building-android))
    
*   Scripting: APIUpdaterManager can now handle more than 64 assemblies. ([1308408](https://issuetracker.unity3d.com/issues/notsupportedexception-is-thrown-when-compiling-slash-recompiling-project-with-more-than-64-different-assemblies))
    
*   Scripting: Avoid flooding the console when parsing a define expression fails and the Asmdef inspector is active.  
    Also improve interaction with define expression parsing errors in the console. ([1314026](https://issuetracker.unity3d.com/issues/tests-assembly-definition-errors-are-thrown-on-adding-invalid-versions-to-version-defines-list))
    
*   Scripting: Avoid GC allocation in UnitySynchronizationContext. ([1276456](https://issuetracker.unity3d.com/issues/additional-memory-allocated-when-removing-workrequest-in-unitysynchronizationcontext-dot-cs))
    
*   Scripting: Build fails when there is a comma in path. ([1325976](https://issuetracker.unity3d.com/issues/build-fails-when-there-is-a-comma-in-the-projects-path))
    
*   Scripting: Change Roslyn Analyzers to be run part of normal Compilation Step.  
    This will also result in Analyzer errors to be treated as an Compile Error.
    
*   Scripting: Disabled native test causing instabilities. (1322841)
    
*   Scripting: Enabled IPv6 sockets creation with the ICMP protocol. ([1309061](https://issuetracker.unity3d.com/issues/cannot-create-an-ipv6-socket-with-the-icmp-protocol))
    
*   Scripting: Exclude readonly files from script execution order menu to reduce visual noise. ([1281215](https://issuetracker.unity3d.com/issues/script-execution-order-does-not-work))
    
*   Scripting: Fix a stack overflow occurring when a custom `ILogHandler` is throwing an exception in LogFormat/LogException methods (1241896)
    
*   Scripting: Fix crash on Stackoverflow, when instantiating infinitely in OnEnable ([1263270](https://issuetracker.unity3d.com/issues/crash-on-gameobject-activateawakerecursively-when-exiting-play-mode))
    
*   Scripting: Fix not being able to select external script editors that don't have the '.app' extension on OSX. ([1250634](https://issuetracker.unity3d.com/issues/mac-unable-to-choose-files-with-sh-and-cmd-extensions-as-external-script-editor))
    
*   Scripting: Fix possible exception after changing Roslyn Analyzers to be part of the initial compilation (1313026)
    
*   Scripting: Fixed a bug where adding a script to the list of custom-ordered scripts in "Project Settings" ->; "Script Ordering" would pick up a totally unrelated script. (1327742)
    
*   Scripting: Fixed a crash happening when trying to enter an unsupported character (such as an emoji) in a field in a game built with IL2Cpp backend. ([1314163](https://issuetracker.unity3d.com/issues/tmp-inputfield-doesnt-properly-handle-surrogate-pairs-causing-crash-within-il2cpp))
    
*   Scripting: Fixed a memory corruption crash related to the incremental GC incorrectly freeing objects.
    
*   Scripting: Fixed a memory leak happening when removing listeners from a UnityEvent that is never raised afterwards. ([1303095](https://issuetracker.unity3d.com/issues/memory-of-non-persistent-event-listeners-isnt-cleared-when-calling-unityeventbase-dot-removealllisteners))
    
*   Scripting: Fixed ApiUpdater incorrectly removing _usings_ in some scenarios
    
*   Scripting: Fixed assemblies in non local/embedded packages triggering updater consent ([1171778](https://issuetracker.unity3d.com/issues/ads-api-updater-called-every-time-for-project-after-ads-package-gets-added-to-that-project))
    
*   Scripting: Fixed condition on accessing a game object from a callback while it was being constructed that was leaving the original GameObject managed wrapper in a detached state. ([1295939](https://issuetracker.unity3d.com/issues/gameobject-reference-is-null-when-creating-it-inside-reset-function-and-assigning-script-as-component))
    
*   Scripting: Fixed crash in ScriptUpdater.exe when editor is installed in a path containing commas. ([1341703](https://issuetracker.unity3d.com/issues/system-dot-io-dot-directorynotfoundexception-appears-when-adding-platforms-windows-package-and-editors-path-contains-comma))
    
*   Scripting: Fixed editor crash when an animation tries to pass an invalid scriptable object as a method parameter. ([1252134](https://issuetracker.unity3d.com/issues/editor-crashes-when-calling-an-animation-event-with-an-invalid-scriptable-object-parameter))
    
*   Scripting: Fixed invalid memory write in MonoBehaviour when it destroys its own instance within the OnDisable call. (1286736)
    
*   Scripting: Fixed nested aliases handling in ApiUpdater ([1251569](https://issuetracker.unity3d.com/issues/scriptupdater-crashes-when-alias-for-the-same-name-is-set-multiple-times-in-same-source))
    
*   Scripting: Fixed NVidia native libraries being included in player build when the Module is disabled. ([1332465](https://issuetracker.unity3d.com/issues/internal-package-modules-that-are-not-used-in-a-project-do-not-get-stripped-from-player-builds))
    
*   Scripting: Fixed potential error due to ApiUpdater not handling extension methods correctly.
    
*   Scripting: Fixed rare deadlock case in GC. (1229776)
    
*   Scripting: Fixed undoing changes to a prefab instance not triggering object change events. (1308479)
    
*   Scripting: Fixed XmlSerializer not working with managed code stripping when using the mono backend. ([1331829](https://issuetracker.unity3d.com/issues/class-get-stripped-when-using-preserve-attribute-with-mono-backend))
    
*   Scripting: Fixes HttpUtility.UrlEncode runtime exceptions ([1296177](https://issuetracker.unity3d.com/issues/httputility-null-reference-exception-on-net-4-dot-x-when-performing-httputility-dot-urlencode))
    
*   Scripting: Ignore Visual Scripting assemblies when building for mobile devices, so no MouseEvent handler warning is raised.
    
*   Scripting: Improved diagnostic messages for unsupported cases of RuntimeInitializeOnLoadMethod usage. ([1246081](https://issuetracker.unity3d.com/issues/uwp-excessive-il2cpp-stripping-of-runtimeinitializeonloadmethod-method-with-preserve-causes-crash-on-runtime))
    
*   Scripting: Interpolated verbatim strings can start with both $@"..." and @$"..." as specified in C# 8.0. ([1304285](https://issuetracker.unity3d.com/issues/interpolated-verbatim-strings-with-at-before-dollars-doesnt-compile-when-used-in-other-class-and-referenced-in-monobehaviour-class))
    
*   Scripting: NativeArray<;T>;.ReadOnly now implements IEnumerable<;T>;. ([1319358](https://issuetracker.unity3d.com/issues/nativearray-dot-readonly-does-not-implement-ienumerable))
    
*   Scripting: Performance improvements in ApiUpdater.
    
*   Scripting: Provide Visual Studio 2019 installers rather than Visual Studio 2017
    
*   Scripting: Self-referencing assemblies will give error during assembly validation.
    
*   Scripting: UnityWebRequest no longer re-uses previous connections when custom certificate handler is changed. (1337019)
    
*   Scripting: When an editor-only precompiled assembly reference is ignored by the script compiler because the asmdef referencing it is not editor-only, a warning now appears in the console. ([1220959](https://issuetracker.unity3d.com/issues/ux-assemblies-which-reference-moq-dot-dll-are-not-referenced-in-editor-when-they-include-any-platform-except-editor))
    
*   Scripting: When inspecting a readonly asmdef file, the inspector fields are disabled and a small text indicates that the asmdef file is read-only. ([1255405](https://issuetracker.unity3d.com/issues/changes-via-inspector-are-not-saved-to-a-asmdef-asset-when-it-is-marked-as-read-only-in-the-operating-system))
    
*   Search: Added a tree view to list and browse save searches.
    
*   Search: Added support to search references using an UnityEngine.Object instance ID, i.e. `ref:-2458`, -2458 can be a component instance ID. (1331890)
    
*   Search: Fix editor stall when the asset worker try to resolve a message log with an UnityEngine.Object in a non-main thread. ([1316768](https://issuetracker.unity3d.com/issues/search-fix-asset-worker-log-object-thread-stalling))
    
*   Search: Fixed degenerative indexing issue with VFX assets.
    
*   Search: Fixed errors are thrown on enabling 'UI Toolkit Live Reload' in 'Search asset store' window. ([1299600](https://issuetracker.unity3d.com/issues/search-errors-are-thrown-on-enabling-ui-toolkit-live-reload-in-search-asset-store-window))
    
*   Search: Fixed floating point search expression parsing for non US locales.
    
*   Search: Fixed indexed prefab objects cannot be resolved using the search result global object id. (1328618)
    
*   Search: Fixed prefab subtypes not available in default project index. (1332948)
    
*   Search: Fixed search index incremental update merge issue.
    
*   Search: Fixed search index should discard long serialized property string (i.e. embedded JSON string). (1362623)
    
*   Search: Fixed search item label and description in compact mode.
    
*   Search: Fixed search tab showing HTML <;a>; tags for the item count. ([1301148](https://issuetracker.unity3d.com/issues/search-tab-show-html-tags-for-the-item-count))
    
*   Search: Fixed search view error reporting in status bar when no group is selected.
    
*   Search: Fixed SearchService.Request when used with a non-asynchronous queries.  
    See https://forum.unity.com/threads/quick-search-preview.635863/page-12#post-6907427.
    
*   Search: Fixed text in the search field of the Search window doesn't get selected after focusing the window and clicking on the field once.
    
*   Search: Fixed too many objects being indexed and out of memory exception  
    Reported on the forums: https://forum.unity.com/threads/quick-search-preview.635863/page-12#post-7004042.
    
*   Serialization: Added pruning when an object with \[SerializeReference\] contains missing types. (1338952)
    
*   Serialization: Binary2Text adding support for SerializeReference/ReferenceRegistry. (1284031)
    
*   Serialization: fix uninitialized member field reported by static analysis (1305542)
    
*   Serialization: Fixed an issue where a SerializedObject is created with empty Objects. ([1279513](https://issuetracker.unity3d.com/issues/no-way-to-check-if-a-serializedobject-is-null-when-it-is-initialized-with-null))
    
*   Serialization: Fixed clone/load/save performance regression. (1338713)
    
*   Serialization: Fixed for ability to find assets derived from a Generic type in the object selector window. ([1288312](https://issuetracker.unity3d.com/issues/assets-are-not-listed-in-the-object-picker-field-when-scriptableobject-is-generic))
    
*   Serialization: Fixed for name conversion not working in specific code path. (1352617)
    
*   Serialization: Fixed regression where prefab override would not show up on SerializeReference instance and you could no longer remove contextually a single Override. ([1348031](https://issuetracker.unity3d.com/issues/prefab-property-override-blue-line-have-disepeared-from-hdrps-custom-passes))
    
*   Serialization: Fixed SerializedProperty to properly set a value across all selected objects when the value already present on the first object matches the specified value. ([1228004](https://issuetracker.unity3d.com/issues/iterating-through-serializedobject-array-and-setting-property-fields-stops-when-an-object-that-does-not-need-updating-is-found))
    
*   Serialization: Fixed SerializeReference object missing in certain situation.
    
*   Serialization: Missing types from managed referenced object are properly stripped when creating a player build.
    
*   Services: Analytics no longer auto-activates on new project link.
    
*   Services: Fixed Android app\_build is 0 for reports in Cloud Diagnostics. ([1217055](https://issuetracker.unity3d.com/issues/android-app-build-is-0-for-crash-reports))
    
*   Services: Fixed Cloud Diagnostics native crash reporting on tvOS. (1332243)
    
*   Services: Fixed Cloud Diagnostics sometimes failing to provide line numbers for Windows Native crashes. (1329172)
    
*   Services: Fixed iOS builds may fail in Xcode with error about USYM\_UPLOAD\_AUTH\_TOKEN. (1329176)
    
*   Services: Fixed the "Latest Version" section of the In-App Purchasing Settings when com.unity.purchasing version of 2 or less is installed. It now always offers the verified version, but adds migration warning messages about moving to newer versions which do not use the IAP Asset Store plugin.
    
*   Services: Fixed upload of symbols to Cloud Diagnostics for Windows builds. (1329220)
    
*   Services: Updated PLCrashReporter version on iOS and tvOS to 1.8.1. (1317214)
    
*   Services: We suppress Analytics curl errors to the console but only in the editor. this change allows this same suppression to carry across into the development console (we still log to file). ([1318074](https://issuetracker.unity3d.com/issues/curl-errors-in-development-builds-cannot-be-disabled-and-spam-the-console-when-offline))
    
*   Shadergraph: - Clean up console error reporting from node shader compilation so errors are reported in the graph rather than the Editor console ([1296291](https://issuetracker.unity3d.com/issues/shadergraph-shadergraph-shader-errors-in-console-are-not-cleared-when-the-graph-is-fixed))
    
*   Shadergraph: Added padding to the blackboard window to prevent overlapping of resize region and scrollbars interfering with user interaction.
    
*   Shadergraph: Blackboard now properly handles selection persistence of items between undo and redos.
    
*   Shadergraph: Disconnected nodes with errors in ShaderGraph no longer cause the imports to fail. ([1349311](https://issuetracker.unity3d.com/issues/shadergraph-erroring-unconnected-node-causes-material-to-become-invalid-slash-pink))
    
*   Shadergraph: Fixed "Disconnect All" option being grayed out on stack blocks. ([1313201](https://issuetracker.unity3d.com/issues/shadergraph-disconnect-all-option-is-greyed-out-on-stack-blocks))
    
*   Shadergraph: Fixed a bug when a node was both vertex and fragment exclusive but could still be used causing a shader compiler error. ([1316128](https://issuetracker.unity3d.com/issues/shadergraph-plugging-both-a-fragment-exclusive-and-vertex-exclusive-node-into-the-same-path-lets-you-make-an-invalid-route))
    
*   Shadergraph: Fixed a bug where changing a Target setting would switch the inspector view to the Node Settings tab if any nodes were selected.
    
*   Shadergraph: Fixed a bug where old preview property values would be used for node previews after an undo operation.
    
*   Shadergraph: Fixed a selection bug with block nodes after changing tabs ([1312222](https://issuetracker.unity3d.com/issues/shadergraph-selecting-stack-nodes-after-coming-back-to-the-shadergraph-tab-immediately-deselects-them))
    
*   Shadergraph: Fixed a serialization bug wrt PVT property flags when using subgraphs. This fixes SRP batcher compatibility.
    
*   Shadergraph: Fixed a Shader Graph issue where property auto generated reference names were not consistent across all property types. ([1336937](https://issuetracker.unity3d.com/issues/not-all-shader-graph-auto-generated-property-reference-names-start-with-a-underscore))
    
*   Shadergraph: Fixed a ShaderGraph issue where a material inspector could contain an extra set of render queue, GPU instancing, and double-sided GI controls.
    
*   Shadergraph: Fixed a ShaderGraph issue where a warning about an uninitialized value was being displayed on newly created graphs. (1331377)
    
*   Shadergraph: Fixed a ShaderGraph issue where Float properties in Integer mode would not be cast properly in graph previews. ([1330302](https://issuetracker.unity3d.com/issues/shadergraph-switching-floating-point-float-slash-vector1-with-fractional-value-to-integer-mode-keeps-fractional-value))
    
*   Shadergraph: Fixed a ShaderGraph issue where hovering over a context block but not its node stack would not bring up the incorrect add menu.. (1351733)
    
*   Shadergraph: Fixed a ShaderGraph issue where keyword properties could get stuck highlighted when deleted. ([1333738](https://issuetracker.unity3d.com/issues/shadergraph-keyword-properties-are-stuck-highlighted-when-a-keyword-node-is-selected-and-then-deleted))
    
*   Shadergraph: Fixed a ShaderGraph issue where ObjectField focus and Node selections would both capture deletion commands. ([1313943](https://issuetracker.unity3d.com/issues/shadergraph-custom-function-node-is-deleted-when-deleting-source-file-from-node-settings))
    
*   Shadergraph: Fixed a ShaderGraph issue where resize handles on blackboard and graph inspector were too small. ([1329247](https://issuetracker.unity3d.com/issues/shadergraph-resize-bounds-for-blackboard-and-graph-inspector-are-too-small))
    
*   Shadergraph: Fixed a ShaderGraph issue where selecting a keyword property in the blackboard would invalidate all previews, causing them to recompile. ([1347666](https://issuetracker.unity3d.com/issues/shadergraph-huge-performance-cost-when-selecting-keyword-in-shadergraph))
    
*   Shadergraph: Fixed a ShaderGraph issue where the right click menu doesn't work when a stack block node is selected. (1320212)
    
*   Shadergraph: Fixed a warning in ShaderGraph about BuiltIn Shader Library assembly having no scripts.
    
*   Shadergraph: Fixed an issue where a requirement was placed on a fixed-function emission property. ([1319637](https://issuetracker.unity3d.com/issues/shadergraph-selecting-urp-shadergraph-material-results-in-error-spam))
    
*   Shadergraph: Fixed an issue where an informational message could cause some UI controls on the graph inspector to be pushed outside the window. ([1343124](https://issuetracker.unity3d.com/issues/shader-graph-target-settings-add-slash-remove-button-disappears-on-adding-visual-effect-active-target))
    
*   Shadergraph: Fixed an issue where an integer property would be exposed in the material inspector as a float. ([1330302](https://issuetracker.unity3d.com/issues/shadergraph-switching-floating-point-float-slash-vector1-with-fractional-value-to-integer-mode-keeps-fractional-value))
    
*   Shadergraph: Fixed an issue where fog node density was incorrectly calculated.
    
*   Shadergraph: Fixed an issue where generated property reference names could conflict with Shader Graph reserved keywords. ([1328762](https://issuetracker.unity3d.com/issues/shadergraph-using-a-gradient-property-in-a-subgraph-and-using-that-subgraph-in-a-shadergraph-causes-compile-errors))
    
*   Shadergraph: Fixed an issue where ShaderGraph "view shader" commands were opening in individual windows, and blocking Unity from closing.
    
*   Shadergraph: Fixed an issue where the Rectangle Node could lose detail at a distance. New control offers additional method that preserves detail better (1156801)
    
*   Shadergraph: Fixed an issue where the ShaderGraph transform node would generate incorrect results when transforming a direction from view space to object space. ([1333781](https://issuetracker.unity3d.com/issues/shadergraph-behavior-of-view-to-object-space-in-direction-mode-is-wrong-in-urp))
    
*   Shadergraph: Fixed an issue where users can't create multiple Boolean or Enum keywords on the blackboard. ([1329021](https://issuetracker.unity3d.com/issues/shadergraph-cant-create-multiple-boolean-or-enum-keywords))
    
*   Shadergraph: Fixed an issue with how the transform node handled direction transforms from absolute world space in camera relative SRPs. ([1323726](https://issuetracker.unity3d.com/issues/shadergraph-transform-algorithm-from-absolute-world-to-object-mode-in-direction-mode-is-wrong))
    
*   Shadergraph: Fixed an unhelpful error message when custom function nodes didn't have a valid file. (1323493)
    
*   Shadergraph: Fixed bug where an exception was thrown on undo operation after adding properties to a category. ([1348910](https://issuetracker.unity3d.com/issues/invalidoperationexception-collection-was-modified-error-thrown))
    
*   Shadergraph: Fixed bug where it was not possible to switch to Graph Settings tab in Inspector if multiple nodes and an edge was selected. ([1357648](https://issuetracker.unity3d.com/issues/when-multiple-nodes-and-an-edge-is-selected-it-is-not-possible-to-switch-into-graph-settings-mode-for-graph-inspector))
    
*   Shadergraph: Fixed compilation problems on preview shader when using hybrid renderer v2 and property desc override Hybrid Per Instance.
    
*   Shadergraph: Fixed default shadergraph precision so it matches what is displayed in the graph settings UI (single). ([1325934](https://issuetracker.unity3d.com/issues/shadergraph-custom-function-node-thinks-graph-precision-is-half-when-created))
    
*   Shadergraph: Fixed divide by zero warnings when using the Sample Gradient Node.
    
*   Shadergraph: Fixed how shadergraph's prompt for "unsaved changes" was handled to fix double messages and incorrect window sizes. ([1319623](https://issuetracker.unity3d.com/issues/shadergraph-undocked-shader-graph-window-is-docked-when-closing-it-without-saving-changes))
    
*   Shadergraph: Fixed incorrect warning while using VFXTarget.
    
*   Shadergraph: Fixed indent level in shader graph target foldout. ([1339025](https://issuetracker.unity3d.com/issues/hdrp-foldout-is-indented-in-the-graph-inspector-while-urp-slash-built-in-is-not))
    
*   Shadergraph: Fixed inspector property header styling.
    
*   Shadergraph: Fixed issue where vertex generation was incorrect when only custom blocks were present. (1320695)
    
*   Shadergraph: Fixed issue with ShaderGraph custom interpolator node dependency ordering. ([1332553](https://issuetracker.unity3d.com/issues/shadergraph-user-is-allowed-to-plug-route-into-both-vertex-and-fragment-stages-combining-this-with-custom-interpolator-fails))
    
*   Shadergraph: Fixed issues with double prompts for "do you want to save" when closing Shader Graph windows. ([1316104](https://issuetracker.unity3d.com/issues/shadergraph-maximizing-a-tab-using-the-3-dots-menu-throws-do-you-want-to-save-menu-for-shadergraph))
    
*   Shadergraph: Fixed loading all materials from project when saving a ShaderGraph.
    
*   Shadergraph: Fixed Parallax Occlusion Mapping node to handle non-uniformly scaled UVs such as HDRP/Lit POM. (1347008)
    
*   Shadergraph: Fixed ParallaxMapping node compile issue on GLES2
    
*   Shadergraph: Fixed ParallaxOcclusionMapping node to clamp very large step counts that could crash GPUs (max set to 256). ([1329025](https://issuetracker.unity3d.com/issues/shadergraph-typing-infinity-into-the-steps-input-for-the-parallax-occlusion-mapping-node-crashes-unity))
    
*   Shadergraph: Fixed reordering when renaming enum keywords. ([1328761](https://issuetracker.unity3d.com/issues/shadergraph-reordering-and-then-renaming-enum-entries-breaks-existing-enum-nodes))
    
*   Shadergraph: Fixed ShaderGraph BuiltIn target not having collapsible foldouts in the material inspector. (1339256)
    
*   Shadergraph: Fixed ShaderGraph BuiltIn target not to apply emission in the ForwardAdd pass to match surface shader results. ([1345574](https://issuetracker.unity3d.com/issues/a-rectangular-area-is-rendered-with-spotlight-when-a-shader-graph-material-with-built-in-is-used))
    
*   Shadergraph: Fixed ShaderGraph exception when trying to set a texture to "main texture". ([1350573](https://issuetracker.unity3d.com/issues/shadergraph-setting-a-texture2d-as-the-main-texture-fails-and-throws-null-reference-exception))
    
*   Shadergraph: Fixed ShaderGraph HDRP master preview disappearing for a few seconds when graph is modified.
    
*   Shadergraph: Fixed ShaderGraph isNaN node, which was always returning false on Vulkan and Metal platforms.
    
*   Shadergraph: Fixed ShaderGraph sub-graph stage limitations to be per slot instead of per sub-graph node. ([1337137](https://issuetracker.unity3d.com/issues/shadergraph-subgraphs-should-have-different-stage-limitations-for-different-outputs))
    
*   Shadergraph: Fixed some shader graph compiler errors not being logged ([1304162](https://issuetracker.unity3d.com/issues/shadergraph-action-that-causes-the-graph-to-error-does-not-print-errors-to-console))
    
*   Shadergraph: Fixed the appearance (wrong text color, and not wrapped) of a warning in Node Settings. ([1356725](https://issuetracker.unity3d.com/issues/node-warnings-are-unreadable-when-using-graph-inspector-window))
    
*   Shadergraph: Fixed the BuiltIn Target to perform shader variant stripping. ([1345580](https://issuetracker.unity3d.com/issues/shadergraph-variant-stripping-fails-for-shader-graph-shaders-when-using-built-in-target))
    
*   Shadergraph: Fixed the Custom Editor GUI field in the Graph settings that was ignored.
    
*   Shadergraph: Fixed the default dimension (1) for vector material slots so that it is consistent with other nodes. ([1328756](https://issuetracker.unity3d.com/issues/shadergraph-default-inputs-for-keyword-nodes-is-vec4s-even-though-they-become-floats-when-the-node-is-plugged-in))
    
*   Shadergraph: Fixed the incorrect value written to the VT feedback buffer when VT is not used.
    
*   Shadergraph: Fixed the InputNodes tests that were never correct. These were incorrect tests, no nodes needed tochange.
    
*   Shadergraph: Fixed the node searcher results to prefer names over synonyms. (1366058)
    
*   Shadergraph: Fixed the ordering of inputs on a SubGraph node to match the properties on the blackboard of the subgraph itself. ([1354463](https://issuetracker.unity3d.com/issues/shadergraph-instances-of-subgraph-nodes-are-not-updated-correctly-when-subgraphs-properties-are-reordered))
    
*   Shadergraph: Fixed treatment of node precision in subgraphs, now allows subgraphs to switch precisions based on the subgraph node ([1304050](https://issuetracker.unity3d.com/issues/precision-errors-when-theres-a-precision-discrepancy-between-subgraphs-and-parent-graphs))
    
*   Shadergraph: Fixed unhandled exception when loading a subgraph with duplicate slots. ([1366200](https://issuetracker.unity3d.com/issues/argumentexception-an-item-with-the-same-key-has-already-been-added-when-opening-shader-graph))
    
*   Shadergraph: Fixed virtual texture layer reference names allowing invalid characters ([1304146](https://issuetracker.unity3d.com/issues/shadergraph-virtual-texture-layer-reference-name-doesnt-sanitize-pasted-inputs))
    
*   Shadergraph: Node included HLSL files are now tracked more robustly, so they work after file moves and renames ([1301915](https://issuetracker.unity3d.com/issues/shadergraph-reference-to-hlsl-file-is-lost-after-moving-it-to-a-different-folder))
    
*   Shadergraph: ShaderGraph SubGraphs now report node warnings in the same way ShaderGraphs do. (1350282)
    
*   Shadergraph: Updated the ShaderGraph searcher package dependency to be in sync with the latest searcher package version i.e. 4.8.0.
    
*   Shaders: Added a LevelOfDetail read-only property to ShaderData.Subshader. ([1352774](https://issuetracker.unity3d.com/issues/not-possible-to-retrieve-lod-from-a-subshader))
    
*   Shaders: Added compute shader compilation logging during project builds or on "Compile and show code" usage. Added raytracing shader (.raytracing file) compile-time logging on import. ([1321684](https://issuetracker.unity3d.com/issues/compute-shader-compile-times-are-not-printed-to-the-editor-dot-log))
    
*   Shaders: Added missing PDB data output for DXC DX12 debug shaders for use in external analysis tools. ([1333848](https://issuetracker.unity3d.com/issues/pix-and-nsight-shader-debuggers-dont-work-on-dx12-with-dxc-compiled-shaders))
    
*   Shaders: Added tests for custom BFI and UBFE implementations in HLSLcc (1305543)
    
*   Shaders: Fixed ddx\_fine and ddx\_coarse on Vulkan and capable GLCore targets. ([1323892](https://issuetracker.unity3d.com/issues/fwidth-behavior-is-inconsistent-between-dx11-slash-dx12-and-opengl-slash-vulkan))
    
*   Shaders: Fixed DXC validator error on Windows that would result from using '#pragma require WaveMultiPrefix'. (1333695)
    
*   Shaders: Fixed editor crash if shader error db fails to open. ([1327429](https://issuetracker.unity3d.com/issues/editor-crashes-on-trying-to-open-project-on-a-very-long-path))
    
*   Shaders: Fixed inaccurate shader\_feature usage tracking with shader stage specific keywords. (1255901)
    
*   Shaders: Fixed Linux Editor SPIR-V validation error when returning OpArrayLength in Compute shader, by generating OpArrayLength with no signedness. ([1302657](https://issuetracker.unity3d.com/issues/vulkan-linux-editor-throws-a-spir-v-validation-error-when-returning-oparraylength-in-compute-shader))
    
*   Shaders: Fixed memory leaks in the shader compiler process when compiling ray tracing shaders. (1352198)
    
*   Shaders: Fixed PassIdentifier being erroneously invalid in some cases. (1348023)
    
*   Shaders: Fixed the "end of shader compiler log" printing to the editor log at compiler crashes if the compiler log is very small.
    
*   Shaders: It is now possible to determine which keywords are disabled in a given ShaderKeywordSet by using ShaderUtil.GetPassKeywords ([1338833](https://issuetracker.unity3d.com/issues/not-possible-to-determine-if-a-keyword-is-disabled-in-a-variant-used-for-stripping))
    
*   Shaders: Prevent editor crash on unlucky timing when a shader compiler process is being killed.
    
*   Shaders: ShaderUtil now has an API to retrieve an array of local keywords valid for a particular shader stage of a Pass and an API to check whether a given keyword is valid for a Pass or a shader stage of a Pass. ([1347380](https://issuetracker.unity3d.com/issues/shaders-shaderutil-dot-getpasskeywords-returns-array-which-is-not-efficient-for-searching-specific-keyword))
    
*   Terrain: Added compatibility tags used to distinguish terrain supported shaders. (1283086)
    
*   Terrain: Fixed Brush Preview rendering when a different hot control is active ([1276282](https://issuetracker.unity3d.com/issues/brush-previews-and-tool-functionality-should-be-disabled-while-user-is-using-scene-camera-controls))
    
*   Terrain: Fixed Brush Preview rendering when mouse is outside of SceneView bounds ([1281231](https://issuetracker.unity3d.com/issues/terrain-hovering-mouse-above-the-terrain-sliders-moves-brush-in-the-scene))
    
*   Terrain: Fixed incorrect conditional statement when validating terrain material shaders. ([1307951](https://issuetracker.unity3d.com/issues/terrain-inspector-is-suggesting-a-shader-which-doesnt-work))
    
*   Terrain: Fixed Terrain Tools package discoverability in Package Manager.
    
*   Terrain: Fixed texture atlas bleeding that occurred on details. Added half pixel offset for grass texture UVs, and collapsed uvs for detail meshes without textures. ([1268510](https://issuetracker.unity3d.com/issues/terrain-detail-meshes-have-dark-shadows-around-uv-seams))
    
*   Terrain: Moved TerrainCallbacks from UnityEngine.TerrainAPI to UnityEngine namespace.
    
*   Terrain: Performance improvement when adding many trees to a terrain. ([1225501](https://issuetracker.unity3d.com/issues/performance-regression-gameobject-dot-activateawakerecursively-noticeably-slower-when-rendering-trees-on-terrain))
    
*   Terrain: Tree Colliders are generated when entering playmode with EnterPlayModeOptions.DisableSceneReload set. ([1290587](https://issuetracker.unity3d.com/issues/there-are-no-collisions-between-the-trees-and-the-player-in-play-mode-when-enter-play-mode-options-experimental-is-enabled))
    
*   Terrain: Trees with LOD groups will not warn the user that they don't have an LOD group when they have a mesh renderer within them. ([1287964](https://issuetracker.unity3d.com/issues/terrain-when-painting-trees-and-selecting-a-tree-with-a-lod-group-a-warning-appears-that-it-does-not-have-a-lod-group))
    
*   Terrain: `Nature/Tree Soft Occlusion Leaves` Shader correctly supports the render paths scene view mode. ([1303714](https://issuetracker.unity3d.com/issues/wrong-scaling-in-the-render-paths-view-mode))
    
*   Tests: Fixed test failure EditorGUI.CanCloseNextWindowDuringOnDestroy on mac and linux platform. (992239)
    
*   Timeline: Fixed an issue where ScriptableObjects are not recognized as valid INotificationReceivers
    
*   TLS: MacOS TLS/SSL verification now checks also against (un)trusted certificates that were manually added to the keychain. ([1306147](https://issuetracker.unity3d.com/issues/curl-error-51-unitytls-x509verify-flag-not-trusted-when-making-a-request-to-the-server-using-self-signed-certificate))
    
*   uGUI: Fixed some UGUI editor fields not showing prefab override indicators. ([1290387](https://issuetracker.unity3d.com/issues/layout-group-component-properties-do-not-show-that-they-were-modified-when-they-are-modified-on-an-instanced-prefab))
    
*   uGUI: Fixed UI Components being selected when their child is selected. ([1067993](https://issuetracker.unity3d.com/issues/parent-and-child-buttons-are-highlighted-when-only-hovering-over-a-child-button))
    
*   uGUI: Fixed undesired values for the Scrollbar by clamping and rounding it. ([1312723](https://issuetracker.unity3d.com/issues/scrollbars-value-becomes-not-accurate-after-clicking-on-the-edges-of-the-scrollbar))
    
*   uGUI: UGUI: This PR fixes a CPU performance issue, were the UI re-renders from scratch every time we select a delayed floating point component (on the IMGUI stack).  
    The reason is quite simple, a floating point comparison between the string representation and the double value is incorrect, causing to always be false.  
    This in turn causes the UI to always be tagged as dirty, and unleashes draw calls / flushing and many bad performance issues on the Editor loop. ([1353802](https://issuetracker.unity3d.com/issues/fps-increases-after-reselecting-or-changing-dynamic-resolution-type-when-changing-dynamic-res-forced-screen-percent))
    
*   UI: Fixed an issue where a Unity GUI element would be stuck in the pressed state on resume. ([1236185](https://issuetracker.unity3d.com/issues/mobile-ui-button-stays-pressed-in-after-releasing-it-while-the-pull-down-menu-is-opened))
    
*   UI: Fixed duplicate USS files in the StyleSheets pane when editing-in-place (1299314)
    
*   UI: Fixed error in console when toggling isOn in inspector during playmode. ([1307257](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-when-toggle-component-is-toggled-in-inspector-window-using-is-on-field))
    
*   UI: Fixed for ScreenPointToWorldPointInRectangle API not returning a valid value when the point is on the plane. which is the case when the canvas plane is on the cameras near plane. ([1313831](https://issuetracker.unity3d.com/issues/recttransformutility-functions-with-out-vector-return-only-00-0-when-canvas-sits-exactly-on-the-nearclipplane-of-the-camera))
    
*   UI: Fixed issue where Canvas inspector would update incorrectly as the renderMode is based on the parentCanvas which is null when a Canvas is disabled. This lead to the inspector rendering the wrong options. ([1311169](https://issuetracker.unity3d.com/issues/the-sorting-layer-property-is-displayed-for-the-nested-canvas-when-the-canvas-component-is-disabled))
    
*   UI: Fixed issue where wrong aspect was used when a explicit aspect is assigned.
    
*   UI: Fixing hard to repo issue where serialization would be a issue due to reuse of serialized name. (1309777)
    
*   UI: Fixing issue where selecting the padding title for a graphic wouldn't expand the area. ([1308734](https://issuetracker.unity3d.com/issues/the-raycast-padding-section-doesnt-un-fold-when-clicking-on-the-raycast-padding-label-in-the-inspector))
    
*   UI: Make inputfield Text property multiline such that multiline input can be viewed easier when multiple lines are typed. (1300867)
    
*   UI Toolkit: 2021.2 Backport to UI Toolkit package of fix for 1351667: \[UI Builder\] Text Shadow Color resets to clear after reopening the project. ([1351667](https://issuetracker.unity3d.com/issues/ui-builder-text-shadow-color-resets-to-clear-after-reopening-the-project))
    
*   UI Toolkit: Added importedWithErrors and importedWithWarnings APIs to USS assets and UXML assets to differentiate between a failed import and an import of an empty file. ([1320914](https://issuetracker.unity3d.com/issues/loading-invalid-uxml-or-uss-returns-non-null-object))
    
*   UI Toolkit: Added missing asset conversion information for Text Core generated assets. ([1348577](https://issuetracker.unity3d.com/issues/ui-toolkit-package-asset-converter-is-missing-text-core-assets-conversion))
    
*   UI Toolkit: Added missing styling definition for dropdown in runtime stylesheet. (1314322)
    
*   UI Toolkit: Added support for RenderTexture for background-image in the UI Builder inspector. ([1320359](https://issuetracker.unity3d.com/issues/uibuilder-add-missing-support-for-rendertexture-to-the-style-inspector))
    
*   UI Toolkit: Added tooltip in StyleSheets pane when hovering a class selector that is trimmed (UI Builder) (1313198)
    
*   UI Toolkit: Allowed UIElements Debugger to pick elements from Game View outside of play mode
    
*   UI Toolkit: Changed EnumField+derivatives & BasePopupField-based classes to properly handle pointer down events ([1248669](https://issuetracker.unity3d.com/issues/quick-search-error-thrown-on-selecting-extension-folder-file-option-under-excludes-from-search-index-manager-window))
    
*   UI Toolkit: Changing choices programmatically after setting the value will show the correct selection, in RadioButtonGroup.
    
*   UI Toolkit: Child's reference is not renamed in parent UXML after renaming the child UXML file. ([1319903](https://issuetracker.unity3d.com/issues/ui-toolkit-childs-reference-is-not-renamed-in-parent-uxml-after-renaming-the-child-uxml-file))
    
*   UI Toolkit: Cleaned up the Theme menu. ([1318600](https://issuetracker.unity3d.com/issues/the-items-in-the-theme-dropdown-in-ui-builder-needs-some-cleanup))
    
*   UI Toolkit: Elements hover and focused states are not properly reset when attaching to a new hierarchy ([1287198](https://issuetracker.unity3d.com/issues/the-hover-state-stays-on-the-button-when-the-button-element-is-cleared-while-in-hover-state-and-loaded-in-later-again))
    
*   UI Toolkit: Ensured that only modified files are saved to disk. ([1355591](https://issuetracker.unity3d.com/issues/the-uxml-and-all-open-uss-files-get-marked-as-dirty-after-modifying-only-one-file))
    
*   UI Toolkit: Ensured that resizing by dragging Resize handles always produces dimensions with rounded values. ([1322550](https://issuetracker.unity3d.com/issues/ui-toolkit-ui-control-size-values-increase-after-setting-windows-display-scaling-to-150-percent-and-resizing-the-control))
    
*   UI Toolkit: Ensures the UI Builder no longer populate VisualElementAsset.stylesheetPaths when adding stylesheets. ([1299464](https://issuetracker.unity3d.com/issues/style-sheet-not-found-error-is-logged-in-player-dot-log-when-stylesheet-is-used-in-uxml-template))
    
*   UI Toolkit: Fix add component button is overlapping on Default Material after undoing added component ([1279830](https://issuetracker.unity3d.com/issues/undo-add-component-button-is-overlapping-on-default-material-after-undoing-added-component))
    
*   UI Toolkit: Fix Custom UIElements Inspector is editable when GameObject has its Flags set to NotEditable ([1306242](https://issuetracker.unity3d.com/issues/custom-uielements-inspector-is-editable-when-gameobject-has-its-flags-set-to-noteditable))
    
*   UI Toolkit: Fix PropertyField shows that it is actively selected when it has been disabled while being actively selected ([1306238](https://issuetracker.unity3d.com/issues/property-field-shows-that-it-is-actively-selected-when-it-has-been-disabled-while-being-actively-selected))
    
*   UI Toolkit: Fixed a bug where users were able to drag slider outside its container when a text field was present
    
*   UI Toolkit: Fixed a few problems with the showMixedValue property for BaseCompositeField:  
    
    *   Subfield's callback registration needs to be applied to the bind event, not the attach/detach panel event (see constructor code) -->; this fixes a problem with field recycling that did not respond after being recycled  
        
    *   Remove boxing and closure issues on the current implementation of the callback in question  
        
    *   We should not use ve.userData to store the SerializedProperty (userData should be reserved for the user, not the field), use SetProperty() instead  
        
    *   showMixedValue does not need to be set on BaseField.SetValueWithoutNotify; it is set later by binding styles code.
*   UI Toolkit: Fixed a logic error when deciding whether styles should be updated when the pseudo states change. (1348866)
    
*   UI Toolkit: Fixed adding templates in an empty document (UI Builder). (1322904)
    
*   UI Toolkit: Fixed an Error in the asset management of the StyleSheet that would show up in a build
    
*   UI Toolkit: Fixed an issue causing ListView's reordering to stop working after docking its parent window to a new pane. ([1345142](https://issuetracker.unity3d.com/issues/uielement-dot-listview-with-reorderable-enabled-in-editorwindow-cannot-be-reordered-when-docked-in-another-window))
    
*   UI Toolkit: Fixed animated reorderable ListView that was having broken item heights when they were dragged too fast. (1361734)
    
*   UI Toolkit: Fixed API inconsistency of the ScrollView class not exposing the "mode" as a property. (1328093)
    
*   UI Toolkit: Fixed bad bounding box calculation causing clicking on rotated elements sometimes resulting in no click. ([1345300](https://issuetracker.unity3d.com/issues/ui-toolkit-button-does-not-respond-to-clicks-correctly-when-rotated))
    
*   UI Toolkit: Fixed being able to paste USS Selectors from the Hierarchy pane and elements from the StyleSheets pane. Paste now works based on which pane is currently active. (UI Builder)
    
*   UI Toolkit: Fixed bug where multiple elements could be shown as being focused simultaneously due to delayed focus events not being well tracked when there is more than 1 of them in the queue. ([1154256](https://issuetracker.unity3d.com/issues/ui-elements-more-than-one-property-can-be-selected-after-opening-curve-editor))
    
*   UI Toolkit: Fixed bug where runtime cursor should not be reset unless it was overridden. ([1292577](https://issuetracker.unity3d.com/issues/ui-toolkit-the-customized-cursor-changes-back-to-default-after-moving-out-of-the-button))
    
*   UI Toolkit: Fixed ClickEvent unpredictably not being sent on Android and iOS when the touch sequence spans over multiple update frames. ([1359485](https://issuetracker.unity3d.com/issues/ui-toolkit-clickevent-is-not-triggered-when-the-button-is-pressed-for-a-longer-time))
    
*   UI Toolkit: Fixed clicking in empty space in Hierarchy pane not deselecting a USS Selector and vice-versa for the StyleSheets pane. (UI Builder)
    
*   UI Toolkit: Fixed clipping issue with nested scrollviews. (1335094)
    
*   UI Toolkit: Fixed clipping with large rects when under a group transform. ([1296815](https://issuetracker.unity3d.com/issues/ui-elements-enumfield-becomes-invisible-when-the-scrollview-contains-a-large-number-of-elements))
    
*   UI Toolkit: Fixed contentHash not being updated in UI Builder. ([1336924](https://issuetracker.unity3d.com/issues/ui-builder-visualtreeasset-dot-contenthash-is-not-updated-after-saving-when-uxml-files-uses-an-uss))
    
*   UI Toolkit: Fixed ContextMenu and Tooltip event handling for disabled elements. Allowed UIDebugger to select disabled elements and modified Panel.Pick to return them. Allows disabled PropertyField Foldouts to react to clicks by using a new (internal) Clickable.m\_AcceptClicksIfDisabled property. ([1306245](https://issuetracker.unity3d.com/issues/uitoolkit-it-is-not-possible-to-right-click-on-a-propertyfield-when-the-component-is-disabled))
    
*   UI Toolkit: Fixed corrupted atlas for Inter. ([1330758](https://issuetracker.unity3d.com/issues/uir-graphview-text-contains-artifacts-when-the-graph-is-zoomed-out))
    
*   UI Toolkit: Fixed cursor not updating when changing it using a variable which has hotspot data. ([1340471](https://issuetracker.unity3d.com/issues/ui-toolkit-cursor-not-updating-when-changing-it-using-a-variable-which-has-hotspot-data))
    
*   UI Toolkit: Fixed custom editor not showing as disabled for read-only inspectors (1299346)
    
*   UI Toolkit: Fixed custom element UXML factory not picked up in pre-compiled DLL. ([1316913](https://issuetracker.unity3d.com/issues/no-registered-factory-method-error-is-thrown-when-class-that-inherit-and-extend-an-uielement-is-used))
    
*   UI Toolkit: Fixed default clicking scroll amount in ScrollView. ([1306562](https://issuetracker.unity3d.com/issues/scroll-bar-scrolls-less-in-the-package-manager-packages-than-elsewhere-when-pressing-on-the-empty-scroll-bar-area-to-scroll))
    
*   UI Toolkit: Fixed directional navigation bug where some elements could be skipped during horizontal navigation. Improved choice of next element when multiple candidates are valid. ([1298017](https://issuetracker.unity3d.com/issues/uitoolkit-buttons-located-closest-to-the-side-dont-get-focused-when-going-through-the-focusable-button-list-with-arrow-keys))
    
*   UI Toolkit: Fixed document settings (like Canvas background and zoom) being reset when editing a sub-document in-place. (UI Builder)
    
*   UI Toolkit: Fixed dynamic atlas not being regenerated after downloading a texture from the cache server. ([1333693](https://issuetracker.unity3d.com/issues/uir-dynamic-atlas-doesnt-get-refreshed-when-importing-from-a-cache-server))
    
*   UI Toolkit: Fixed element highlight overlay not being reset after deleting the element. (UI Builder)
    
*   UI Toolkit: Fixed elements being added to the parent in builder hierarchy when editing a sub-document in place (UI Builder) ([1306104](https://issuetracker.unity3d.com/issues/ui-builder-it-is-possible-to-add-content-to-parent-document-while-editing-child-document-in-place))
    
*   UI Toolkit: Fixed empty name showing up in Memory Profiler for one of the UI Toolkit internal render texture ([1307441](https://issuetracker.unity3d.com/issues/children-of-rendertexture-have-empty-names-in-the-profiler-memory-module))
    
*   UI Toolkit: Fixed EventSystem using InputSystem package sometimes sending large amounts of PointerMoveEvents during a single frame. (1295751)
    
*   UI Toolkit: Fixed exception in ListView when pressing page up key after hitting navigation keys. ([1324806](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-pressing-pageup-key-after-a-directional-key-is-pressed-and-using-uidocument))
    
*   UI Toolkit: Fixed exception on Text Settings coming from uninitialized Line Breaking Rules when text wrap is enabled. ([1305483](https://issuetracker.unity3d.com/issues/nullreferenceexception-gets-thrown-in-the-console-when-the-label-text-value-contains-cjk-characters-and-text-wrap-is-enabled))
    
*   UI Toolkit: Fixed exception thrown when selecting the currently open UXML asset in the Project Window. (UI Builder)
    
*   UI Toolkit: Fixed ExecutiveCommand commandName being stripped when a sent event require a new layout pass. (1329303)
    
*   UI Toolkit: Fixed float and double attributes not being stored correctly in UXML as CultureInvariant. (UI Builder)
    
*   UI Toolkit: Fixed focus outline for the following controls: CurveField, GradientField, EnumField/PopupField (and derivatives), RadioButton (choice), ObjectField (when hovered). (1324381)
    
*   UI Toolkit: Fixed for unsetting min and max size in UI Builder. ([1322457](https://issuetracker.unity3d.com/issues/cannot-unset-min-slash-max-sizes-from-context-menu-when-right-clicking-on-the-words-min-or-max))
    
*   UI Toolkit: Fixed from UI Builder package 1.0.0-preview.13 to the editor.
    
*   UI Toolkit: Fixed GraphView shader not compiling on Shader Model <; 3.0. (1348285)
    
*   UI Toolkit: Fixed handling of a deleted StyleSheet that is being used by the currently open UXML UI Document. (UI Builder)
    
*   UI Toolkit: Fixed hover state remaining after a touch event on iOS and Android. UI Toolkit runtime now ignores simulated mouse events if no mouse is present on the device. ([1326493](https://issuetracker.unity3d.com/issues/ios-ui-toolkit-button-remains-in-hover-state-after-a-touch))
    
*   UI Toolkit: Fixed how the USS styles are applied: we now skip unknown properties instead of breaking when applying a style. ([1312500](https://issuetracker.unity3d.com/issues/uss-file-parsing-stops-when-it-encounters-an-unknown-css-parameter))
    
*   UI Toolkit: Fixed inconsistencies in the visuals of text underline/strikethrough. ([1349202](https://issuetracker.unity3d.com/issues/text-underline-is-not-a-straight-line))
    
*   UI Toolkit: Fixed infinite loop in CreateInspectorGUI if Editor contains a child InspectorElement targetting a different SerializedObject. ([1336093](https://issuetracker.unity3d.com/issues/uitoolkit-createinspectorgui-is-called-and-stacked-infinitely))
    
*   UI Toolkit: Fixed InspectorElement enabled state in EditorElement.Reinit (1221162)
    
*   UI Toolkit: Fixed InternalsVisibleTo for com.unity.ui.builder 1.0.0-preview.10
    
*   UI Toolkit: Fixed invalid property access after saving a document in UI Builder (UI Builder) ([1281537](https://issuetracker.unity3d.com/issues/a-childs-and-next-in-hierarchy-item-variables-swap-when-saving-the-ui-document-after-changing-the-childs-border-width))
    
*   UI Toolkit: Fixed issue where the layout of a document was getting corrupted after saved the document. (1348002)
    
*   UI Toolkit: Fixed issue where user could not override the text color and font-size of the Unity Default Runtime Theme using the ":root" or "VisualElement" selectors. ([1335507](https://issuetracker.unity3d.com/issues/runtime-themes-text-color-and-font-size-cannot-be-overridden-from-user-stylesheets-using-root-selector))
    
*   UI Toolkit: Fixed Label Element is not resized when Display Style is changed from None to Flex ([1293761](https://issuetracker.unity3d.com/issues/label-element-is-not-resized-when-display-style-is-changed-from-none-to-flex))
    
*   UI Toolkit: Fixed left-click not opening EnumField after using ContextMenu on MacOS. ([1311011](https://issuetracker.unity3d.com/issues/shadergraph-macos-node-dropdown-does-not-open-when-it-is-clicked-after-right-clicking-on-the-background))
    
*   UI Toolkit: Fixed ListView item selection through PointerMoveEvent, for example when holding right-click down while clicking. ([1287031](https://issuetracker.unity3d.com/issues/shadergraph-nodes-are-not-getting-created-after-applying-mouse-left-click-in-node-panel))
    
*   UI Toolkit: Fixed non-uniform scaling issues with UI Toolkit elements. (1336053)
    
*   UI Toolkit: Fixed non-whole pixel size and position values resulting from resizing or moving elements in the Viewport with the zoom set to 75%. (UI Builder)
    
*   UI Toolkit: Fixed not being able to create a single-character selector. (UI Builder)
    
*   UI Toolkit: Fixed not being able to rename USS Selectors directly inside the StyleSheets pane via double-click or the right-click menu.
    
*   UI Toolkit: Fixed null reference exception thrown when reimporting the uss while an unsaved uxml file is in the Builder. ([1298490](https://issuetracker.unity3d.com/issues/ui-builder-nullreferenceexception-error-is-thrown-on-saving-uxml-file-after-applying-changes-in-uss-file-importer-settings))
    
*   UI Toolkit: Fixed null reference exception when using the Align style properties on a USS Selector. (UI Builder)
    
*   UI Toolkit: Fixed NullReferenceException on turning UI Toolkit Live Reload on/off on maximized docked Search window ([1312367](https://issuetracker.unity3d.com/issues/uitoolkit-search-nullreferenceexception-is-thrown-on-enabling-ui-toolkit-live-reload-in-maximized-search-window))
    
*   UI Toolkit: Fixed NullReferenceException with using TrackPropertyValue on BindingExtensions for ExposedReference and Generic serialized property types ([1312147](https://issuetracker.unity3d.com/issues/ui-toolkit-nullreferenceexception-when-using-bindingextensions-dot-trackpropertyvalue))
    
*   UI Toolkit: Fixed older GraphView still relying on old idsFlags field
    
*   UI Toolkit: Fixed RadioButtonGroup and DropdownField choice attribute parsing in the UI Builder, when first added.
    
*   UI Toolkit: Fixed rebuild logic on inspectors with culled elements. ([1324058](https://issuetracker.unity3d.com/issues/createinspectorgui-gets-called-twice-when-a-custom-inspector-is-used-for-a-scriptableobject))
    
*   UI Toolkit: Fixed regression on the styling of the ProgressWindow's progress bars, removed usage of images in progress bar. (1297045)
    
*   UI Toolkit: Fixed scroll wheel event modifiers not assigned when using EventSystem and StandaloneInputModule combination in UI Toolkit. ([1347855](https://issuetracker.unity3d.com/issues/wheelevent-does-not-receive-modifiers-change-when-scrolling-mouse-wheel-and-holding-a-modifier-key))
    
*   UI Toolkit: Fixed scrollbar showing for no meaningful reason when the content of a scrollview is almost equal to the size of the scrollview. (1297053)
    
*   UI Toolkit: Fixed scrollview offset when Reordering the contents in hierarchy is not visible. (1341758)
    
*   UI Toolkit: Fixed selection on pointer up on mobile to allow touch scrolling. ([1312139](https://issuetracker.unity3d.com/issues/uitoolkit-listview-onselectionchange-conflicts-with-scrolling-on-touch-devices))
    
*   UI Toolkit: Fixed settings search not working for UI Builder settings in the Project Settings window. (UI Builder)
    
*   UI Toolkit: Fixed SVG triangle clipping issue (1288416)
    
*   UI Toolkit: Fixed TextCore visual artifacts caused by ddx/ddy glitches on AMD Radeon hardware. ([1317114](https://issuetracker.unity3d.com/issues/shader-graph-texts-in-new-shader-graph-are-blurred))
    
*   UI Toolkit: Fixed the default value used for applying rotation and scaling using the VisualElement.transform interface. Instead of always use the top left corner of the VisualElement, the operation are now centered around the transform-origin value, which is the center of the object by default.
    
*   UI Toolkit: Fixed the focus handling so elements not displayed in the hierarchy cannot be focused. (1324376)
    
*   UI Toolkit: Fixed the hover and pressed color of buttons in the Runtime theme ([1316380](https://issuetracker.unity3d.com/issues/vanilla-runtime-themes-buttons-need-better-visual-feedback-when-clicked))
    
*   UI Toolkit: Fixed the InvalidCastException thrown when assigning a built-in image asset to a Texture2D in the UI Builder inspector. (UI Builder)
    
*   UI Toolkit: Fixed the lack of feedback to users about problems with the UIDocument and PanelSettings inspectors. (1351792)
    
*   UI Toolkit: Fixed the missing Unicode arrow on ShaderGraph Transform Node. ([1333774](https://issuetracker.unity3d.com/issues/shadergraph-unicode-arrow-on-transform-node-no-longer-displays))
    
*   UI Toolkit: Fixed the refresh of the canvas's content when modifying properties of style selectors. (1323665)
    
*   UI Toolkit: Fixed the source path of template referenced in UXML getting cleared after saving ([1288918](https://issuetracker.unity3d.com/issues/errors-when-saving-the-ui-template-twice))
    
*   UI Toolkit: Fixed Toolbar shrinking when there is another element filling the parent container. ([1330415](https://issuetracker.unity3d.com/issues/scrollview-incorrectly-scales-elements-above-and-below-when-resizing-the-custom-window))
    
*   UI Toolkit: Fixed tooltip not showing in the UI Builder inspector. ([1346433](https://issuetracker.unity3d.com/issues/tooltips-are-not-displayed-when-hovering-over-labels-in-the-ui-builder-window))
    
*   UI Toolkit: Fixed ui builder layout broken when restarting unity. (1340218)
    
*   UI Toolkit: Fixed UIT-1340195 and UIT-1340189  
    
    *   Can't assign a none Font in UIBuilder.  
        
    *   Selecting a FontAsset to none in the UI Builder throws warnings.  
        
    *   Added test to check that it is possible to set both Font and FontAsset to none. ([1340189](https://issuetracker.unity3d.com/issues/selecting-a-fontasset-to-none-in-the-ui-builder-throws-warnings), [1340195](https://issuetracker.unity3d.com/issues/cant-assign-a-none-font-in-uibuilder))
*   UI Toolkit: Fixed view data persistence not working inside custom inspectors that use UI Toolkit. (1311181)
    
*   UI Toolkit: Fixed VisualElement contains "null" stylesheet after deleted uss file from project (1290271)
    
*   UI Toolkit: Fixed VisualElement doesn't render instantly after setting display property to flex through C#. ([1359661](https://issuetracker.unity3d.com/issues/display-flex-doesnt-make-element-visible-right-away))
    
*   UI Toolkit: Fixed window creator on linux caused a null reference and the new editor window was displayed corrupted. ([1295140](https://issuetracker.unity3d.com/issues/linux-ui-toolkit-nullreferenceexception-appear-on-enabling-the-open-files-in-editor-once-created-while-creating-ui-toolkit))
    
*   UI Toolkit: Fixed wrong runtime touch event coordinates on panels with scaling
    
*   UI Toolkit: Fixes 1304581: \[UIElements\] ArgumentException is thrown when the PropertyField is bind to the BuildTarget enum  
    Popup/Dropdown (Enum-compatible) fields now gracefully handle unselected/invalid values. ([1304581](https://issuetracker.unity3d.com/issues/uielements-argumentexception-is-thrown-when-the-propertyfield-is-bind-to-the-buildtarget-enum))
    
*   UI Toolkit: Fixes undo of a change of Sort Order field value for a UI Document. ([1337070](https://issuetracker.unity3d.com/issues/undoing-udocument-sort-order-does-not-take-effect))
    
*   UI Toolkit: Fixes \[UI Builder\] Saving a document that contains a one character name template fails. (1313509)
    
*   UI Toolkit: Implemented the missing support in the UI Builder for Rich Text' spacing USS properties.
    
*   UI Toolkit: Improved readability of USS import error/warnings. (1295682)
    
*   UI Toolkit: InputSystem fails to store ElementUnderPointer when a VisualElement is moving, creating flickering hover feedback. ([1306526](https://issuetracker.unity3d.com/issues/in-game-ui-element-under-mouse-is-reset-whenever-an-element-moves))
    
*   UI Toolkit: InspectorElement now correctly supports rebinding when used outside of the InspectorWindow ([1299036](https://issuetracker.unity3d.com/issues/inspectorelement-does-not-get-updated-when-using-bind))
    
*   UI Toolkit: Match text colors of UITK label and UITK field label with IMGUI label and IMGUI prefix label respectively. It also fixes the text color of buttons. ([1310581](https://issuetracker.unity3d.com/issues/uielements-text-color-is-different-from-imguis-text-color))
    
*   UI Toolkit: Missing theme style sheet on PanelSettings now gets logged to console.
    
*   UI Toolkit: Nested UI Document allowed changing the Panel Settings once. (1315242)
    
*   UI Toolkit: On Windows, the position obtained by the mouse event callbacks is as expected while the mouse is outside of the view even if the mouse down was applied while a temporary window such as a pulldown menu was already opened. (1324369)
    
*   UI Toolkit: Overlay, "Show Layout" now works for Runtime panels in Edit Mode (and not only in Play Mode like before)
    
*   UI Toolkit: Panels instantiated by PanelSettings assets now ordered deterministically when their sort order have the exact same value.
    
*   UI Toolkit: Prevented clicks from passing through runtime panels if they weren't used. ([1314140](https://issuetracker.unity3d.com/issues/ui-toolkit-click-event-passes-through-overlapping-uidocuments-visualelement))
    
*   UI Toolkit: Removed an extra step from the RadioButtonGroup focus navigation. (1324373)
    
*   UI Toolkit: Scroll bars now use display instead of visibility to avoid scroll bars being visible when parent visibility is set to false. ([1297886](https://issuetracker.unity3d.com/issues/ui-toolkit-scrollviews-scrollbar-remains-visible-after-setting-the-parent-elements-visibility-to-false))
    
*   UI Toolkit: Submit event on a ListView focuses in the content to allow keyboard navigation. ([1311688](https://issuetracker.unity3d.com/issues/ui-toolkit-listview-isnt-being-selected-when-clicking-submit-key))
    
*   UI Toolkit: Template references get deleted when the assets are moved. (1337112)
    
*   UI Toolkit: TextField text selection area is displayed incorrectly. ([1347904](https://issuetracker.unity3d.com/issues/ui-toolkit-textfield-text-selection-area-is-displayed-incorrectly))
    
*   UI Toolkit: The label of a focused Foldout now has its color changed. (1311200)
    
*   UI Toolkit: The UI Builder window's layout will not reset anymore when the window is reloaded (UI Builder).
    
*   UI Toolkit: This completes the MVP list of improvements to the UI Toolkit Event Debugger.
    
*   UI Toolkit: UQuery: Enumerator support allows for foreach iteration with no or minimal gc allocations
    
*   UI Toolkit: Value Change Callbacks for bound fields now happen after the value is applied to the target object. ([1321156](https://issuetracker.unity3d.com/issues/ui-elements-value-change-callbacks-for-bound-fields-happen-before-the-new-value-is-applied-to-the-fields))
    
*   Undo System: Ensure interested systems are updated after undoing RectTransform changes. (1116058)
    
*   Undo System: Improved performance when overwriting the redo stack.
    
*   Undo System: Prevent crashing when attempting to finalize an undo that is already being finalized. ([1352394](https://issuetracker.unity3d.com/issues/crash-after-recompilation-of-visual-scripting-package-update))
    
*   Undo System: Reduced register undo log. (1342970)
    
*   UNET: Fixed Multiplayer hlapi package is missing a declaration of its dependency on Physics2D. ([1324449](https://issuetracker.unity3d.com/issues/multiplayer-hlapi-package-is-missing-a-declaration-of-its-dependency-on-physics2d))
    
*   Universal: Fixed a case where shadow fade was clipped too early.
    
*   Universal: Fixed an issue in shaderGraph target where the ShaderPass.hlsl was being included after SHADERPASS was defined
    
*   Universal: Fixed an issue that caused shader compilation error when building to Android and using GLES2 API. (1343061)
    
*   Universal: Fixed an issue that caused shader compilation error when switching to WebGL 1 target. (1343443)
    
*   Universal: Fixed an issue that that caused a null error when creating a Sprite Light. ([1295244](https://issuetracker.unity3d.com/issues/urp-nullreference-exception-is-thrown-on-changing-light-type-under-light-2d-experimental-in-prefab-asset))
    
*   Universal: Fixed an issue where 2D lighting was incorrectly calculated when using a perspective camera.
    
*   Universal: Fixed an issue where Depth Prepass was not run when SSAO was set to Depth Mode.
    
*   Universal: Fixed an issue where motion blur would allocate memory each frame. ([1314613](https://issuetracker.unity3d.com/issues/urp-gc-alloc-increases-when-motion-blur-override-is-enabled-with-intensity-set-above-0))
    
*   Universal: Fixed an issue where SmoothnessSource would be upgraded to the wrong value in the material upgrader.
    
*   Universal: Fixed an issue where soft particles did not work with orthographic projection. ([1294607](https://issuetracker.unity3d.com/issues/urp-particles-are-rendered-behind-gameobjects-when-depth-texture-and-soft-particles-are-enabled-orthographic-camera-is-used))
    
*   Universal: Fixed an issue where SSAO would sometimes not render with a recently imported renderer.
    
*   Universal: Fixed an issue where the inspector of Renderer Data would break after adding RenderObjects renderer feature and then adding another renderer feature.
    
*   Universal: Fixed an issue where transparent objects sampled SSAO.
    
*   Universal: Fixed an issue where using Camera.targetTexture with Linear Color Space on an Android device that does not support sRGB backbuffer results in a RenderTexture that is too bright. (1307710)
    
*   Universal: Fixed an issue with backbuffer MSAA on Vulkan desktop platforms.
    
*   Universal: Fixed base camera to keep display index in sync with camera stacks for canvas. ([1291872](https://issuetracker.unity3d.com/issues/canvas-renders-only-on-the-display-1-when-its-set-to-screen-space-camera-or-world-space-and-has-overlay-type-camera-assigned))
    
*   Universal: Fixed base camera to keep display index in sync with camera stacks. ([1252265](https://issuetracker.unity3d.com/issues/universal-rp-overlay-camera-still-renders-to-display))
    
*   Universal: Fixed base camera to keep render texture in sync with camera stacks. ([1288105](https://issuetracker.unity3d.com/issues/srp-base-camera-rendering-to-render-texture-takes-overlay-camera-into-account-but-not-its-canvas))
    
*   Universal: Fixed base camera to keep viewport in sync with camera stacks. ([1311268](https://issuetracker.unity3d.com/issues/buttons-clickable-area-is-offset-when-canvas-render-camera-is-an-overlay-camera-and-viewport-rect-is-changed-on-base-camera))
    
*   Universal: Fixed Camera Inspector Stack list issues.
    
*   Universal: Fixed camera stack UI correctly work with prefabs. ([1308717](https://issuetracker.unity3d.com/issues/the-prefab-apply-slash-revert-menu-cant-be-opened-by-right-clicking-on-the-stack-label-under-the-camera-component-in-the-inspector))
    
*   Universal: Fixed double sided and clear coat multi editing shader.
    
*   Universal: Fixed issue causing missing shaders on DirectX 11 feature level 10 GPUs.
    
*   Universal: Fixed issue where copy depth depth pass for gizmos was being skipped in game view. ([1302504](https://issuetracker.unity3d.com/issues/urp-handles-with-set-ztest-do-not-respect-depth-sorting-in-the-game-view))
    
*   Universal: Fixed lit shader property duplication issue. ([1315032](https://issuetracker.unity3d.com/issues/shader-dot-propertytoid-returns-the-same-id-when-shaders-properties-have-the-same-name-but-different-type))
    
*   Universal: Fixed materials being constantly dirty.
    
*   Universal: Fixed multi editing of Bias property on lights. (1289620)
    
*   Universal: Fixed render pass reusage with camera stack on vulkan. ([1226940](https://issuetracker.unity3d.com/issues/vulkan-each-camera-stack-layer-generate-a-render-pass-separately-when-render-pass-are-the-same))
    
*   Universal: Fixed SafeNormalize returning invalid vector when using half with zero length. (1315956)
    
*   Universal: Fixed shadow cascade blend culling factor.
    
*   Universal: Fixed shadowCoord error when main light shadow defined in unlit shader graph.
    
*   Universal: Fixed undo issues for the additional light property on the UniversalRenderPipeline Asset. (1300367)
    
*   Universal: Normalized the view direction in Shader Graph to be consistent across Scriptable Render Pieplines.
    
*   Universal: SMAA post-filter only clear stencil buffer instead of depth and stencil buffers.
    
*   Universal Windows Platform: Fixed black square appearing with custom cursors in Executable Only build. ([1299579](https://issuetracker.unity3d.com/issues/uwp-ui-cursor-is-replaced-with-a-black-square-when-cursor-dot-setcursor-is-called-with-anything-but-the-default-cursor))
    
*   Universal Windows Platform: Fixed CultureInfo.CurrentCulture and CultureInfo.CurrentUICulture to return languages from the preferred UWP language list in system settings. It now matches .NET Native behavior. (1170029)
    
*   Universal Windows Platform: Updated UWP PlayerSettings API documentation. (1325420)
    
*   URP: Fixed a Universal Targets in ShaderGraph not rendering correctly in game view.
    
*   URP: Fixed additional camera data help url.
    
*   URP: Fixed additional light data help url.
    
*   URP: Fixed an issue in PostProcessPass causing OnGUI draws to not show on screen. ([1348882](https://issuetracker.unity3d.com/issues/ui-and-scene-view-fail-to-render-when-2d-renderer-data-has-post-processing-enabled))
    
*   URP: Fixed an issue where shadow artefacts appeared between cascades on Terrain Detail objects.
    
*   URP: Fixed an issue where ShadowCasters were sometimes being rendered twice in the editor while in playmode.
    
*   URP: Fixed an issue where Sprite type Light2Ds were missing a default sprite.
    
*   URP: Fixed an issue where Sprite type Light2Ds would throw an exeception if missing a sprite.
    
*   URP: Fixed an issue where TerrainLit was rendering color lighter than Lit. ([1340751](https://issuetracker.unity3d.com/issues/mobile-urp-gameobjects-with-terrainlit-shader-are-rendered-lighter-than-lit))
    
*   URP: Fixed an issue where the 2D Renderer was not rendering depth and stencil in the normal rendering pass.
    
*   URP: Fixed an issue where \_AfterPostProcessTexture was no longer being assigned in UniversalRenderer.
    
*   URP: Fixed an issue with the blend mode in Sprite-Lit-Default shader causing alpha to overwrite the framebuffer. ([1331392](https://issuetracker.unity3d.com/issues/urp-alpha-blend-is-incorrect-for-sprite-lit-default-shader-when-using-with-rendertexture))
    
*   URP: Fixed Camera rendering when capture action and post processing present. (1350313)
    
*   URP: Fixed CopyDepthPass incorrectly always enqueued when deferred rendering mode was enabled when it should depends on the pipeline asset settings.
    
*   URP: Fixed gizmos no longer allocate memory in game view. (1328852)
    
*   URP: Fixed graphical artefact when terrain height map is used with rendering layer mask for lighting.
    
*   URP: Fixed indentation of Emission map on material editor.
    
*   URP: Fixed issue where it will clear camera color if post processing is happening on XR. (1324451)
    
*   URP: Fixed issue with legacy stereo matrices with XR multipass. (1342416)
    
*   URP: Fixed memory leak with XR combined occlusion meshes.
    
*   URP: Fixed pixel perfect camera rect not being correctly initialized. ([1312646](https://issuetracker.unity3d.com/issues/pixel-perfect-camera-height-is-updated-on-the-third-frame))
    
*   URP: Fixed post processing to be enabled by default in the renderer when creating URP asset option. ([1333461](https://issuetracker.unity3d.com/issues/post-processing-is-disabled-by-default-in-the-forward-renderer-when-creating-a-new-urp-asset))
    
*   URP: Fixed remove of the Additional Camera Data when removing the Camera Component.
    
*   URP: Fixed remove of the Additional Light Data when removing the Light Component.
    
*   URP: Fixed renderer creation in playmode to have its property reloaded. (1333463)
    
*   URP: Fixed renderer post processing option to work with asset selector re-assing. ([1319454](https://issuetracker.unity3d.com/issues/urp-universal-renderer-post-processing-doesnt-enable-when-postprocessdata-reassigned-from-the-asset-selector-window))
    
*   URP: Fixed return values from GetStereoProjectionMatrix() and SetStereoViewMatrix(). ([1312813](https://issuetracker.unity3d.com/issues/xr-urp-begincamerarender-method-is-lagging-behind-when-using-urp))
    
*   URP: Fixed ShaderGraph materials to select render queue in the same way as handwritten shader materials by default, but allows for a user override for custom behavior. (1335795)
    
*   URP: Fixed shaderGraph shaders to render into correct depthNormals passes when deferred rendering mode and SSAO are enabled.
    
*   URP: Fixed soft shadows shader variants not set to multi\_compile\_fragment on some shaders (gbuffer pass, speedtree shaders, WavingGrass shader).
    
*   URP: Fixed sporadic NaN when using normal maps with XYZ-encoding. ([1351020](https://issuetracker.unity3d.com/issues/android-urp-vulkan-nan-pixels-and-bloom-post-processing-generates-visual-artifacts))
    
*   URP: Fixed UniversalRenderPipelineAsset now being able to use multiedit.
    
*   URP: Fixed unlit shader function name ambiguity.
    
*   URP: MaterialReimporter.ReimportAllMaterials and MaterialReimporter.ReimportAllHDShaderGraphs now batch the asset database changes to improve performance.
    
*   URP: Removed unsupported fields from Presets of Light and Camera. (1335979)
    
*   URP: Support undo of URP Global Settings asset assignation.
    
*   URP: URP Global Settings can now be unassigned in the Graphics tab. ([1343570](https://issuetracker.unity3d.com/issues/xpipeline-renderpipelineglobalsettings-cannot-be-unassigned))
    
*   URP: VFX: Compilation issue with ShaderGraph and planar lit outputs. ([1349894](https://issuetracker.unity3d.com/issues/urp-shadergraph-undeclared-identifier-builtinemissivecolor-error-when-assigning-a-lit-vfx-shadergraph-to-a-lit-urp-output))
    
*   URP: VFX: Fixed OpenGL soft particles fallback when depth texture isn't available.
    
*   URP: VFX: Fixed soft particles when HDR or Opaque texture isn't enabled.
    
*   Version Control: Fixed contextual menu not showing up in project view.
    
*   Version Control: Fixed some namespace collisions with Antlr3.
    
*   Version Control: Fixed SSO renew token after password change.
    
*   Version Control: Fixed view not switching to workspace after creating an Enterprise Gluon workspace.
    
*   Version Control: Renamed the CoreServices namespace so it doesn't conflict.  
    Fixed some situations where the history window would be blank.  
    Fixed missing Enterprise login link.  
    Fixed low resolution icons in light theme.
    
*   VFX Graph: Added a missing paste option in the context menu for VFX contexts. Also the paste options is now disabled when uneffective.
    
*   VFX Graph: An existing link can be remade.
    
*   VFX Graph: Blackboard fields can now be duplicated either with a shortcut (Ctrl+D) or with a contextual menu option.
    
*   VFX Graph: Compilation error undeclared identifier 'Infinity'. ([1328592](https://issuetracker.unity3d.com/issues/vfx-shader-errors-are-thrown-for-output-particle-quad-when-graph-contains-add-size-by-speed-block-with-matching-range-values))
    
*   VFX Graph: Compilation issue when normal is used in shadergraph for opacity with unlit output.
    
*   VFX Graph: Compilation issue while using new SG integration and SampleTexture/SampleMesh. ([1359391](https://issuetracker.unity3d.com/issues/undeclared-identifier-texture-a-error-when-connecting-a-sampletexture2d-operator-to-an-input-from-the-new-sg-integration))
    
*   VFX Graph: Deleting a context node and a block while both are selected throws a null ref exception.
    
*   VFX Graph: Don't open an empty VFX Graph Editor when assigning a VFX Asset to a Visual Effect GameObject from the inspector. ([1347399](https://issuetracker.unity3d.com/issues/vfx-assigning-an-empty-vfx-asset-to-vfx-game-object-results-in-a-duplicate))
    
*   VFX Graph: Enabled an optimization for motion vectors, storing projected positions for vertices instead of the transform matrix.
    
*   VFX Graph: Exception using gizmo on exposed properties. ([1340818](https://issuetracker.unity3d.com/issues/gizmos-all-exposed-shape-gizmos-break-and-throw-errors-upon-an-edit-attempt))
    
*   VFX Graph: Exposed Camera property fails to upgrade and is converted to a float type. ([1357685](https://issuetracker.unity3d.com/issues/exposed-camera-property-fails-to-upgrade-and-is-converted-to-a-float-type))
    
*   VFX Graph: Exposed Parameter placement can be moved after sanitize.
    
*   VFX Graph: Eye dropper in the color fields kept updating after pressing the Esc key.
    
*   VFX Graph: Eye dropper in the color fields kept updating after pressing the Esc key.
    
*   VFX Graph: Eye dropper in the color fields kept updating after pressing the Esc key.
    
*   VFX Graph: Fix CameraFade for shadow maps ([1294073](https://issuetracker.unity3d.com/issues/shadows-camera-fade-makes-vfx-shadow-casting-disappear-at-unexpected-ranges))
    
*   VFX Graph: Fix incorrect buffer type for strips.
    
*   VFX Graph: Fix unexpected Spawn context execution ordering.
    
*   VFX Graph: Fixed collision with depth buffer when using an orthographic camera ([1309958](https://issuetracker.unity3d.com/issues/vfx-teleports-to-the-camera-position-when-the-vfx-has-a-collide-with-depth-buffer-block-and-projection-is-set-to-orthographic))
    
*   VFX Graph: Fixed Collision with Depth Buffer when using Orthographic camera. ([1309958](https://issuetracker.unity3d.com/issues/vfx-teleports-to-the-camera-position-when-the-vfx-has-a-collide-with-depth-buffer-block-and-projection-is-set-to-orthographic))
    
*   VFX Graph: Fixed compilation failure on OpenGLES. ([1348666](https://issuetracker.unity3d.com/issues/vfx-opengles3-error-when-compiling-shaders-unexpected-token-number-at-kernel-csmain))
    
*   VFX Graph: Fixed crash when loading SDF Baker settings holding a mesh prefab. ([1343898](https://issuetracker.unity3d.com/issues/sdfbaker-unity-crash-when-switching-sdf-baker-saved-settings-containing-prefabs))
    
*   VFX Graph: Fixed culling of point output. ([1225764](https://issuetracker.unity3d.com/issues/output-selection-outline-shows-a-point-in-the-middle-of-the-scene-view-when-indirect-draw-is-off))
    
*   VFX Graph: Fixed Exception on trying to invert a degenerate TRS matrix. ([1307068](https://issuetracker.unity3d.com/issues/vfx-graph-vfxexpressioninversetrsmatrix-used-on-a-not-trs-matrix-exception-is-thrown-when-sample-sdfs-size-is-set-to-0))
    
*   VFX Graph: Fixed IsFrontFace shader graph node for VFX.
    
*   VFX Graph: Fixed issue with VFX using incorrect buffer type for strip data.
    
*   VFX Graph: GPU hang on some initialize dispatch during dichotomy (platform specific).
    
*   VFX Graph: In the Gradient editor undo will now properly refresh the gradient preview (color swatches).
    
*   VFX Graph: Inspector group headers now have a better indentation and alignment.
    
*   VFX Graph: Modified state in the VFX tab has now a correct state.
    
*   VFX Graph: Motion Vector map sampling for flipbooks were not using correct mips.
    
*   VFX Graph: Prevent out of sync serialization of VFX assets that could cause the asset to be dirtied without reason.
    
*   VFX Graph: Prevent vector truncation error in HDRP Decal template.
    
*   VFX Graph: Prevent VFX Graph compilation each time a property's min/max value is changed.
    
*   VFX Graph: Prevent vfx re-compilation in some cases when a value has not changed.
    
*   VFX Graph: Properties labels do not overlap anymore.
    
*   VFX Graph: Property Binder : Allow copy/past from a game object to another.
    
*   VFX Graph: Random crash using subgraph. ([1345426](https://issuetracker.unity3d.com/issues/editor-crashes-when-trying-to-create-subgraph-operator))
    
*   VFX Graph: Removed some useless compilation triggers (modifying not connected or disabled nodes for instance).
    
*   VFX Graph: Renamed "Material Offset" to "Sorting Priority" in output render state settings. ([1365257](https://issuetracker.unity3d.com/issues/vfx-unexpected-inconsistent-naming-of-sorting-priority-settings))
    
*   VFX Graph: Sample Mesh Color when value is stored as float.
    
*   VFX Graph: Sticky notes can now be deleted through contextual manual menu.
    
*   VFX Graph: Tidy up of platform abstraction code for random number generation, requires a dependency on com.unity.render-pipelines.core for those abstractions.
    
*   VFX Graph: Unexpected compilation error while modifying ShaderGraph exposed properties. ([1361601](https://issuetracker.unity3d.com/issues/vfx-graph-error-is-thrown-to-the-console-and-vfx-is-not-displayed-when-assigning-vector-property-to-shader-graphs-blocks))
    
*   VFX Graph: Unexpected operator and block removal during migration. ([1344645](https://issuetracker.unity3d.com/issues/vfx-sanitize-deletes-some-operators-slash-blocks))
    
*   VFX Graph: VFX Graph operators keep the same width when expanded or collpased so that the button does not change position.
    
*   VFX Graph: VFXEventBinderBase throwing a null reference exception in runtime
    
*   VFX Graph: VFXEventBinderBase throwing a null reference exception in runtime
    
*   VFX Graph: Visual Effect inspector input fields don't lose focus anymore while typing (Random seed).
    
*   VFX Graph: When adding a new node/operator in the graph editor and using the search field, the search results are sorted in a smarter way.
    
*   VFX Graph: Zoom and warning icons were blurry in the "Play Controls" and "Visual Effect Model" scene overlays.
    
*   Video: Fixed an issue where undoing a property in the Video Clip Import Settings also undoes the parent Transcode checkbox. ([1314433](https://issuetracker.unity3d.com/issues/undo-transcode-checkbox-gets-undone-together-with-any-of-the-child-checkboxes-that-are-shared-between-platforms))
    
*   Video: Fixed audio bitrate value for medium quality in MediaEncoder when channel count is more than 2.
    
*   Video: Fixed importing unsupported video frame size crashing the Editor. ([1340340](https://issuetracker.unity3d.com/issues/crash-on-windowsvideomedia-stepallstreams-when-reimporting-a-m4v-file))
    
*   Video: Fixed regression in applying standalone platform override settings for video clips. ([1360821](https://issuetracker.unity3d.com/issues/cant-apply-video-clip-importer-overrides-for-standalone-when-linux-standalone-support-is-installed))
    
*   Video: Fixed source Info text of the video asset that was barely visible. ([1328269](https://issuetracker.unity3d.com/issues/source-info-text-of-the-video-asset-is-barely-visible))
    
*   Video: Fixed Video Player's 5.1 audio channel layout being incorrect when outputting to Audio Source. ([1318983](https://issuetracker.unity3d.com/issues/macos-video-players-5-dot-1-audio-channel-layout-is-incorrect-when-outputting-to-audio-source))
    
*   Video: Increased VideoClipImporter version following a fix that adds missing platform dependencies in this importer.
    
*   Video: Videos encoded in 601 or 709 colourspaces will now be rendered in the correct colorspace. ([1185335](https://issuetracker.unity3d.com/issues/color-discrepancy-between-source-videoclip-and-videoplayer-output))
    
*   Video: \[audio/AVFoundation\] Low / Medium / High quality settings don't change the final audio bit rate. (1092549)
    
*   Video: \[audio\] webm/vp8/vorbis encoding does not use audio bitrate. (1092206)
    
*   Virtual Texturing: Completed requests now won't be incorrectly canceled if the last `InvalidateRegion` call is made before `PopRequests`.
    
*   WebGL: Added handling for Norwegian Bokmal and Nynorsk in SystemInfo for macOS and Linux, and to SystemInfo in Runtime/Misc used by WebGL and MetroPlayer.
    
*   WebGL: Enabled the URP feature SRP Batcher for WebGL 2. (1344614)
    
*   WebGL: Fix for URP scene being rendered incorrectly with the new texture subtarget options in the build settings. (1343208)
    
*   WebGL: Fixed a regression with building WebGL on Windows 7. ([1340260](https://issuetracker.unity3d.com/issues/webgl-fails-building-on-windows-7))
    
*   WebGL: Fixed audio restarting when paused and resumed on timeline. ([1204018](https://issuetracker.unity3d.com/issues/audio-restarts-on-webgl-when-pausing-and-resuming-the-timeline))
    
*   WebGL: Fixed bug in webgl publishing where doing multiple builds with the same project could sometime cause code from an older build to be mixed in with the new build, causing a crash on startup. ([1371445](https://issuetracker.unity3d.com/issues/webgl-macos-build-fails-to-launch-due-to-runtime-errors))
    
*   WebGL: Fixed FMOD related error messages showing up in console when audio is played on Timeline. ([1270635](https://issuetracker.unity3d.com/issues/webgl-fmod-error-spam-in-the-console-when-playing-an-audio-clip-in-a-timeline))
    
*   WebGL: Fixed handling of touch events. ([1349226](https://issuetracker.unity3d.com/issues/webgl-touch-events-do-not-work-when-in-built-player))
    
*   WebGL: Fixed hang on quit of the Unity Editor after a Build And Run of a WebGL project. (1352715)
    
*   WebGL: Fixed incorrect loading progress shown in Player when Brotli build compression is used. ([1288367](https://issuetracker.unity3d.com/issues/webgl-incorrect-loading-progress-is-shown-in-the-player-when-build-files-are-compressed-using-brotli))
    
*   WebGL: Fixed input coordinates when config.matchWebGLToCanvasSize is false. ([1325989](https://issuetracker.unity3d.com/issues/uncommenting-config-dot-matchwebgltocanvassize-equals-false-in-index-dot-html-makes-ui-elements-ignore-mouse-input))
    
*   WebGL: Fixed layout of WebGL template custom properties in the project settings. ([1316210](https://issuetracker.unity3d.com/issues/webgl-template-variables-are-inlined))
    
*   WebGL: Fixed Permission denied error during build ([1345412](https://issuetracker.unity3d.com/issues/webgl-build-fails-with-emscripten-permission-errors))
    
*   WebGL: Fixed Unity profiler auto-connect for WebGL builds. ([1360399](https://issuetracker.unity3d.com/issues/webgl-profiler-does-not-autoconnect-on-webgl-builds))
    
*   WebGL: Fixed video playback to be muted when Audio Output Mode is set to Audio Source and the selected Audio Source is Muted. Also fixed another issue where video clips that browser blocked from autoplaying would not start playing after user interacts with the web page. ([1241582](https://issuetracker.unity3d.com/issues/webgl-video-audio-is-being-played-when-videoplayers-audio-output-mode-is-set-to-none))
    
*   WebGL: Fixed video textures not getting converted to linear color space. ([1314263](https://issuetracker.unity3d.com/issues/webgl-colors-in-the-video-are-too-light-slash-incorrect-when-using-video-player-component-and-color-space-is-set-to-linear))
    
*   WebGL: Fixed WebGL pages on macOS with Safari 11. (1318420)
    
*   WebGL: Fixed WebGL project build when Exception support is None. ([1343976](https://issuetracker.unity3d.com/issues/webgl-cant-disable-exception-support-without-the-build-failing))
    
*   WebGL: Implement Accelerometer and Gyroscope sensor support for mobile WebGL ([1283206](https://issuetracker.unity3d.com/issues/webgl-android-gyroscope-does-not-work-relative-to-the-device-view-orientation-on-android-webgl))
    
*   WebGL: Implement Attitude Sensor support for mobile WebGL
    
*   WebGL: Implement Gravity Sensor support for mobile WebGL
    
*   WebGL: Implement Linear Acceleration Sensor support for mobile WebGL
    
*   WebGL: Improved Webcam backend with added support for mobile devices, improved performance and fixes issues with input device selection and other bugs. ([1273253](https://issuetracker.unity3d.com/issues/webcamtexture-dot-devices-field-is-not-updated-when-disconnecting-webcam-on-webgl-build))
    
*   WebGL: Show warnings when an embedded VideoClip is used with WebGL builds. Use Video Player component's URL option instead. ([1241263](https://issuetracker.unity3d.com/issues/webgl-no-warnings-slash-errors-are-thrown-in-editor-or-webgl-build-about-videoclip-being-unsupported-on-webgl-platform))
    
*   WebGL: Support mobile WebGL touch events to Immediate Mode GUI when the New Input System package is used. (1300223)
    
*   WebGL: The WebGL 1 Graphics API is now marked as deprecated and will be removed in a future release of Unity once all major browser vendors have released browser versions with WebGL 2 enabled by default. (1345140)
    
*   WebGL: WebGL1 shaders can fail to compile if they have large arrays. (1298096)
    
*   Windows: Fixed absolute mouse position when mouse acceleration is enabled. ([1221634](https://issuetracker.unity3d.com/issues/input-system-mouse-dot-current-dot-position-value-is-offset-by-1-pixel-compared-to-old-systems-input-dot-mouseposition))
    
*   Windows: Fixed input latency increasing by 1 frame when switching between exclusive fuilscreen and other fullscreen modes on D3D11 and D3D12 graphics APIs.
    
*   Windows: Fixed mouse position being off-by-1 pixel when rendering at lower than native resolution in certain cases.
    
*   Windows: Fixed performance issues caused by using a high input polling rate mouse (8000 Hz+). ([1336740](https://issuetracker.unity3d.com/issues/editor-slows-down-when-rapidly-moving-mouse-with-high-polling-rate-in-play-mode))
    
*   Windows: Fixed resolution resetting to native resolution on primary window when trying to move the secondary window use Display.SetParams.
    
*   Windows: Fixed Windows player infrequently deadlocking when changing fullscreen modes on D3D11 and D3D12 graphics APIs.
    
*   Windows: Fixed Windows standalone player misdetecting whether it's running at native resolution and as a result reopening in wrong resolution if the native resolution changes between runs.
    
*   Windows: Round Resolution.refreshRate. ([1318053](https://issuetracker.unity3d.com/issues/resolutions-returned-by-screen-dot-resolutions-differ-between-editor-and-build))
    
*   XR: Enabled Vulkan lazy allocation for memory savings on Oculus Quest.
    
*   XR: Fixed an issue where terrain tree shadows would be culled when they are still in view. ([1234785](https://issuetracker.unity3d.com/issues/xr-xr-sdk-tree-shadows-disappear-when-edge-of-fov-is-reached))
    
*   XR: Fixed differences between single pass instancing on Vulkan and D3D11 when using the MockHMD. (1287075)
    
*   XR: Fixed issue that XRSettings.gameViewRenderMode did not work when using a Scriptable Render Pipeline. ([1279033](https://issuetracker.unity3d.com/issues/xr-sdk-hdrp-xrsettings-dot-gameviewrendermode-does-not-change-game-view-render-mode))
    
*   XR: Fixed issue when enabling multiview when using single pass instanced rendering mode on PC.
    
*   XR: Fixed occlusion mesh displaying when stereo is disabled. ([1307273](https://issuetracker.unity3d.com/issues/xr-sdk-mockhmd-secondary-camera-does-not-render-into-full-render-texture))
    
*   XR: Fixed subsystem manifest json files not being found when using patch and run on Android. (1349953)
    
*   XR: Fixed XR Interaction Toolkit not appearing in the Package Manager window even when pre-release packages are enabled.
    
*   XR: Fixed XRDevice.fovZoomFactor not working in URP and HDRP. (1278072)
    
*   XR: Fixed XRSettings.occlusionMaskScale not working in SRPs.
    
*   XR: Fixed XRSettings.showDeviceView not working in SRPs.
    
*   XR: Fixed XRSettings.useOcclusionMesh not working in SRPs.