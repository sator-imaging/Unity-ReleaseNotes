# Unity 2020.2.0

https://unity3d.com/unity/whats-new/2020.2.0

## Final 2020.2.0f1 Release Notes

- [Features](#features)
- [Improvements](#improvements)
- [Changes](#changes)
- [API Changes](#api-changes)


### Features

*   2D: Added C# job tessellation support for the Sprite Shape's _Fill Area_.
    
*   Android: Improved support for playing video in addressables and AssetBundles. Compressed and in-memory bundles are now supported on Android 9 and newer devices.
    
*   Animation: Verified [Animation Rigging](https://docs.unity3d.com/Packages/com.unity.animation.rigging@latest) package version 1.0.3.
    
*   Asset Pipeline: Added Safe Mode for startup, which gives you the option to avoid asset importing when there are script compilation errors.  
    
    ![](/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif)
    
*   Asset Pipeline: Added two new properties to the _Asset Pipeline_:  
    
    *   `AssetDatabase.GlobalArtifactDependencyVersion`  
        
    *   `AssetDatabase.GlobalArtifactProcessedVersion`.
*   Asset Pipeline: Enabled consistency checking of assets using `-consistencyCheck` on the command-line and when force reimporting through the Project window.
    
*   Editor: Added a `-version` argument to command-line inputs that prints the current version of Unity to the console.
    
*   Editor: Added an `EditorToolContext` class to allow custom tools to override built-in transform tools. See [EditorToolContext](https://docs.unity3d.com/2020.2/Documentation/ScriptReference/EditorTools.EditorToolContext.html).
    
*   Editor: Added button _Enable debugging to all projects_ to the dialog box _C# Debugger Attached_, and made text more descriptive.
    
*   Editor: Added support for a Root Namespace field in Assembly Definition files. New scripts created inside Unity have a namespace in the default template if it is set in the corresponding Assembly Definition file (or for non-Assembly Definition file scripts, the _Project Settings_ > _Editor_ > _Project Root_ namespace).  
    
    ![](/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif)
    
*   Editor: Added support for importing texture arrays (`Texture2DArray`) and volume textures (`Texture3D`) from "flipbook" image layouts. To use this, open the Texture Importer and see the _Shape_ setting.  
    
*   Editor: Added support for Roslyn reference assemblies. Unity skips compilation of assembly references if the metadata for the modified assembly does not change when compiling scripts for the editor. Reference assemblies are enabled by default; to disable them, open the Player settings and disable _Use Reference Assemblies_.
    
*   Editor: Added the ability to optionally drag all the edges from one port to another at the same time.
    
*   Editor: Added the ability to toggle `GraphView` snap lines on or off in _Preferences_. If enabled, `GraphElements` in `GraphViews` align with one another when moved. If disabled, `GraphElements` move freely.
    
*   Editor: Modified the built-in Visual Studio C# solution generator to include Root Namespace from Assembly Definition Files in generated C# project files.
    
*   Editor: Renamed `auto_quitter` to `UnityAutoQuitterauto_quitter` on all platforms and made it a native program on MacOS and Linux.
    
*   Editor: Updated ProBuilder version to 4.3.1.
    
*   Editor: Updated [ProBuilder](https://docs.unity3d.com/Packages/com.unity.probuilder@4.2/manual/index.html) to version 4.2.3.
    
*   Editor: Verified [Editor Coroutines](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@latest) package version 1.0.0.
    
*   Editor: Verified [Profile Analyzer(com.unity.performance.profile-analyzer)](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@latest) package.
    
*   GI: Added support for blue noise sampling (as described in Eric Heitz and Laurent Belcour's [SIGGRAPH 2019 talk](https://eheitzresearch.wordpress.com/762-2/)).
    
*   Graphics: Added an experimental `ExternalGPUProfiler` capture API that allows users to programmatically take GPU frame captures using supported GPU debugging tools. See [ExternalGPUProfiler](https://docs.unity3d.com/2020.2/Documentation/ScriptReference/Experimental.Rendering.ExternalGPUProfiler.html).
    
*   Graphics: Added an option to evict data in a region. The original invalidate now keeps the original "stale" data on your graphics hardware until refreshed.
    
*   Graphics: Added an `ExtensibleCamera` class that inherits properties from the `Camera` class.
    
*   Graphics: Added Custom Render Texture API, so you can write your own update loop in C#.
    
*   Graphics: Added support for importing 16-bit per-channel integer formats without quantization. This also exposed new `TextureFormats` R16G16, R16G16B16 & R16G16B16A16.
    
*   Graphics: Added support for Virtual Texturing for Linux Standalone player.
    
*   Graphics: Added the ability to output a CPU event and get it back to the component level.
    
*   Graphics: Added the Virtual Texturing Profiler module to the Unity Profiler, which you can use to get performance information about the Virtual Texturing system.
    
*   Graphics: Added trilinear filtering support for procedural VT.
    
*   Graphics: Added Virtual Texturing support on the Universal Windows Platform.
    
*   IL2CPP: Added `Il2CppEagerStaticClassConstructionAttribute`, which can help to avoid performance impact associated with static constructors.
    
*   Linux: Added VTune integration support for Linux.
    
*   macOS: Added support for native Apple Silicon and macOS Universal 2 builds.  
    
*   Mobile: Added Adaptive Performance settings.
    
*   Mobile: Verified [Adaptive Performance](https://docs.unity3d.com/Packages/com.unity.mobile.adaptiveperformance@latest) package version 2.0.0.
    
*   Package Manager: Added a UI for users to manage their Scoped Registries from inside the Editor. Also added a popup alert for when Scoped Registries are added to their project from outside that Scoped Registries management UI. The Scoped Registries management UI automatically opens when the popup appears.  
    
    ![](/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif)
    
*   Package Manager: Added advanced Project Settings for the Package Manager.
    
*   Package Manager: Added an option on the Asset Store Has Moved window to skip it in future. If enabled, this setting opens the Asset Store directly in the browser when clicking on _Window > Asset Store_, and the user will not see the Asset Store Has Moved window again once they close it.
    
*   Package Manager: Added support for distinguishing between operation and state errors.
    
*   Package Manager: Added the **Pause** and **Resume** buttons when downloading Asset Store packages in the **My Assets** context in the Package Manager.
    
*   Package Manager: Added the ability to extract any hyperlinks and display them as text in an Asset Store package description (when in **My Assets** list context). This allows the user to copy them so they can still visit the page (until hyperlinks are supported in descriptions).
    
*   Package Manager: Added the Preview Packages in Use dropdown menu.
    
*   Package Manager: Added `changelogUrl` and `licensesUrl` as optional properties that can be specified in the `package.json` of a custom package. If specified, the auto-generated changelog and license links will be replaced with custom URLs.
    
*   Package Manager: Introduced two new environment variables to override the user and global configuration file path. `UPM_GLOBAL_CONFIG_FILE` overrides the default path to the global configuration file, and `UPM_USER_CONFIG_FILE` overrides the default path to the user configuration file.
    
*   Package Manager: Made console log errors from Package Manager UI clearly specify that they are from \[Package Manager Window\]. Also modified error messages in the UI so that they do not prompt the user to 'see console for more details' if no details are logged in the console.
    
*   Package Manager: Modified the appearance of the Package Manager window to highlight preview packages.
    
*   Package Manager: Modified the package details interface to display the full version of a package, including tags. Removed the '(Current)' note from the release details view of UPM packages.
    
*   Package Manager: Modified the package details interface to display the installation path for locally installed packages.
    
*   Package Manager: Modified the refresh button in the Package Manager window to a drop-down that selects the type of refresh to perform.
    
*   Package Manager: Moved the _Enable Preview Packages_ option in the Package Manager Project Settings window.
    
*   Package Manager: Split the Package Name into Name and Organization.
    
*   Particles: Added Local and Shape Scaling Mode support when using Mesh Renderer and Skinned Mesh Renderer in the Shape module.
    
*   Particles: Modified the Triggers module to query which colliders a particle is interacting with.
    
*   Physics: Expose `Joint.connectedArticulationBody` to be able to link `ArticulationBody` and `Rigidbody` hierarchies together with regular joints.
    
*   Player: Added the ability to pull Unity Player logs after test runs.
    
*   Prefabs: Added support for a Prefab post-processor.
    
*   Profiler: Added the Module Editor, which supports the creation of custom Profiler modules the ability to add charts to the Profiler for either existing or user generated Profiler statistics.
    
*   Scripting: Added support for Roslyn analyzers in Unity projects.  
    
    ![](/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif)
    
*   Scripting: Added support for script compilation with C# 8.
    
*   Services: Added Services Window support for the Unity Distribution Portal.  
    
    ![](/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif)
    
*   Shaders: Added scriptable stripping support for compute shaders.
    
*   Shaders: Implemented Shader Live-Link support.
    
*   Shaders: Modified shader preprocessors so that they can be overriden on a per-shader basis.
    
*   UI Toolkit: Added the asset type `ThemeStyleSheet`.
    
*   UI Toolkit: Added `TwoPaneSplitView` control.
    

### Improvements

*   2D: Added a **Detect Contiguous Tiles** toggle to GridBrush when you do a FloodFill. The toggle only changes contiguous Tiles when enabled, and all Tiles of the same type when disabled.
    
*   2D: Added a Copy, Paste and Paste All functionality to the Outline and Physics Shape modules for the Sprite Editor.
    
*   2D: Added ability to delete a selection of Tiles with the Delete/Backspace key when you select Tiles with the Select tool.
    
*   2D: Added ability to specify Corners properties.
    
*   2D: Added custom axis sort to the Tile Palette asset to allow users to show Tiles in the Tile Palette that the custom axis sorts.
    
*   2D: Added message to inform user about dependent packages when they view certain sample Scenes in the Animation package.
    
*   2D: Added support for SpriteShape meshes to be precomputed.
    
*   2D: Added Transform Gizmos for making Transform changes to a Grid Selection for a Scene view.
    
*   2D: Adjusted the length of the popup and value fields for the Skinning Module's _Weight Slider_ window.
    
*   2D: Implemented repainting of the Tile Palette when you make changes to a Grid Selection for a Tile Palette.
    
*   2D: Improved deformation performance when Collection and Burst package is installed.
    
*   2D: Improved Memory Allocations.
    
*   2D: Improved performance in SceneView for SceneViewOpenTilePaletteHelper.
    
*   2D: Improved performance of TilemapRenderer Individual mode.
    
*   2D: Improved the memory and speed of `Animation.SpritePostProcess` when used for a large sprite count.
    
*   2D: Improved the organization of the 2D Menus to allow for easier creation of default assets and GameObjects. This will improve user experience in level white boxing and prototyping.
    
*   2D: Improved the Sprite Skin Editor UI.
    
*   2D: Improved user experience of FloodFill tool from the Tile Palette when previewing the results of FloodFill.
    
*   2D: Updated 2D template to use current verified version of 2D packages.
    
*   2D: Updated Bone Influence window to allow you to rearrange the order of bones in the Sprite Skin Inspector.
    
*   AI: Added tooltips to Navigation window and related components. ([970778](https://issuetracker.unity3d.com/issues/navmesh-tool-tips-are-missing-for-navmesh-agent))
    
*   Android: Added anti-piracy measures which print your Company Name and Product Name in the log during application start. This can be used to prove that the game is yours if someone pirates it.
    
*   Android: Added support for compressed 3D textures with OpenGL ES 3.1.
    
*   Android: Added support for Vulkan backbuffer pre-rotation.
    
*   Android: Added target display support for Android.
    
*   Android: Added update so that frame rate is decided automatically when optimized frame pacing is enabled and Vsync is disabled.
    
*   Android: Enabled support for Light Probe proxy volumes when using OpenGL ES 3.
    
*   Android: Improved documentation for Application.targetFrameRate behavior on mobile devices.
    
*   Android: Improved logging when you try to find a plugin that is missing. ([1268172](https://issuetracker.unity3d.com/issues/android-unable-to-find-lib-burst-0-0-and-burst-0-0-message-logged-when-burst-is-enabled))
    
*   Android: Improved `Application.genuine implementation`, so it checks that the package name set in Player Settings matches with the one acquired at runtime.
    
*   Android: Improved `Screen.currentResolution.refreshRate` to correct itself if the display refresh rate changes.
    
*   Android: Improved `Screen.resolutions` to include supported display resolutions for 4K detection. ([1178233](https://issuetracker.unity3d.com/issues/mobile-systemwidth-isnt-set-to-renderingwidth-or-currentresolution-dot-width))
    
*   Android: Moved `noCompress` settings from launcher project to `unitylibrary`. (1239760)
    
*   Android: Optimized async texture readback and CopyTexture when using Vulkan on Mali GPUs.
    
*   Android: Updated [Android Logcat](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.2/manual/index.html) package to version 1.1.1.
    
*   Animation: Improved warnings for animated property curve names by minimizing false-positives and lessening repeated logs.
    
*   Animation: Localized some terms in the Animation window.
    
*   Asset Import: Added support for 3DsMax's Simplified Physical Material from FBX files in the Model Importer.
    
*   Asset Import: Asset previews are generated as a separate step after importing an asset.
    
*   Asset Import: Improved search speed when using glob syntax to search project assets.
    
*   Asset Import: Improved UV unwrapper performance.
    
*   Asset Import: Made `AssetDatabaseExperimental.SetImporterOverride` accessible from the Inspector. You can now access it in any Asset Importer header by selecting an available Importer Override to apply.
    
*   Asset Pipeline: Improved the adb Profiler output in the Editor log so it only gives necessary information.
    
*   Asset Pipeline: Removed unnecessary additional domain reloads associated with asset import workers.
    
*   Asset Pipeline: Unity no longer needs to reimport all textures, audio, and video when switching between Standalone platforms (for example, Win32 to Win64, or Mac to Linux).
    
*   Asset Pipeline: Updated progress dialog to display more precise information when asset postprocess callbacks take a long time to finish. (1228418)
    
*   Asset Pipeline: Updated source asset dependencies to use both file hash and timestamp to decide when to reload an asset.
    
*   Audio: Updated audio previews so that they stop when Unity loses focus and _Run in Background_ is disabled.
    
*   Bug Reporter: Updated `services-config.json` to add ability to set Bug Reporter defaults for _Publicity_ and _CustomerEmail_, and to set whether to exclude project files.
    
*   Build Pipeline: Added support to obtain GameCore redist DLLS from locally installed MSVC instances.
    
*   Burst: Added support for External symbols on a platform that required it.
    
*   Core: Improved Time.deltaTime consistency for the Metal graphics API on iOS and macOS.
    
*   DX12: Added support for constant buffers set with the `CommandBuffer.SetGlobalConstantBuffer` and `Shader.SetGlobalConstantBuffer` methods in Ray Tracing Shaders. Fixed and improved all the Ray Tracing-related Scripting API documentation.
    
*   DX12: Added support for GraphicsBuffer constant buffers that can be set using `ComputeShader.SetConstantBuffer` and `CommandBuffer.SetComputeConstantBufferParam`.
    
*   DX12: Added support for GraphicsBuffer constant buffers that can be set using `RayTracingShader.SetConstantBuffer` and `CommandBuffer.SetRayTracingConstantBufferParam`.
    
*   DX12: Ensured that values are only filled in for available channels when reading vertex attributes from vertex buffers (closest hit / any hit shaders). Unavailable channel values do not default to 0.
    
*   DX12: Improved CPU performance when binding raytracing shaders.
    
*   DX12: Improved CPU performance when building Ray Tracing Acceleration Structures.
    
*   DX12: Improved CPU performance when dispatching Ray Tracing Shaders.
    
*   DX12: Updated skin pose buffer to use scratch buffer memory, so that updates do not trigger an upload operation.
    
*   Editor: Added "Set as Default" option to Hierarchy objects so that users can set a custom parent GameObject for GameObjects they drag into the Scene/Hierarchy windows, and GameObjects they create via the GameObject menu.
    
*   Editor: Added a label displaying how many Game Objects are currently selected in the Inspector. (1208698)
    
*   Editor: Added a new naming scheme option to Editor Settings. This is set to _Prefab (1)_ by default, or you can choose _Prefab.1_ or _Prefab\_1_.
    
*   Editor: Added ability to copy and paste arrays and user-written serializable classes and structs in the Inspector.
    
*   Editor: Added ability to create keyboard shortcuts to copy and paste camera positions. In the shortcut settings, these are _Scene View/Copy Camera Placement_, _Scene View/Paste Camera Placement_ and _Game View/Copy Camera Placement_. No default keys are assigned.
    
*   Editor: Added optional "thickness" parameter functions for `Handle`: `DrawLine`, `DrawWireDisc` and `DrawWireArc`, for drawing thick handles.
    
*   Editor: Added Recent Scenes to the File menu in the Toolbar.
    
*   Editor: Added shift + select functionality to various tree view windows (e.g. Hierarchy, Project) to enable you to select multiple items without deselecting previously selected items.
    
*   Editor: Added support for Ray Tracing Shader (DX12) which sends information to the Frame Debugger.
    
*   Editor: Added support for the Scene view's _Shaded Wireframe_ mode to work with SRPs, via `ScriptableRenderContext.DrawWireOverlay`.
    
*   Editor: Added support for Undo and Redo for moving and renaming assets in the Project view.
    
*   Editor: Added support for `GradientFields` and Gradient editor to have their color interpreted as linear.
    
*   Editor: Added the ability to use Ctrl+C on a focused progress dialog in Windows Editor to copy the progress text to clipboard.
    
*   Editor: Added the command line argument "vcsModeSession", which sets VCS mode for the current Editor session only. ([1226304](https://issuetracker.unity3d.com/issues/vcsmode-cli-argument-writes-to-projectsettings-slash-editorsettings-dot-asset))
    
*   Editor: Added tooltips to Editor status bar icons.
    
*   Editor: Enhanced the **Open** context menu so that it expands the folders in One Column Layout in the Project Browser. ([1243843](https://issuetracker.unity3d.com/issues/folders-are-opening-when-trying-to-open-them-from-editor))
    
*   Editor: Improved how assert user messages are displayed in the Console view, so the user message for an assert can be read in the Console without needing to look at expanded details.
    
*   Editor: Improved inspector performance for large text asset files. ([1241212](https://issuetracker.unity3d.com/issues/editor-keeps-repainting-continuously-when-selecting-a-txt-file-that-contains-binary))
    
*   Editor: Improved Move/Rotate/Scale handles: thicker lines, brighter colors, increased movement accuracy, better visibility, and other UI improvements.
    
*   Editor: Improved performance of Scene hierarchy when you select GameObjects in the Project view. (1252528)
    
*   Editor: Improved progress bar details for texture importing, including details on crunch compression and cubemap convolution.
    
*   Editor: Improved Project Browser window to show asset file path whilst in One Column mode. ([1200880](https://issuetracker.unity3d.com/issues/assets-path-is-not-shown-when-using-one-column-layout-in-the-project-window))
    
*   Editor: Improved ray direction calculations so they are relative to the camera instead of a direction in world space. This should significantly improve precision when interacting with handles far away from the origin. (1178966)
    
*   Editor: Improved script creation so that Unity no longer writes a UTF8 BOM to new scripts it creates. This removes problems that BOM's can cause with tools such as source control.
    
*   Editor: Improved scripting defines list cut/copy/paste functionality. (1287729)
    
*   Editor: Improved scroll smoothness in Editor in macOS.
    
*   Editor: Improved the Layouts menu and dialogs. Layout deletion is now under a submenu and has a confirmation dialog. Save layout now has a confirmation dialog when overwriting an existing layout. The menu item "Revert Factory Settings" has been renamed to "Reset All Layouts". The Layouts dropdown in main toolbar is wider. Save Layout to File now shows the file in file explorer.
    
*   Editor: Improved the time taken for mobile ETC/ETC2/EAC texture compression.
    
*   Editor: Improved `JobsDebugger` performance.
    
*   Editor: Minimized allocations when calculating bounds for the _Rect Tool_.
    
*   Editor: Modified prefabs in the Hierarchy window so that certain Version Control state icons (Out of Sync, Conflicted, Remote Locked, Remote Delete, Remote Checkout) will be displayed (if enabled in the Project Settings window).
    
*   Editor: Optimized Gizmo rendering; now is ~5x faster when many gizmos are visible.
    
*   Editor: Optimized style catalog asset post-processing. (1222761)
    
*   Editor: Released [Quick Search](https://docs.unity3d.com/Packages/com.unity.quicksearch@1.1/manual/index.html) package version 1.5.3 with minor fixes, and improved test stability regarding Asset Store.
    
*   Editor: Removed redundant preview packages message from the title bar.
    
*   Editor: Replaced the text field for Scripting Define Symbols in Project Settings with a foldout string array.
    
*   Editor: Updated Frame Selected so that pressing it a second time focuses on the GameObject's handle/gizmo.
    
*   Editor: Updated Inspector so that you can re-order arrays and lists. To enable this, use the `[Reorderable]` attribute on your script variables.
    
*   Editor: Updated Mesh Inspector to add _Pan_, _Zoom_ and _Blendshape Preview_.
    
*   Editor: Updated Polybrush to 1.0.2.
    
*   Editor: Updated Quick Search to 2.0.  
    
    ![](/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif)
    
*   Editor: Updated Scene View to accept multiple objects when dragging and dropping.
    
*   Editor: Updated Settings Provider example and doc.
    
*   Editor: Updated the Game View resolution dropdown for Standalone platform with a more comprehensive list of default aspect ratios (16:9, 16:10) and resolutions (1920x1080, 1366x768, 2560x1440, 3840x2160).
    
*   Editor: Updated the material preview in the Inspector to remember the last used preview mesh.
    
*   Editor: Updated the Quick Search window to version 1.5.2, including minor fixes and improved performance.
    
*   Editor: Updated the UI for background tasks and main toolbar.
    
*   Editor: Updated to ProBuilder 4.4.0.
    
*   Editor: Updated UI so that Scene view deselect-click (Ctrl/Cmd) works more intuitively with prefabs that contain child GameObjects.
    
*   Editor: Updated Unity so it no longer treats layers 3, 6 and 7 as reserved. (1264751)
    
*   GI: Added API to get or set the Lighting Setting Asset for loaded scenes.
    
*   GI: Added support for half float texture format for Light Probe Proxy Volume (LPPV) component. You can now choose the format of the 3D LPPV texture from the LPPV inspector.
    
*   GI: Ensured that correct, official AMD graphics card names are displayed in the Lighting window GPU device dropdown.
    
*   GI: Improved Lighting Settings such as preset support, updated related docs and exposed default settings.
    
*   GI: Improved scheduling of lightmaps, light probes and additional probe bakes with the GPU lightmapper.
    
*   GI: Improved speed of GI main thread initialization on Editor startup. ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   GI: Improved the com.unity.rendering.hybrid package by forcing all lightmaps to max atlas size so that they can be stored in texture arrays.
    
*   GI: Reduced GPU memory usage when you bake large lightmaps with the GPU lightmapper. Achieved by baking in smaller tiles in non progressive mode.
    
*   GI: Removed custom Lighting Settings from 3D template.
    
*   GI: Updated Light Probe Proxy Volumes components so that they only update once per frame, rather than once per camera render, because these components are not camera relative.
    
*   GI: Upgraded Radeon denoiser to use RIF 1.5.1.2. This will only attempt to run on GPUs with at least 4GB of memory, becuase this is required by the AI model.
    
*   Graphics: A warning message appears when a users sets a UV out of range in the RecalculateUVDistributionMetric C# function.
    
*   Graphics: Added **Shader Precision Model** to the Player Settings, which allows you to change between current platform defaults and the new Unified Model. The Unified Model defaults to full sampler precision on all platforms, but allows explicit declarations of lower precision and using FP16 ops on targets where this is available. (1280157)
    
*   Graphics: Added debug names for resources on DX12.
    
*   Graphics: Added generated warnings when you use an unsupported CommandBuffer API inside a Render Pass.
    
*   Graphics: Added support for ASTC decode mode RGB9E5 for ASTC HDR textures. This only works when there is no alpha channel in use.
    
*   Graphics: Added support for DXT5nm normal maps on Android, iOS, tvOS. (1235914)
    
*   Graphics: Added the option to delay acquiring the swapchain buffer until it is actually used when rendering in Vulkan.
    
*   Graphics: Copy spawn count because we can process several time Init/Update per frame. ([1268360](https://issuetracker.unity3d.com/issues/vfx-thread-group-size-must-be-above-zero-error-is-thrown-continuously-when-exact-fixed-time-update-mode-is-enabled))
    
*   Graphics: Disabled rendering to color channels during a Scriptable Render Pipeline shadow pass, to improve performance.
    
*   Graphics: Enabled threaded texture creation on Xbox DX11 to remove frame spikes. Added support for direct upload of offline processed data on DX12 when threaded texture creation is disabled.
    
*   Graphics: Enhanced colorspace switching to only recreate textures with colorspace sensitive formats (for example DXT1\_sRGB/UNorm).
    
*   Graphics: Ensured that ComputeBuffer counters are put into separate physical buffers to impove data access/alignment for the Metal API.
    
*   Graphics: Extended supported types/formats for RWTexture2D when using Vulkan and OpenGL ES.
    
*   Graphics: Improved ComputeBuffer data alignment for Metal.
    
*   Graphics: Improved DX12 async texture loading so that when out of GPU memory, it returns a failure state, reports an error and cleans up memory.
    
*   Graphics: Improved DX12 performance when Unity creates a lot of resources per frame.
    
*   Graphics: Improved DX12 performance with the hybrid renderer.
    
*   Graphics: Improved error reporting in the Ray Tracing shaders interface.
    
*   Graphics: Improved input validation of RenderPass API.
    
*   Graphics: Improved performance by initializing the intermediate tree renderer with AABB::zero instead of NaN.
    
*   Graphics: Improved shader property error messages.
    
*   Graphics: Improved texture creation performance for cube maps on Metal.
    
*   Graphics: Improved texture creation performance for cube maps on Vulkan.
    
*   Graphics: Improved texture creation performance for CubeMaps on PC and Xbox on DX11 and DX12, and PS4.
    
*   Graphics: Improved the error messaging interface which appears when texture stacks are set up incorrectly.
    
*   Graphics: Improved validation of `RenderTexture` with bindTextureMS for unsupported formats.
    
*   Graphics: Increased draw calls per command list to improve URP Shadow Pass performance when rendering cascaded shadow maps.
    
*   Graphics: Metal: Add changes required for Apple GPU support on a Mac.
    
*   Graphics: Optimized D3D12 Constant Buffers for per-Pass binding.
    
*   Graphics: Reduced shader compilation times and application build sizes for GLSL/Metal platforms.
    
*   Graphics: Updated the D3D12 internal command buffer to allow access from a D3D12 native plugin.
    
*   GraphView: Added capability support to stacks, child stacks, and groups to better avoid unsupported behaviors, specifically with grouping and heterogeneous selections.
    
*   IL2CPP: Added attribute to avoid runtime performance impact of static constructors.
    
*   IL2CPP: Fixed a GC performance regression on Android and Linux.
    
*   IL2CPP: Improved error message when required Visual Studio components are not installed when building for Windows.
    
*   IL2CPP: Parallel IL2CPP Conversion is now default to improve IL2CPP build performance.
    
*   IL2CPP: Reduced the number of error messages produced by an IL2CPP failure from two to one.
    
*   iOS: Added support for custom storyboards on iOS.
    
*   iOS: Changed built-in .xib launch screens to storyboard.
    
*   iOS: Improved how version defines in Trampoline are generated so all versions are supported and they can be compared numerically. ([1244796](https://issuetracker.unity3d.com/issues/ios-unity-version-in-unitytrampolineconfigure-dot-h-is-higher-in-earlier-unity-versions-compared-to-newer-versions))
    
*   iOS: Modified `Camera.targetDisplay` to work with iOS Metal. ([1171951](https://issuetracker.unity3d.com/issues/mobile-multi-display-doesnt-work-on-secondary-displays-using-lwrp))
    
*   iOS: Under some circumstances, interim AA resolve no longer results in an extra texture copy.
    
*   Kernel: Fixed issue where Unity would crash when passing an empty filename to `AsyncReadManager.Read`.
    
*   Kernel: Optimized the low-level atomic queue container used by the `JobQueue`.
    
*   Kernel: Reduced job system overhead on macOS.
    
*   Kernel: Reduced main thread overhead of creating job reflection data.
    
*   Kernel: Reduced the time it takes to enter Play mode with many IJobChunk-style Burst compiled jobs.
    
*   Kernel: Refactored memory label code, for a lower generated code size.
    
*   Kernel: Removed the unneccesary parallel for access restrictions for `IJobFor.Schedule`
    
*   macOS: Removed project name in the window title bar.
    
*   Mobile: Added VRR support.
    
*   Mobile: Improved Provider Stats reporting.
    
*   Mobile: Updated com.unity.mobile.notifications to 1.3.2.
    
*   Mobile: Updated verified package Adaptive Performance and Samsung provider to 1.1.6.
    
*   Mobile: Updated [Adaptive Performance Samsung Android](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@2.1/manual/index.html) package to version 1.1.1.
    
*   Package: Updated input system package to 1.0.1. ([1292513](https://issuetracker.unity3d.com/issues/input-system-after-package-install-the-update-slash-switch-and-restart-prompt-does-not-appear))
    
*   Package Manager: Added a clearer error message that appears when the UnityPackageManager program is missing.
    
*   Package Manager: Added a loading screen to the Package Manager to give visual feedback when you install a package from a Git URL.
    
*   Package Manager: Added support for returning enterprise entitlement packages from the `PackageManager.Client.SearchAll()` method. These packages now show in the Package Manager UI **Unity Registry** section when users have the entitlement to use them.
    
*   Package Manager: Added the Package Manager lock file (`Packages/packages-lock.json`) to the _Bug Reporter_ report.
    
*   Package Manager: Added tooltips to action buttons for packages.
    
*   Package Manager: Improved package interoperability with Unity IAP. Added functionality for Unity IAP package to work directly with UDP Package instead of maintaining it's own UDP.dll.  
    Enabled user permissions to be set at Project level.  
    Updated UDP settings so that inspector window opens when you invoke the asset file. This allows for faster load and sync times.  
    Refined general code.
    
*   Package Manager: Improved performance of Package Manager metadata requests sent to the registry.
    
*   Package Manager: Improved visibility of **Import** and **Download** buttons.
    
*   Package Manager: Updated dependency resolution so that it automatically resolves trivial conflicts.
    
*   Package Manager: Updated Unity Package Manager so that it caches state on disk, to improve project loading time.
    
*   Package Manager: Upgraded Cinemachine to 2.6.1.
    
*   Particles: Added a button to the Particle System UI to identify ownership of the system for sub-emitters.
    
*   Particles: Added a new Depth sorting mode, to sort particles based on their distance from the camera plane. ([1207573](https://issuetracker.unity3d.com/issues/shuriken-particle-sort-mode-by-distance-does-not-take-depth-into-account-when-particles-are-aligned-by-view))
    
*   Particles: Improved performance by removing unnecessary calls to `ParticleSystemRenderer::UpdateCachedMesh`. This especially improves performance of enabling or disabling ParticleSystemRenderers that use meshes consisting of Triangle Strip geometry. ([1271169](https://issuetracker.unity3d.com/issues/particles-updatecachedmesh-needlessly-called-when-disabling-thne-enabling-a-particlesystemrenderer))
    
*   Particles: Improved the Collision and Trigger Modules so they can have any number of colliders.
    
*   Physics: Added tooltips for some of the physics settings in the Editor. ([1268052](https://issuetracker.unity3d.com/issues/imgui-auto-sync-transforms-property-tooltip-missing-under-physics-in-the-project-setting-window))
    
*   Physics: Added tooltips to the properties exposed in the ArticulationBody inspector. ([1256304](https://issuetracker.unity3d.com/issues/imgui-articulation-body-components-tooltips-are-missing))
    
*   Physics: Implemented visualisers for articulation body joint limits (both linear and angular). This update applies to revolute, prismatic and spherical joints.  
    
    ![](/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif)
    
*   Prefabs: Added **Create Prefab** item to the asset menu, so you can create and start editing a new Prefab Asset without interfering with the current scene.
    
*   Prefabs: Improved the performance of nested Prefab modification saving.
    
*   Prefabs: Improved the performance of Prefabs in the Editor.  
    
*   Prefabs: Improved the performance of the prefab editor.
    
*   Prefabs: Introduced the **Allow Auto Save** Project Setting for Prefab Mode. It is enabled by default, which matches the same behavior in previous versions of Unity. However, if you disable this setting, Unity does not auto save while in Prefab Mode, and the toggle is not displayed. This is different to the main Auto Save toggle, which is a per-user setting that carries across projects. This new setting applies to all users of the project. (1141476)
    
*   Prefabs: Prefabs with a lot of properties load faster than before.
    
*   Profiler: Added a progress bar when loading and saving Profiler data.
    
*   Profiler: Added a visualization for Async Loading flow in the CPU Profiler Timeline view.
    
*   Profiler: Added ability to specify a Profiler category for ProfilerMarker.
    
*   Profiler: Added an option to specify a port in the direct Profiler connection UI.
    
*   Profiler: Added the ability to see the metadata associated with a Profiler sample in the Hierarchy View of the CPU Profiler module.
    
*   Profiler: Aligned the Memory and Rendering Profiler module detailed panel test with runtime counter names.
    
*   Profiler: Burst jobs have a different color from normal jobs in CPU Profiler Timeline view.
    
*   Profiler: Changed the load icon in the Profiler window so that it clearly represents loading better.
    
*   Profiler: Fixed an issue where the Profiler window did not process small frames immediately when they come to Profiler Window. (1260269)
    
*   Profiler: Improved the handling of message sending and receipt in `PlayerConnection`, and split the receipt of messages across multiple frames.
    
*   Profiler: Optimized Profiler Window chart updates.
    
*   Profiler: Updated the Hierarchy and Timeline view to no longer display frame data while profiling unless the "Live" toggle is enabled. This reduces the Editor overhead while profiling the Editor or Play mode.
    
*   Scripting: Added a way to get the stack trace without garbage collection in the Editor.
    
*   Scripting: Added inline documentation, constructors and implicit conversion operators to `LazyLoadReference`.
    
*   Scripting: Added support for new managed code stripping annotation attributes.
    
*   Scripting: Implemented switching code coverage without needing to restart the Editor. Introduced API to enable/disable code coverage.
    
*   Scripting: Improved performance of the Memory Profiler.
    
*   Scripting: Improved performance of `DefineConstraintsHelper`.
    
*   Scripting: Improved the query time of Camera.main.
    
*   Scripting: Improved UnsafeUtility.Malloc so that it throws an exception when it is given a positive alignment value that is not also a power of two. Previously this was only flagged as an assert in debug builds.
    
*   Scripting: Improved `UnityWebRequest.certificateHandler` so it is now invoked for root certificates on Windows.
    
*   Scripting: Updated AtomicSafetyHandle to throw ObjectDisposedExceptions instead of InvalidOperationException when code attempts to access a container after it has been disposed. This mimics the behavior of built-in container types.
    
*   Scripting: Updated Unity to invoke crash handler when Mono runtime encounters an abort or assert.
    
*   Scripting: When an instruction pointer is null, it obtains a full call stack to prevent a crash from happening.
    
*   Scripting: When Unity fails to load a .dll file, a detailed error message is displayed.
    
*   Scripting Upgrade: Added update to avoid logging potentially misleading messages when no assemblies successfully update.
    
*   Serialization: Increased the allowed serialization depth to allow Unity serialize larger, more complex data models.
    
*   Shaders: Added indentation to the compute shader preprocessed source.
    
*   Shaders: Added support for Caching Shader preprocessor to recognise ellipsises (but there is no variadic macros support).
    
*   Shaders: Added the ability to toggle #line directives on and off via a toggle in Shader and Compute Shader inspectors.
    
*   Shaders: Enabled shader live link to cache compilation results on disk.
    
*   Shaders: Improved #line directive output for preprocessed source.
    
*   Shaders: Improved preprocessed source so it is saved in a text file with a different name from compiled source.
    
*   Shaders: Improved the readability of the error produced when SV\_VertexID semantic is used with OpenGL ES 2.
    
*   Shaders: Reduced in-Editor memory usage for Compute shaders.
    
*   Shaders: Updated shader live link to only build one shader variant at player build time.
    
*   Terrain: Added "Delete Brush..." button to the brush selection UI.
    
*   Terrain: Added a **Hole Edge Padding** option to terrain Detail Prototype to control how far details objects will be from the hole edge.
    
*   Terrain: Added a warning message that appears after you select a detail prototype, if Terrain cannot hold all the detail GameObjects when you paint at maximum density. ([1248486](https://issuetracker.unity3d.com/issues/target-strength-appears-to-be-way-too-strong))
    
*   Terrain: Added warnings which occur if you paint too many detail objects on terrain. Unity will now draw red boxes highlighting these areas in the scene view and display an error message explaining the issue. ([1248488](https://issuetracker.unity3d.com/issues/hitting-the-upper-bound-of-detail-meshes-causes-previously-placed-detail-meshes-to-dissappear))
    
*   Terrain: Made Terrain per-frame CPU updates less resource-intensive.
    
*   UI: Added secondary list of graphics that are raycast targets to `CanvasUpdateRegistry`. This prevents iterating over the whole list every frame.
    
*   UI: Added the ability to have wrap around navigation for horizontal and vertical navigation.
    
*   UI: Added the ability to toggle the "Maskable" option from the Inspector as well as from a script.
    
*   UI: Improved UIStruct memory to use bitfields to save.
    
*   UI: Updated documentation for `OnRectTransformDimensionsChange` to clarify when it can be called.
    
*   UI: Updated UI to save the value of `.Count` when iterating through loops, instead of accessing it every time.
    
*   UI: Updated `ColorBlock` to default to a static colorblock.
    
*   UI: Updated `GraphicRaycaster` `eventCamera` implementation to cache some calls for performance.
    
*   UI Toolkit: Added import of FontAsset via USS to UI Toolkit. (1266414)
    
*   Universal Windows Platform: Added warnings to Player Settings if any of the required icon images are not set, to alert the user that missing images will result in the application failing Windows certification.
    
*   Version Control: Improved Smart Merge (UnityYamlMerge) so it now sets premerge base to file in correct base values instead of leaving them blank. Blank premerge base values can still be configured - see mergerules.txt for an example.
    
*   Version Control: Updated existing version control icons. Added theme support.
    
*   Windows: Improved `Time.deltaTime` consistency for D3D11 graphics API.
    
*   Windows: Improved `Time.deltaTime` consistency for D3D12 graphics API.
    
*   XR: Improved XR Statistics so it caches thread-safe stats that only get promoted to 'live' data after a render pass. A number of data points need to be 'initialized' before you can render a frame.
    
*   XR: Reduced unnecessary Vulkan backbuffer allocations.
    
*   XR: Updated verified packages for AR Foundation and related packages.
    
*   XR: Updated Windows Mixed Reality XR Plugin verified version to 4.1.1.
    
*   XR: Updated XR Plug-in Management to 3.2.16, Update Windows MR XR Plug-in to 4.2.1.
    

### Changes

*   2D: Added a contextual helper in the Scene view to open the Tile Palette window that appears when you select a GameObject which can be edited with the Tile Palette window.
    
*   2D: Added support for user to edit Tile Palettes with Brushes. For this to work, the Tile Palette must be empty and unlocked, and the Editor must be in Edit mode.
    
*   2D: Added the correct URL to the Tile help icon.
    
*   2D: Removed the _Reset Bounds_ button from the Sprite Skin Editor.
    
*   2D: Removed Tile _Create Asset_ menu item.
    
*   2D: Updated Scriptable Brushes to use `layoutGrid` for `GridBrushEditorBase` preview calls.
    
*   Android: Moved `UnityEngine.Android.AndroidDevice` from `UnityEngine.dll` to `UnityEngine.AndroidJNIModule.dll`.
    
*   Android: Moved `UnityEngine.Android.Permission` from `UnityEngine.dll` to `UnityEngine.AndroidJNIModule.dll`.
    
*   Android: Updated gradle template to use `enableR8` setting in `gradle.properties` instead of `useProguard`.
    
*   Android: Upgraded Android Gradle Plugin to 3.6.0 and Gradle to 5.6.4.
    
*   Asset Import: Changed the default material import mode of the model importer from 'Standard' to 'Import via MaterialDescription'.
    
*   Asset Pipeline: Only accept protocol >=TLSv1.2. SECURITY-1828.
    
*   Audio: Updated DSPGraph so that the interleaving of samples in the output buffer happen inside Unity, rather than third-party output hook implementations
    
*   Build Pipeline: Updated build pipleline to always add a copy of the managed symbols to a `Temp/ManagedSymbols` folder during a build.
    
*   Burst: Asserts that are currently discarded no longer discard arguments with potential side effects.
    
*   Burst: Changed the version of com.unity.mathematics to 1.2.1.
    
*   Burst: Temporarily removed the Burst compiler warning about exception throws not in \[Conditional("ENABLE\_UNITY\_COLLECTIONS\_CHECKS")\] methods, to let us address user feedback. The next minor version of Burst will reincorporate this in a more friendly manner.
    
*   Burst: Unity temporarily disables `Debug.Log` output to avoid a deadlock on a domain reload, when used in Burst function pointers and jobs. A fix for the Unity Editor is being developed.
    
*   Compute: Changed the result to NaN from 0 when a 0 is divided by 0. ([1257445](https://issuetracker.unity3d.com/issues/the-value-of-a-float-or-double-field-becomes-0-when-inputting-0-slash-0-in-the-inspector))
    
*   Editor: As part of gizmo optimizations, we've made many gizmos (e.g. collider gizmos) fade out and turn off when they are small on screen. Cameras typically used for planar reflections (ones with oblique clip projection matrix) now also do not render gizmos.
    
*   Editor: Changed the Position handle to follow mouse movements more precisely. ([1217150](https://issuetracker.unity3d.com/issues/sceneview-move-tool-axis-move-does-not-follow-the-mouse-position))
    
*   Editor: Disabled the _Maximize_ option for _Preview_ window when docked. ([1258262](https://issuetracker.unity3d.com/issues/inspector-framework-nullreferenceexception-is-thrown-when-the-preview-window-is-maximized))
    
*   Editor: Marked Unity Remote as deprecated.
    
*   Editor: Modified the _Rect Tool_ when calculating an object's bounds so that _GameObjects_ with a `MeshFilter` but no `MeshRenderer` are included.
    
*   Editor: Removed "macOS Color Picker" editor preference setting.
    
*   Editor: Removed 3D With Extras template.
    
*   Editor: Removed Asset Store integration from the Project Browser. ([1240939](https://issuetracker.unity3d.com/issues/unityeditor-dot-asynchttpclient-done-error-when-switch-between-in-packages-and-in-assets-for-the-serach-results))
    
*   Editor: Removed the ability to discard changes to an untitled Scene. ([1111388](https://issuetracker.unity3d.com/issues/scene-management-invalidoperationexception-is-thrown-when-discarding-changes-in-deleted-scene))
    
*   Editor: Revert reintroduction of OnDestroy/Awake calls for ExecuteAlways scripts when we enter Play Mode with the Scene Reload disabled.
    
*   Editor: Updated GameObject creation from a context menu or Scene so new GameObjects are instantiated at the world origin. (1179419)
    
*   Editor: Updated Hierarchy view to automatically enter rename mode when new objects are created. "Rename New Objects" in Hierarchy view settings menu turns this behavior off.
    
*   Editor: Updated interaction mode labels and tooltips.
    
*   Editor: Updated the com.unity.ide.rider package to version 2.0.7 as a verified package.
    
*   Editor: Verified the configurable Enter Play Mode feature.
    
*   GI: Modified the LightingSettings asset so it is now only created when saving an upgraded project.
    
*   GI: Unlocked the maximum number of bounces supported by the lightmapper.  
    Added min bounces and max bounces UI labels for better readability.  
    
*   GI: Updated 3D template so that new projects created with it support baked light cookies by default.
    
*   GI: Updated Open Image Denoise to the Clang compiled binary instead of IC., This fixed a Rosetta emulation issue on a Mac.
    
*   Graphics: Enabled "Gfx command not handled: 0 (Last command: 10123)" in the Editor's console while in Scene view when using the wireframe mode and Vulkan rendering API. ([1276056](https://issuetracker.unity3d.com/issues/graphics-gfx-command-not-handled-error-thrown-continuously-on-switching-editor-to-wireframe-mode-using-vulkan-graphics-api))
    
*   Graphics: Exposed mesh function to set UV Distribution metric for procedurally generated meshes with mip streaming. ([1248390](https://issuetracker.unity3d.com/issues/graphics-scripting-meshes-created-in-c-number-cannot-have-their-uv-distribution-metric-updated))
    
*   Graphics: Updated the SRP packages and template to version 10.2.2 ([1291998](https://issuetracker.unity3d.com/issues/hdrp-opening-template-scene-freezes-or-reboots-mac))
    
*   iOS: Removed OpenGL ES support on iOS/tvOS.
    
*   iOS: Removed support for Launch Images, to adhere to new Apple guidelines.
    
*   Kernel: Updated native allocators to use slightly larger blocks, to avoid the more resource-intensive overflow allocations that go directly to system memory. This causes a very slight increase in initial memory usage, but avoids some spikes in performance.
    
*   License: Updated the output message after a return license request timeouted. (1146162)
    
*   macOS: MacOS 10.13 is now the minimum OS requirement for the MacEditor and MacPlayer. (1263013)
    
*   Mobile: Changed maximum temperative level to level 10 in Adaptive Performance Samsung Provider GameSDK 3.2.
    
*   Mobile: Fixed Analytics system error with unloaded subsystem in Adaptive Performance.
    
*   Mobile: Provider downloader will now download latest available build instead of verified if verified version is below 2.0.0. This can happen on 2019 and 2020.1 as the verified package version is 1.x.
    
*   Mobile: Removed unnecessary folders and files from the Adaptive Performance package.
    
*   Mobile: Updated Adaptive Performance Samsung Provider GameSDK 3.2. You can use the Adaptive performance CPU and GPU levels until the system reaches warning level 2 (throttling).
    
*   Package Manager: Added a General Preference option to allow the log level used by the Unity Package Manager for the Editor.log and upm.log files to be customized. This preference is saved and re-used across sessions, and it is overridden by the effects of the `-enablePackageManagerTraces` command-line argument.
    
*   Package Manager: Added the `UnityEditor.PackageManager.Client.LogLevel` property that allows you to configure the log level that the Unity Package Manager uses for the upm.log file.
    
*   Package Manager: Changed path and file format of global configuration file. The configuration file format is now TOML. The old global configuration file path is deprecated. New global configuration should be set in this new file.
    
*   Package Manager: Changed the design of the items in the Package List to be one line.
    
*   Package Manager: Modified Package Manager to no longer discard the existing package state in case of critical errors such as failure to parse the project manifest.
    
*   Package Manager: Split `All Packages` into `Unity Registry` and `My Registries`.
    
*   Package Manager: Updated functionality to automatically add embedded package files to the version control system.
    
*   Package Manager: Updated how version conflicts involving a direct project dependency are reported. They are now reported like any other version conflict instead of being silenced.
    
*   Package Manager: Updated the com.unity.purchasing package to version 2.1.0.
    
*   Package Manager: Updated the recommended version logic in the Package Item version drop down.
    
*   Package Manager: Upgraded Cinemachine to 2.6.0. See Cinemachine 2.6 release notes.
    
*   Player: Added a dependency on 'com.unity.modules.subsystems' to the Subsystem Registration package.
    
*   Player: Added ToString override to PlayerLoopSystem to show system type.
    
*   Scripting: Reintroduced a warning when a script that is derived from MonoBehaviour has the same name as a built-in component (for example,Transform).
    
*   Scripting: Removed Boo.dll and UnityScript.dll from Mono distribution.
    
*   Scripting: Roslyn Analyzers inside Assembly Definitions Folders are now only applied to the Asmdef Assembly itself and to other Assemblies referencing the Asmdef Assembly - but not to any other code in the project.
    
*   Scripting: Strong Name Assembly references only validate if the assemblies are in different folders.
    
*   Services: Added support to in the In-App Purchasing Service settings for safely migrating the [IAP](https://docs.unity3d.com/2019.4/Documentation/Manual/UnityIAP.html) package from older versions to 3.0+. Retained the ability to update to the most recent legacy versions of In-App Purchasing without migrating. Projects without any versions of this package already installed can install 3.0+ from the In-App Purchasing Settings user interface.
    
*   Services: Updated com.unity.purchasing to 2.1.1.
    
*   Shaders: Changed Editor so that it skips warming up shaders from shader collections in the Preloaded shaders section of Graphics settings.
    
*   Shaders: Made Caching Shader preprocessor the default preprocessor for shaders.
    
*   Shaders: Relaxed macro expansion rules in Caching Preprocessor for token pasting to always use expanded arguments instead of non-expanded arguments.
    
*   Timeline: Modified `ControlPlayableAsset.searchHierarchy` to default to false. You now have to specifically set it to true to search the entire hierarchy.
    
*   Timeline: Updated the default [Timeline](https://docs.unity3d.com/Packages/com.unity.timeline@1.5/manual/index.html) package version to 1.4.4.
    
*   UI: Expanded the usable UV to Vector4 instead of the previous limit of Vector2. ([1208182](https://issuetracker.unity3d.com/issues/only-2-uv-components-per-channel-are-accessible-in-shader-when-mesh-is-rendered-by-canvasrenderer))
    
*   UI: Set `Switch m_CullTransparentMesh` to true so transparent Meshs are culled by default. (1257834)
    
*   UI: Updated the `EventSystem.current` API so that it doesn't do unnecessary work when setting `current` to the already current system.
    
*   UI Toolkit: Renamed menu entries of UIElements to UI Toolkit.  
    
    *   _Window/Analysis/UIElements Debugger_ becomes _Window/UI Toolkit/Debugger_  
        
    *   _Window/UI/UIElements Samples_ becomes _Window/UI Toolkit/Samples_  
        
    *   _Create/UIElements/Editor Window_ becomes _Create/UI Toolkit/Editor Window_  
        
    *   _Create/UIElements/USS File_ becomes _Create/UI Toolkit/Style Sheet_  
        
    *   _Create/UIElements/UXML Template_ becomes _Create/UI Toolkit/UI Document_  
        Removed mentions of UIElements in the output of the Editor Window script generator.
*   XR: Added interface changes for providers to share unresolved MSAA targets between eye texture swap chains. This provides some memory savings. (1254408)
    
*   XR: Changed how temporarily disabling runtime MSAA level is affected if running with Vulkan and XR Management.
    
*   XR: Keep SRP occlusion mesh data accessible from the CPU.
    
*   XR: Removed the ARCore client libraries from Unity. These libraries are now added to a project by installing the ARCore SDK for Unity (distributed by Google).
    
*   XR: Updated the Oculus XR Plugin package to 1.6.1.
    
*   XR: Updated verified packages for AR Foundation and related packages.
    
*   XR: Updated verified version of com.unity.xr.legacyinputhelpers to v2.1.6  
    Changelog for 2.1.6 of com.unity.xr.legacyinputhelpers:  
    
    *   Fixes error message when using the color camera  
        
    *   Changes default near clip plane to 0.01f  
        
    *   Fixes rig migration for URP and HDRP.  
        
    *   Support for URP/HDRP v10.1.

### API Changes