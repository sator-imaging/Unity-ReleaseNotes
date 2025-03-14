# Unity 6000.0.23f1 LTS
Published at Wed, 16 Oct 2024 23:50:12 GMT  
https://unity.com/releases/editor/whats-new/6000.0.23


# Known Issues in 6000.0.23f1

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- HDRP: Graphics Compositor breaks Unity rendering when the "Output Camera" is changed to a scene Camera and one Camera SubLayer is active.<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84610

- IAP: [Android] Build fails with Error "A failure occurred while executing com.android.build.gradle.internal.tasks.CheckDuplicatesRunnable" when using In-App Purchasing and Facebook SDK
    ([UUM-76723](https://issuetracker.unity3d.com/issues/android-build-fails-when-using-in-app-purchasing-and-facebook-sdk))

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Scene Tooling: GPU utilization increases when a GameObject is selected
    ([UUM-84132](https://issuetracker.unity3d.com/issues/gpu-utilization-increases-when-a-gameobject-is-selected))

- Shader System: Shader cache is not used when building the Player repeatedly
    ([UUM-75264](https://issuetracker.unity3d.com/issues/shader-cache-is-not-used-when-building-the-player-repeatedly))

- Shader System: Shaders are always recompiled when the Editor is opened
    ([UUM-75262](https://issuetracker.unity3d.com/issues/shaders-are-always-recompiled-when-the-editor-is-opened))

- Vulkan: [Android] Particles not rendered in the Player on some Android devices with Android 14
    ([UUM-68080](https://issuetracker.unity3d.com/issues/android-particles-not-rendered-in-the-player-on-some-android-devices-with-android-14))


# Full Unity 6 Release Notes
Find out what's new in Unity 6 Preview and Unity 6, and view the documentation for the affected areas on [this page](https://docs.unity3d.com/6000.0/Documentation/Manual/WhatsNewUnity6.html). 
(_6000.0.23f1 release notes are below this section_)

## Features

- Android: Added the Addressables for Android \(com.unity.addressables.android\) package. This package provides Play Asset Delivery support for Addressables.

- DX12: Added support for indirect Dispatch Rays \(part of DXR 1.1\). The method is similar to `RayTracingShader.Dispatch`, but the three dispatch dimensions are retrieved from a GraphicsBuffer. Added `RayTracingShader.DispatchIndirect` and a new `CommandBuffer.DispatchRays` signature. Added `SystemInfo.supportsIndirectDispatchRays` capability status.

- Editor: Added a custom menu on `IRenderPipelineGraphicsSettings`.

- Editor: Added a piercing menu that you can open with Ctrl + Right-click in the Scene view. The piercing menu provides a UI that lists all GameObjects under the pointer. GameObjects in the menu can be highlighted and selected.

- Editor: Added the `ForceNoCrunch` option to the *Build Windows &gt; Asset Import Overrides &gt; Texture Compression* dropdown which forces all textures to disable crunch compression and re-import.

- Editor: Added `Additional App IDs` to Steam ID Provider Editor Settings for Multiple App ID support.

- Editor: Integrated new build profile icons.

- Editor: Introduced `IRenderPipelineResources` to host SRP resources, which uses the `ResourcePath` to auto-load resources.

- Editor: The Build Profile Diagnostic checkbox is no longer available because the Build Settings window has been replaced with the Build Profile window.

- Graphics: Added a new backend rendering path for rigid GameObjects in Unity that puts them through the Batch Render Group API when the option is enabled on the Render Pipeline asset \('GPU Resident Drawer'\). This functionality creates a persistent GPU state for these objects and they will be rendered by the same fast batching path as used by the entities renderer.

- Graphics: Added small-mesh culling for gpu-driven instances.

- Graphics: Added support for GPU occlusion culling of instances that are compatible with the 'GPU Resident Drawer', which can be enabled in the Render Pipeline asset.

- Graphics: Added UITK support for CustomPostProcessOrder.

- Graphics: Adding a new per batch layer filtering setting for BatchRendererGroup. This setting is useful for the context of culling out specific batches that go through the batch renderer group.

- Graphics: Enabled SpeedTree GameObjects rendering using GPU Resident Drawer.

- Graphics: Updated the default `IRenderPipelineGraphicsSettings` Inspector to trigger notifications when a value is modified.

- HDRP: Added AMD FidelityFX Super Resolution 2 \(FSR2\) Unity script bindings and HDRP integration.

- HDRP: Added support for overriding material properties such as smoothness, albedo, and normal maps on all materials to facilitate material and lighting debugging. The material override feature in HDRP is available through the Rendering Debugger's Lighting panel when rendering through the path tracer pipeline.

- HDRP: Added support for Spatial Temporal Post-Processing \(STP\) upscaling solution.

- HDRP: Added the Sky Occlusion feature to Adaptive Probe Volumes \(APV\), to allow time of day with static probe volumes.

- HDRP: Disabled storing of baked data as Streaming Asset in Adaptive Probe Volumes \(APV\) to make it compatible with Asset Bundles and Addressables.

- HDRP: Improved on existing Mipmap Streaming debug views and added more. The current offering in HDRP is consistent with what URP offers.

- iOS: Added Apple Privacy Manifest support.

- Package: Added the Character Controller package, version 1.2.4.

- Package: Improved the user experience in the 2.0.8 patch of the User Reporting package.

- Package Manager: Improved Project manifest files to repopulate with default dependencies when the files are empty or contain only whitespace.

- Particles: Add `BakeTexture` and `BakeTrailsTexture` scripting methods.

- Particles: Added the Custom Vertex Streams feature for particle trails.

- Shadergraph: Added a customizable Heatmap color mode, which by default displays the estimated performance impact of each node in a Shader Graph.

- Shadergraph: Added a new sample content pack that can be installed with the Package Manager. The samples contain descriptions, examples, and break downs for a majority of the nodes in Shader Graph. These samples help users understand the inner workings of the nodes and see examples of how they work and how they can be used.

- Shadergraph: Added a zoom step size option in the user preferences.

- Shadergraph: Added new shortcuts for adding new nodes and toggling sub-window visibility, and moved several existing shortcuts to the Shortcut Manager.

- Shadergraph: Added the Feature Examples Sample to Shader Graph to show users how to achieve specific effects in Shader Graph.

- SpeedTree: Added the SpeedTree9Importer, which supports .st9 files exported by SpeedTree Modeler 9 and includes the following:<br>
    * Support for SpeedTree Games Wind and SpeedTree Legacy Wind effects<br>
    * The ability to configure wind strength and direction responsiveness through the Importer Settings<br>
    * New SpeedTree9 shaders for built-in \(.cg\), URP, and HDRP renderers \(.shadergraph\)<br>
    * New shaders for the new wind effects, but no major changes to lighting

- SRP Core: Added the option to cache Render Graph compilation for both URP and HDRP.

- TextCore: Native TextGenerator Rewrite.

- UI Toolkit: Added a debugger for the UI Toolkit dynamic atlas.

- UI Toolkit: Added missing UxmlAttribute converters to support UXML authoring: `Gradient`, `AnimationCurve`, `ToggleButtonGroupState`, Unsigned Int and Unsigned Long.

- UI Toolkit: Added support in `PropertyField` for `ToggleButtonGroupState` serialized properties.

- Universal RP: Added a Camera History Texture manager and basic interfaces to access per-camera history textures.<br>
    History textures are wrapped and stored in types which contain all the textures, additional data, and API methods specific for that history.<br>
    History textures are useful for rendering algorithms that accumulate samples over multiple frames or use data of previous frames as input.

- Universal RP: Added a new config package that allows you to override the maximum number of lights visible on screen.

- Universal RP: Added C\# script templates to create a post-processing `ScriptableRendererFeature` that uses a custom `VolumeComponent`.

- Universal RP: Added per-camera color and depth history and history access for custom render passes.

- Universal RP: Added support for foveated rendering in the Forward+ rendering path.

- Universal RP: Added the `8192x8192` option in Shadow textures.

- URP: Added Adaptive Probe Volumes \(APV\) Lighting Scenario Blending to URP

- URP: Added APV Sky Occlusion support for URP.

- URP: Added Render Graph Viewer. Access it through the *Window &gt; Rendering* menu. The tool helps to visualize and debug resource usage of Render Passes in the Render Graph framework.

- URP: Added six Mipmap Streaming debug views to the Rendering Debugger. These views can be found in the *Rendering* tab, under *Mipmap Streaming*. The available debug views are: Mip Streaming Performance, Mip Streaming Status, Mip Streaming Activity, Mip Streaming Priority, Mip Count, and Mip Ratio.

- URP: Added support for Spatial Temporal Post-Processing \(STP\) upscaling solution.

- VFX Graph: Added Camera Buffer Access support in VFX with URP.

- VFX Graph: Added collision events that allow specific processes upon contact.

- VFX Graph: Added new profiling/debugging panels in the VFX window.

- VFX Graph: Added particle count readback for strips, which also allows strips to go to sleep state.

- VFX Graph: Added support for per-particle sorting in strips.

- VFX Graph: Allowed instanced rendering of VFX that have exposed textures or graphic buffers.

- VFX Graph: Built-in and custom attributes can now be handled from the blackboard panel.

- VFX Graph: Enabled Frustum Culling for strips.

- VFX Graph: Improved the Shader Graph Cross Pipeline workflow.

- VFX Graph: Reworked Flipbook player block.

- VFX Graph: Strips now support the "Indirect draw" option. "Indirect draw" renders only the particles that are active, instead of full capacity.

- VFX Graph: Support of `ShaderKeyword` declared in Shader Graph.

- VFX Graph: The following improvements have been made to shortcuts in VFX Graph:<br>
    * Registered the shortcuts in the global Unity Shortcut window.<br>
    * Synced shortcuts with ShaderGraph where possible.<br>
    * Added new shortcuts.

- Web: Implemented the following `LocationService` methods and properties in Web platform:<br>
    * `Start()`<br>
    * `Stop()`<br>
    * `isEnabledByUser`<br>
    * `lastData`<br>
    * `status`

- Web: \[Web Platform\] Added the ability to copy and paste to and from the Unity player.

- WebGL: Added support for **WebAssembly 2023**, which is a Unity-coined term for a collection of newer WebAssembly language features such as, sign-ext opcodes, non-trapping fp-to-int, bulk-memory, bigint, wasm table, native Wasm exceptions, and Wasm SIMD.

- WebGL: Implemented the following LocationService methods and properties:<br>
    * `GetLastHeading()`<br>
    * `SetHeadingUpdatesEnabled()`<br>
    * `IsHeadingUpdatesEnabled()`<br>
    * `GetHeadingStatus()`<br>
    * `IsHeadingAvailable()`

- XR: Added support for Foveated Rendering on Vision Pro.



## Improvements

- 2D: Improved performance of shadow generation.

- Accessibility: Improved multiple API documentation for the Screen Reader API.

- AI: Increased the speed of the instantiation of NavMeshes into the scene.

- Android: Added a new Player setting to display warnings when the symbols package size exceeds the specified threshold.

- Android: Added a new property in `.androidlib` plug-in inspector to specify dependencies for `unityLibrary`. You can now configure `.androidlib` to depend on `unityLibrary`, and thus expand an activity by overriding `UnityPlayerActivity`.

- Android: Fixed `.androidlib` default `build.gradle`, it will correctly apply android library plugin + targetSDKVersion.

- Android: When producing the symbols.zip package, Unity will prompt Gradle to produce the zip, which means the symbols.zip package might contain more symbol files, allowing for better stack trace resolution. This also allows you to regenerate the symbols package from within the Gradle project.

- Android: You can now embed Debug symbols into an app bundle \(e.g., in the Build Settings window, choose Debug Symbol &gt; level and format to IncludeInBundle\) when uploading .aab files to the Google Play Store. The symbols are uploaded together with aab, which means you don't need to upload the symbols separately.

- Apple TV: Included platform name in Bundle Identifier error messages.
    ([UUM-52189](https://issuetracker.unity3d.com/issues/tvos-making-a-build-for-tvos-with-invalid-bundle-id-will-throw-an-error-saying-that-the-bundle-id-for-ios-is-invalid))

- Asset Pipeline: Improved error handling when updating ArtifactDB or SourceAssetsDB.
    ([UUM-48669](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-opening-a-project))

- Audio: Added an "Edit Audio Random Container" button to the *Audio Random Container Inspector*. Also, disabled presets for the Audio Random Container.
    (UUM-51019)

- Audio: Enabled ALT+P as a shortcut to preview the Audio Random Container \(ARC\).

- Audio: You can now create an Audio Random Container \(ARC\) from a selection of audio clips using the following method:<br>
    1. From your Project browser, select a set of audio clips.<br>
    2. Right-click and click **Create** &gt; **Audio** &gt; **Audio Random Container**.<br>
    This creates a fresh audio random container that contains the clips from your selection.

- Build System: Added deterministic shader ordering in output content.

- Build System: Content is now deterministically sorted when being pulled from the resource manager.

- Build System: Made bee_backend's directory deletion explicitly handle read-only files on Windows.

- Burst: Added a new `Math.Clamp` API, which is available when the *API Compatibility Level* is set to *.NET Standard 2.1*.

- Burst: Added Burst support for Apple visionOS.

- Burst: Added support for default interface methods.

- Burst: Added support for hashing against different target frameworks.

- Burst: Added support for string interpolation in exception messages.

- Burst: Added support for `System.Math` functions Acosh, Asinh, Atanh, Cbrt, CopySign, Log2, SinCos, FusedMultiplyAdd, and ILogB.

- Compute: Added logging when a ComputeShader variant is created with no keywords.

- Core: Clean up and clarify areas of the source code.

- Core: Improved baking of large scenes that use Probe Volumes.

- Documentation: Add instructions for blending Adaptive Probe Volumes at runtime.

- Documentation: Added a Multiplayer overview page to summarize Unity's multiplayer packages and services.

- Documentation: Added new and updated existing Accelerator cache server command line argument documentation.

- Documentation: Added two new workflows to the Timeline Workflows documentation<br>
    - The `Use markers and signals for footsteps` workflow demonstrates how to use Timeline markers, Signal assets, and Signal Receiver components to play audio sources for footsteps.<br>
    - The `Create a Sub-Timeline instance` workflow demonstrates how to create a single cut-scene by nesting a Timeline instance within another Timeline instance.

- Documentation: Improve the scripting documentation for RaycastHit2D.

- Documentation: Improved code sample for `NavMeshAgent.CalculatePath()` to better clarify how to interpret and use its results.
    (UUM-43219)

- Documentation: Updated documentation of Mathf.SmoothDamp.
    (UUM-60504)

- Documentation: \[AI\] Added some detail to NavMeshPathStatus.PathInvalid.
    (UUM-43218)

- DX12: Implemented a dedicated GPU memory allocator for small acceleration structures \(BLASes\) to save GPU memory when using ray tracing.

- DX12: Implemented acceleration structure \(BLAS\) compaction for static meshes to reduce GPU memory consumption in Ray Tracing effects. Compaction reduces memory requirements by more than 50% for BLASes.

- DX12: Optimized writing shader records into shader tables before ray tracing dispatches.

- Editor: Added a column that displays the shortcut type in the Shortcut Manager window.

- Editor: Added a general *Graph* category to the *search by type* option in ProjectBrowser.

- Editor: Added a new internal Editor API to control Rendering Layer names in Tag &amp; Layers.

- Editor: Added a toggle in the preferences to show the project path instead of the project name in main window title.

- Editor: Added Deselect and Invert Selection to the context menu.

- Editor: Added discrete menu items for pasting cut or copied GameObjects as children while preserving local or world transform.
    ([UUM-43090](https://issuetracker.unity3d.com/issues/gameobjects-world-position-is-not-preserved-when-cutting-and-pasting-it-as-a-child-to-another-gameobject))

- Editor: Allow for action and clutch shortcuts to use the same mouse button \[with or without modifiers\].

- Editor: Categorised and alphabetised the order of items in the Create menu.
    (UUM-49318)

- Editor: Changed the overlay menu into an overlay itself. This allows us to use the new Overlay Popup feature and to remove the need to maintain two code paths for very similar behaviors.

- Editor: Changed unused System namespaces so they are no longer added to new scripts.
    (UUM-60811)

- Editor: Data used for preview is released when the baked lightmap preview system is not used for 30 seconds.

- Editor: Implement guard for crash in TimeSliceAwakeFromLoadQueue::IntegrateTimeSliced.
    ([UUM-41509](https://issuetracker.unity3d.com/issues/crash-on-timesliceawakefromloadqueue-integratetimesliced-when-opening-a-scene))

- Editor: Improve performance when fetching artifacts that are missing \(e.g link to an artifact deleted from the project\).
    ([UUM-22002](https://issuetracker.unity3d.com/issues/the-animator-window-is-slow-when-displaying-a-blend-tree-with-many-nodes))

- Editor: Improved exception handling when package load fails.
    ([UUM-16258](https://issuetracker.unity3d.com/issues/crash-on-burstcompilerservice-compileasync-when-opening-project))

- Editor: Improved moving files in the Project window. Moving files in the Project window now takes less memory and is faster.
    ([UUM-44466](https://issuetracker.unity3d.com/issues/dragging-a-file-to-the-root-assets-directory-of-a-project-causes-large-allocations-and-a-long-hang-which-can-lead-to-a-oom-crash))

- Editor: Improved the Build window message that appears when a Dedicated Server target is not installed.
    (UUM-45218)

- Editor: Improved the Clamp Gizmo icon render size to prevent gizmos from being drawn obstructively large or unreadably small in certain scenes.

- Editor: Improved visibility on Volume component when Profile Instance used.

- Editor: Improvements to the Graphics Settings UI.

- Editor: Improvements to `CustomPropertyDrawer` to allow filtering per Render Pipeline with the `SupportedOnRenderPipeline` attribute.

- Editor: Modified the *Create* menu so it now contains a script template for an empty C\# Script and a Scriptable Object Script. In addition, the *C\# Script* menu item has been renamed to *MonoBehaviour Script*.
    (UUM-60811)

- Editor: Renamed Post-processing and Lighting Quality settings to Tiers.

- Editor: Reorganized the Edit menu.

- Editor: The menu **Animation item** has been renamed to **Animation Clip**.
    (UUM-60811)

- Editor: Updated OpenSSL to 1.1.1w.
    (UUM-53226)

- GI: Added missing color legends for the Lighting Visualizations Colors panel, to explain the colors used in the Texel Validity Scene View Mode.

- GI: Added the *Bake Reflection Probes* menu item.

- GI: Added the *Clear Baked Data* menu item.

- GI: Changed packing of instances into lightmap atlases to be spatially coherent, and prefer packing instances that are located close to be together.

- GI: Changed several scene view modes to have lit shading, to make them easier to read.

- GI: Exposed a "Lightmap Scale" slider for baked preview mode, which lets you quickly change the effective lightmap resolution.

- GI: Finalize APV baking using new probe baking API.

- GI: Implemented tests which target meta passes without light baking.

- GI: Improved and optimized both undo and redo in VFX Graph.

- GI: Improved Typeset lightmap and light probe numbers in the Lighting Window.

- GI: Optimized light baking input extraction by parallelizing surface area calculations.

- GI: Optimized the initialization time for GPU lightmapper bakes.

- Graphics: Added the option *Use Legacy Lightmaps* to disable lightmap texture arrays when GPU Resident Drawer is enabled.

- Graphics: Added three new `UNITY_DOTS_INSTANCED_PROP` variants to give users more control over DOTS instanced property loading performances.

- Graphics: Added `ShadowDrawingSettings.splitIndex` to control which split index is drawn for a shadow renderer list.

- Graphics: Improved CPU performance when binding geometry buffers \(i.e. unity_MeshVertexBuffers_RT\) to ray tracing hit shaders

- Graphics: Improved culling performance when using Batch Render Group.

- Graphics: Improved the performance and memory requirements of Texture API calls such as LoadRawTextureData that write to a Texture2D that was created with the TextureCreationFlags.DontUploadUponCreate flag.
    ([UUM-35989](https://issuetracker.unity3d.com/issues/texturecreationflags-dot-dontuploaduponcreate-does-not-prevent-an-increase-to-the-refcount-of-texturedata))

- Graphics: Kick GameObjects shadow casters culling jobs earlier to improve performance.

- Graphics: Optimized DOTS instanced properties loading code for URP and HDRP stock shaders.

- Graphics: Updated platform macros for VRR code.

- HDRP: Add support for fixing `IRenderPipelineGraphicsSettings` on the HDRP Wizard.

- HDRP: Added a new LOD mode for the High Quality Line Renderer that is based on screen coverage.

- HDRP: Added a slider to High Quality Line Rendering Volume Component to specify when to omit depth and motion vector write if alpha is too low.

- HDRP: Added a warning to the HDRP Wizard if a users project contains materials that can't be upgraded.
    (UUM-46394)

- HDRP: Added an **Importance** property to Reflection Probes. Use this property to indicate the relative priority of the Reflection Probe for sorting.

- HDRP: Added atmospheric scattering from PBR Sky.

- HDRP: Added line light support to the Stacklit, Water, Hair, Eye, and Fabric shaders.

- HDRP: Added new visual effects examples to the HDRP Water Sample example scenes.

- HDRP: Added support for tube-shaped and disc-shaped area lights in the path tracer.

- HDRP: Added the ability to express the width of lines in the High Quality Line Renderer in centimeter units on a per-vertex basis.

- HDRP: Added the option to compose hair before color pyramid but after clouds.

- HDRP: Allow using Solid Angle Culling Mode in Ray Tracing Settings volume override. This ray tracing culling mode rejects objects that are small enough or that are far away from the camera position based on their projected solid angle. These will not be added to the ray tracing acceleration structure.

- HDRP: Avoid clamping to integers for HDR manipulation.
    (UUM-29767)

- HDRP: Following HDRP fixes were made:<br>
    * Support for decals in the Raytracing mode of SSR and SSGI.<br>
    * Changed the value type of *Texture Lod Bias* from integer to float<br>
    * Support debug rendering of decals' light cluster from Window &gt; Rendering Debugger &gt; Fullscreen Debug Mode &gt; LightCluster, Light Category &gt; Decal.<br>
    * Changed the color of the light cluster in the debug view, so that it uses the same color palette as that of tiled lighting.

- HDRP: Improved HDRP build time.
    (UUM-61700)

- HDRP: Improved implementation of line lights for all materials and performance.

- HDRP: Improved path tracer denoising when using AOVs in combination with volumetric fog. Added an option to denoise the volumetric scattering effect separately.

- HDRP: Improved Render Graph Viewer.

- HDRP: Improved scene culling performance when APV is enabled in the project.

- HDRP: Improved skyContext caching when the sky renderer changes.
    ([UUM-43697](https://issuetracker.unity3d.com/issues/player-leaking-memory-when-using-cubemaparrays-and-rendertextures))

- HDRP: Improved the performance of the `FrameSettings.Sanitize` method.

- HDRP: Improved user feedback when a framesetting is disabled.

- HDRP: Improved water surface underwater backface rendering.

- HDRP: Improved water system foam generatorattenuation.

- HDRP: Improved water system performances.

- HDRP: Improvements in the volumetric lighting performance.

- HDRP: Made changes to improve the conversion from string to type for each Custom PP.

- HDRP: Optimized the performance of reflection probe baking by baking all probes in a single batch.

- HDRP: Optimized water surface scripting interactions.

- HDRP: Reduced GC Alloc when using raytracing and HDRP.
    ([UUM-40657](https://issuetracker.unity3d.com/issues/hdrp-garbage-collection-issue-with-ray-traced-reflections))

- HDRP: Reduced the amount of memory that LTC area light tables consume.

- HDRP: Reduced time taken by default scriptable shader stripping.

- HDRP: Updated description of Decal Projector Draw Distance setting to mention HDRP asset setting
    ([UUM-42539](https://issuetracker.unity3d.com/issues/draw-distance-of-the-decal-projector-functions-as-if-the-value-were-set-to-1000-when-the-distance-between-the-camera-and-decal-is-greater-than-1000))

- HDRP: Updated `com.unity.collections` package from 1.4.0 to 2.2.0 in HDRP and light-transport packages.

- Kernel: Added the "-timestamps" command line argument to the player, which makes it prepend timestamps at the beginning of each log line. This setting was previously only available to the Editor.

- Mono: Implemented stack probes for Windows Arm64.

- Package: Alembic: Prevented a NullReferenceException when upgrading a project with URP and Alembic to Unity 2023.3.

- Package Manager: A warning is logged in upm.log when a deprecated UPM environment variable is detected.

- Package Manager: Added the ability to configure the UPM global cache size via the `UPM_MAX_CACHE_SIZE` environment variable or the `maxCacheSize` property in the user configuration file. The default is 10GB.

- Package Manager: Concurrent operations made via the `UnityEditor.PackageManager.Client` class will now be processed sequentially instead of failing with a concurrency error.

- Package Manager: Optimized handling of built-in packages with type module to avoid unnecessary network calls and file operations.

- Package Manager: The global cache that contains the uncompressed contents of registry package tarballs is now obsolete and the `UPM_CACHE_PATH` environment variable is no longer supported.

- Particles: Improved two error messages to include the name of the Particle System.

- Physics: Improved Physics callback dispatching performance by jobifying the processing of trigger and joint break events and only dispatching events that have their callback implemented.

- Profiler: Released Memory Profiler version 1.1.0. Refer to https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1/manual/index.html for more information.

- Scene/Game View: Changed the overlays order for a consistent one in the Overlay Menu.

- Scene/Game View: Updated the Cameras overlay icon to be more descriptive.

- Scripting: Fixed `Hierarchy.Remove` performance issues that could not scale when performed in loop.
    (UUM-63478)

- Scripting: Reduced noise in logs by setting logging level to 'Debug' in `AssemblyUpdater` when collecting ApiUpdater configurations.
    ([UUM-45511](https://issuetracker.unity3d.com/issues/ioexception-is-triggered-by-apiupdater-when-opening-a-project))

- Shadergraph: Added  the**Disable Color Tinting** property to Canvas and Sprite SubTargets. Use this property to override the color completely.
    (UUM-46771)

- Shadergraph: Added a shader variant limit to the Project Settings, and clarified the difference between the variant limits in the Preferences tooltip.

- Shadergraph: Addressed delays related to graph concretization where certain operations were taking longer than expected.

- Shadergraph: Exposed a scope option for Texture3D, CubeMap, and Texture2D Array Blackboard properties.

- Shadergraph: Improved clarity and behavior of Blackboard properties when options change. Renamed **Exposed** to **Show in Inspector**.

- Shadergraph: Improved the performance of undo/redo operations in large graphs.
    ([UUM-52220](https://issuetracker.unity3d.com/issues/editor-loads-for-a-long-time-when-doing-an-undo-action-in-a-large-shader-graph))

- Shadergraph: Removed the **Global/Local** scope for Keyword properties and replaced them with an **Is Overridable** toggle. Updated the corresponding option enablement to clarify behavior.

- Shadergraph: Updated the toolbar UI to make it more similar to VFX Graph.

- Shaders: When compiling shaders with DXC and targeting Metal, HLSL `min16float` instructions will be converted to 16-bit floating point \(MSL `half`\) instructions.

- SRP Core: Added GPU Resident Drawer debug panel to display culling stats when Instanced Drawing is enabled.

- SRP Core: Added icons and fixed bugs in Render Graph Viewer.

- SRP Core: Dumping in the temp folder the stripping of IRenderPipelineGraphicsSettings

- SRP Core: Improved and unified render graph profiling markers.

- SRP Core: Improved execution performance with Render Graph.

- SRP Core: Improved Render Graph Viewer UI to allow jumping to pass definitions in C\# IDE.

- SRP Core: Improved the CPU performance of the Native Render Pass Render Graph compiler by 15-40% \(combined with NativeList PR and other optimization\), depending on the complexity of the rendering and the runtime device.

- SRP Core: Improved the resource pooling system in Render Graph.

- SRP Core: Improved `BeginRenderPass` CPU performance in the Native Render Pass Render Graph \(URP\).

- SRP Core: Merged rendergraph native render passes that have different depths.

- SRP Core: Prevented the unnecessary store op of MSAA buffers in URP when using Native Render Pass Render Graph.

- SRP Core: Reduced `AddRaster/Compute/UnsafeRenderPass` Render Graph API CPU cost by not clearing internal arrays. Now it relies on the handle IsValid\(\) API instead.

- SRP Core: Replaced the overlays inside the RenderGraph Viewer with a fixed side panel.

- SRP Core: Replaced `DynamicArray` with `NativeList` in `NativeRenderPassCompiler` to improve performance.

- SRP Core: Small optimization, frame allocation checks of the Render Graph resource pool are now enabled through Validation checks.

- SRP Core: Validation checks of Render Graph can now be enabled or disabled from the Editor. They are enabled by default, and disabling them slightly improves Render Graph performance.

- SRP Core: `RenderGraphObjectPool` is now three times faster with `RasterRenderRenderGraphPass` objects by using UnityEngine.Pool.

- Text: Improved dynamic FontAsset initialization time and reduced the required number of managed memory allocations.

- uGUI: Provided early out to scenarios where a null mesh was being set on a `CanvasRenderer`.

- UI Elements: Refactored the TreeView and MultiColumnTreeView control to use the Hierarchy as its data structure.

- UI Toolkit: Added support for defining null `UxmlObjects` by using the `<null/>` tag.

- UI Toolkit: Added support for generic `UxmlAttributeConverters` and Types.

- UI Toolkit: Added support for setting the searchfield placeholder text via UXML.

- UI Toolkit: Added support for `UxmlObjects` to use custom property drawers for their serialized data.

- UI Toolkit: Added the ability to preview changes to the inline value of a UXML attribute or a USS property In the UI Builder, even if they are bound.

- UI Toolkit: Added undo/redo functionality for when you create a binding on attributes or style properties.
    (UUM-49503)

- UI Toolkit: Added validation of UXML attribute and element names to ensure they are valid XML names.
    ([UUM-54829](https://issuetracker.unity3d.com/issues/ghost-attributes-saved-in-uxml-files))

- UI Toolkit: Added warning for UxmlAttributes in a non UxmlElement class.
    (UIT-2017)

- UI Toolkit: Changing a UxmlElements namespace or class name is now supported with the MovedFromAttribute.

- UI Toolkit: Exposed the `align-content` API in the Editor, via the **Align Content** property in the **Align** section of the Builder Inspector.
    (UIT-1703)

- UI Toolkit: Improved the performance of the UXML attributes view in the builder during undo/redo operations.
    (UIT-2161)

- UI Toolkit: Improved the UI Builder performance when using UXML serialization and data bindings.

- UI Toolkit: Improved the UI Toolkit performance by reducing the number of managed memory allocations \(GC.Alloc\), specifically when using a virtualized ListView containing Label items.
    (UUM-57824)

- UI Toolkit: Improved UI Builder Attribute type picker field to use a popup selector instead of a completer.
    ([UUM-59486](https://issuetracker.unity3d.com/issues/typeloadexception-is-thrown-when-entering-an-invalid-type-in-the-binding-window-in-ui-builder))

- UI Toolkit: Modified the builder attribute field tooltips so they now include the value.

- UI Toolkit: The Editor now tracks which fields are overridden in UXML in the UxmlSerializedData. During the deserialize process, the Editor only applies the overridden fields instead of all of them.

- UI Toolkit: The UI Builder is improved to no longer react to asset changes unnecessarily if it's not opened.
    (UIT-2157)

- UI Toolkit: Updated the bound fields in the UI Builder Inspector so they can be navigated through keyboard events.

- Universal RP: Added checks to avoid building shadow atlases, adjusting shadow resolution, calculating rendering layers, and running other related operations when their features are disabled.

- Universal RP: Bloom shader variants are now stripped per feature \(LQ, LQ Dirt, HQ, HQ Dirt\).

- Universal RP: Disabled implicit use of all globals in URP passes

- Universal RP: Improved performance for Deferred Rendering when using many lights.

- Universal RP: Improved performance for `AdditionalLightShadowCasterPass` and `BuildAdditionalLightsShadowAtlasLayout`.

- Universal RP: Improved performance when creating shadow data.

- Universal RP: Improved runtime performance by adding checks for `_ALPHATEST_ON` when rendering depth, shadows, and depth normals.

- Universal RP: Improved stripping logic for Accurate G-buffer normals when using Deferred rendering on Vulkan.

- Universal RP: New Renderer Feature updated with Render Graph code.

- Universal RP: Optimized bloom post processing effect CPU performance. Converted many RasterPass into a single UnsafePass.

- Universal RP: SSAO CPU optimization. Many RasterPass into single UnsafePass.

- Universal RP: Updated NewRendererFeature Template.

- Universal Windows Platform: Improved the performance of repeating checks on whether the accelerometer and gyrometer are supported.

- URP: Enabled APV Disk Streaming in URP.

- URP: Enabled the APV Lighting Scenario Baking in URP.

- URP: Enabled `renderViewportScale` for XR intermediate textures.

- VFX Graph: Improved AddComponent performance for VFX by precaching script pointers in common case operation.

- VFX Graph: Improved and optimized both undo and redo.

- VFX Graph: Improved compilation times with VFX Graph using Subgraphs.

- VFX Graph: Improved error feedback and added more error feedback.

- VFX Graph: Improved Position, Collision, and Kill blocks.

- VFX Graph: Improved the collision system so it is more stable, robust, and energy conservative.

- VFX Graph: Improved the performance of VFX.ProcessCommandList by skipping the use of a RenderingCommandBuffer.

- VFX Graph: Improvements to texture types to allow using in branch operators.
    ([UUM-38037](https://issuetracker.unity3d.com/issues/vfx-graph-branch-node-does-not-accept-texture-input))

- VisionOS: Added VisionOS as a target for Windows and Linux.
    (UUM-63466)

- Web: Improved performance for instance rendering in WebGPU.

- WebGL: Improved Web builds to be able to allocate up to 4GB of WebAssembly Memory, up from the previous limit of 2GB. Note that at the time of development, this feature did not work in Firefox \( https://bugzilla.mozilla.org/show_bug.cgi?id=1838218 \), so the default memory limit on the web is still set to 2048 MB.

- WebGL: Removed redundant filesystem persistence operations, to improve IndexedDB filesystem performance.



## API Changes

- Accessibility: Added: Added mobile screen reader support for sliders, allowing them to be made compatible with TalkBack \(Android\) and VoiceOver \(iOS\).

- Accessibility: Added: Support added for the Dismiss Gesture \(Two-finger scrub\) on iOS and the Dismiss Action \(Action Menu item\) on Android when using a screen reader.

- Accessibility: Added: support for reading the bold text system setting on Android and iOS.

- Accessibility: Added: support for reading the closed captioning system setting on Android and iOS.

- Accessibility: Added: support for reading the font scale system setting on Android and iOS.

- Accessibility: Changed: Made label parameter on AccessibilityHierarchy.AddNode and AccessibilityHierarchy.InsertNode null by default to make some use cases easier to achieve

- Accessibility: Changed: Toggle role added to the AccessibilityRole enum.

- AI: Added: All the new `NavMeshEditorHelpers.CollectSourcesInStage()` methods have been copied from the `NavMeshBuilder.CollectSourcesInStage()` methods, which, in turn, have been deprecated.

- AI: Added: `NavMesh.GetAreaNames()` has been added to replace the deprecated method `GameObjectUtility.GetNavMeshAreaNames()`.

- AI: Deprecated: All methods from `GameObjectUtility` related to NavMesh area names have been deprecated. Use the similar methods from the `NavMesh` class instead.

- AI: Deprecated: All methods from `GameObjectUtility` that assign and retrieve NavMesh area types to/from GameObjects have been deprecated. Instead, use `NavMeshBuildMarkup` and `UnityEngine.AI.NavMeshBuilder` to designate different area types in a generated NavMesh.

- AI: Deprecated: The editor-only `NavMeshBuilder` class has been deprecated. Use `UnityEngine.AI.NavMeshBuilder` instead.

- AI: Deprecated: The `NavMeshBuilder.CollectSourcesInStage()` methods have been deprecated. Use `NavMeshEditorHelpers.CollectSourcesInStage()` instead.

- Android: Added: ConfigurationManager has new APIs:<br>
    * ApplyPluginList.AddPluginFromPath<br>
    * ApplyPluginList.AddPluginFromRaw<br>
    * Ndk.DebugSymbolLevel

- Android: Changed: `Unity.Android.Gradle.GradlePropertiesFile.EnableUncompressedNativeLibs` was replaced with `Unity.Android.Gradle.JniLibs.UseLegacyPackaging`.

- Core: Added: API to force active set for APV.
    (UUM-64028)

- Core: Added: ContextContainer to SRP Core. A storage container which works like a dictionary with the key being a generic type id and the value being the value of the given type.

- Core: Added: `Component.GetComponentIndex()` returns a components index on it's `GameObject`.

- Core: Added: `ContentLoadInterface.GetIntegrationTimeMS()` and `ContentLoadInterface.SetIntegrationTimeMS()` for timeslicing integration from Content Files.

- Core: Added: `Object.Instantiate(Object,Scene)` allows for directly instantiating an object to a specific scene.

- Editor: Added: a flag for recursive dependency calculation.  For use with the Compatibility Pipeline API.

- Editor: Added: Added API for collecting in-scene assets and promoting them to project assets.

- Editor: Added: Added RenderingLayerMask as a separate Runtime structure.

- Editor: Added: Added the ScriptableRenderPass.requiresIntermediateTexture flag  to allow individual ScriptableRenderPasses to request offscreen rendering

- Editor: Added: Expose DropdownMenu contextual menu API

- Editor: Added: Exposed new MenuItem attribute constructor with a path to iconResource.

- Editor: Added: Layout field in the DropdownMenuDescriptor to the behavior of the menu when there is a large number of items.

- Editor: Added: Make `OverlayCanvas.SetOverlaysEnabled` and `OverlayCanvas.overlaysEnabled` public API.

- Editor: Added: PrefabUtility callbacks for prefab instance apply.

- Editor: Added: public methods RegisterToolContext and DeregisterToolContext to the ShortcutManager class to allow users to register and unregister custom shortcut contexts.

- Editor: Added: the IShortcutToolContext interface to allow users to create their own custom shortcut context.

- Editor: Added: `EditorGraphicsSettings.TryGetRenderPipelineSettingsForPipeline` to access settings of other pipelines than the currently active pipeline.

- Editor: Added: `GameObject.GetComponentAtIndex()` returns the component at the specific index on a `GameObject`.

- Editor: Added: `HandleUtility.GetOverlappingObjects` for getting an ordered list of all pickable objects under the give mouse location.

- Editor: Added: `HandleUtility.RegisterRenderPickingCallback` and a few peripheral structures that enables custom rendering-based picking solutions to be developed.

- Editor: Added: `SceneManager.MoveObjectToSceneBatch` allows for moving objects in batches to a scene.

- Editor: Changed: EditorUserBuildSettings.androidCreateSymbols was replaced with UnityEditor.Android.UserBuildSettings.DebugSymbols.level and UnityEditor.Android.UserBuildSettings.DebugSymbols.format.

- Editor: Changed: Renamed ArticulationBody.velocity to ArticulationBody.linearVelocity in order for the API to be symmetric with ArticulationBody.angularVelocity

- Editor: Changed: Renamed Rigidbody.velocity to Rigidbody.linearVelocity in order for the API to be symmetric with Rigidbody.angularVelocity

- Editor: Deprecated: The property ChildCount on HierarchyNodeFlattened was renamed to ChildrenCount.<br>
    The following methods are now deprecated: GetExpanded replaced by DoesNotHaveFlags\(Collapsed\), GetSelected replaced by HasFlags\(Selected\), SetExpanded replaced by ClearFlags\(Collapsed\), and SetSelected replaced by SetFlags\(Selected\).

- Editor: Deprecated: Using XRSettings.enabled to enable/disable XR for an application is now deprecated in favor of calling Start\(\)/Stop\(\) on an XRDisplaySubystem instance.<br>
    Using XRSettings.LoadDeviceByName to load XR devices is now deprecated in favor of querying subsystem descriptors to create and start the subsystems of your choice with the SubystemManager.

- Editor: Deprecated: `ObjectIdResult.DecodeIdFromColor`. Users are now encouraged to use `HandleUtility.DecodeSelectionId` for decoding and `HandleUtility.EncodeSelectionId` for encoding selection IDs.

- Editor: Obsoleted: Made PropertyCollectionAttribute obsolete. Use PropertAttribute constructor argument applyToCollection to make a collection attribute.

- Editor: Obsoleted: Using Unsupported.CaptureScreenshotImmediate will now result in a compilation error. Please use ScreenCapture.CaptureScreenshot instead.

- Editor: Removed: IOSLaunchScreenType.CustomXib launch screen option was removed.

- Editor: Removed: SceneManager.MoveObjectToSceneBatch  becase it was never was properly exposed.

- EmbeddedLinux: Deprecated: UnityEditor.EmbeddedLinuxArchitecture enum and UnityEditor.EditorUserBuildSettings.selectedEmbeddedLinuxArchitecture are deprecated. UnityEditor.EmbeddedArchitecture and UnityEditor.EmbeddedLinux.EmbeddedLinuxSettings.Get\(\).architecture should be used instead.

- GI: Added: Add functions for better manipulating LightTransport.BufferSlice, including LightTransport.BufferID.Slice, LightTransport.BufferSlice.SafeReinterpret and LightTransport.BufferSlice.UnsafeReinterpret.

- GI: Added: New light probe baking API. A data driven, stateless, public API for GI probe baking without dependencies on game objects. The API provides CPU and GPU integrators for direct and indirect radiance, validity and a post processing API for conversion to irradiance and other operations needed to composite results before rendering.

- GI: Changed: Added IDisposable to LightTransport.IProbeIntegrator, LightTransport.IWorld and LightTransport.PostProcessing.IProbePostProcessor interfaces.

- GI: Changed: Change LightTransport.BufferSlice to carry a type annotation, indicating the type of elements in the buffer slice.

- GI: Changed: Changed LightTransport.IDeviceContext.WriteBuffer and LightTransport.IDeviceContext.ReadBuffer to take a LightTransport.BufferSlice rather than a LightTransport.BufferID. This lets you provide an offset for your reads and writes.

- GI: Changed: Only one of ignoreDirectEnvironment and ignoreIndirectEnvironment is relevant in each of the IntegrateRadiance methods in IProbeIntegrator.<br>
    Removed the unnecessary ignoreIndirectEnvironment parameter from LightTransport.IProbeIntegrator.IntegrateDirectRadiance.<br>
    Removed the unnecessary ignoreDirectEnvironment parameter from LightTransport.IProbeIntegrator.IntegrateIndirectRadiance.
    ([UUM-61353](https://issuetracker.unity3d.com/issues/only-one-of-ignoredirectenvironment-and-ignoreindirectenvironment-are-relevant-in-api-signature))

- GI: Changed: Renamed LightTransport.IDeviceContext.WaitForAsyncOperation and LightTransport.IDeviceContext.IsAsyncOperationComplete to LightTransport.IDeviceContext.Wait and LightTransport.IDeviceContext.IsComplete.

- Graph Tool Foundation: Removed: GTF and CSO modules removed from the editor. Use package com.unity.graphtoolsauthoringframework instead.

- Graphics: Added: Added a "Texture.SetStreamingTextureMaterialDebugProperties" overload that takes in a "materialTextureSlot" integer. This overload can be used to debug any \(non-hidden\) texture property on materials used by renderers.

- Graphics: Added: API to reconstruct SRP using a certain IRenderPipelineGraphicsSettings in the Editor.

- Graphics: Added: New method overloads accepting GraphicsTexture parameters were added to the Graphics.CopyTexture API

- Graphics: Added: Texture2D.CopyPixels, Texture2DArray.CopyPixels, Texture3D.CopyPixels, Cubemap.CopyPixels, CubemapArray.CopyPixels allow copying readable pixel data only on the CPU.

- Graphics: Added: UseBufferRandomAccess and UseTextureRandomAccess to IRasterRenderGraphBuilder

- Graphics: Added: watermark API to indicate if watermark is visible.

- Graphics: Changed: BatchDrawCommand.visibleCount no longer has to be set to 1 when BatchDrawCommandFlags.HasSortingPosition is set

- Graphics: Changed: HLSL `min16float` variables are now translated to MSL `float` in all CPU visible buffers \(e.g. Constant Buffers, Structured Buffers, Vertex Shader Input\). When accessing these values inside shaders, they are casted to MSL `half` \(16-bit\) for faster arithmetic operations. Any project that uses `min16float` or `half` in shaders and accesses this data as 16-float \(from CPU\) on iOS is incompatible with this change. For these cases, a new `#pragma metal_fxc_allow_float16_in_cpu_visible_buffers` was added so that HLSL `min16float` variables are converted to MSL `half` in all CPU visible buffers \(just like before\).

- Graphics: Changed: Updated contextual menu drawer API with PropertyDrawer information.

- HDRP: Added: Added an API to set and get the material type via script on HDRP Materials.

- HDRP: Added: Fix missing API to get deformation buffer
    (UUM-48355)

- HDRP: Added: New forceVisible API on light to get information from a light from SRP even if it is not in frustrum.

- Package: Added: Added `GetCustomId` method to PlayerInfo

- Package: Added: Added `SignInWithSteamAsync` method with `appId` parameter for Multiple App Id Support

- Package: Changed: Added `LinkWithSteamAsync` method with `appId` parameter for Multiple App Id Support

- Particles: Added: New custom vertex streams: particle index, mesh axis of rotation, and color packed as 2 floats.

- Physics: Changed: Collider.material now returns PhysicsMaterial instead of PhysicMaterial

- Physics: Changed: Collider.sharedMaterial now returns PhysicsMaterial instead of PhysicMaterial

- Physics: Changed: Renamed PhysicMaterial into PhysicsMaterial

- Physics: Changed: Renamed PhysicMaterialCombine to PhysicsMaterialCombine

- Physics: Changed: Renamed Rigidbody.angularDrag to Rigidbody.angularDamping to create symmetry between ArticulationBody and Rigidbody APIs

- Physics: Changed: Renamed Rigidbody.drag to Rigidbody.linearDamping to create symmetry between ArticulationBody and Rigidbody APIs

- Physics: Obsoleted: PhysicMaterial is now obsolete. All references to PhysicMaterial are upgradeable to PhysicsMaterial when updating your project.

- Physics: Obsoleted: PhysicMaterialCombine is now obsolete. All references to PhysicMaterialCombine are upgradeable to PhysicsMaterialCombine when updating your project.

- Physics: Removed: Removed long deprecated type field SoftJointLimit.bouncyness

- Physics: Removed: Removed long deprecated type field SoftJointLimit.damper

- Physics: Removed: Removed long deprecated type field SoftJointLimit.spring

- Player: Added: `AsyncInstantiateOperation.GetIntegrationTimeMS()` and `AsyncInstantiateOperation.SetIntegrationTimeMS()` for time slicing integration times of `InstantiateAsync()`.

- Player: Added: `Object.InstantiateAsync<T>()`.

- QNX: Deprecated: UnityEditor.QNXArchitecture enum, UnityEditor.EditorUserBuildSettings.selectedQnxArchitecture, UnityEditor.EditorUserBuildSettings.selectedQnxOsVersion are deprecated. UnityEditor.EmbeddedArchitecture and UnityEditor.QNX.QNXSettings.Get\(\).architecture should be used instead.

- Scripting: Added: Constructor to TextAsset which takes a ReadOnlySpan of bytes.

- Scripting: Added: Every hierarchy node type handler now has access to an member hierarchy command list in which they can write to whenever they want. This is to simplify the workflow of integrating changes into the hierarchy, which in turn makes the ChangesPending and IntegrateChanges methods optional.
    (UUM-58062)

- Scripting: Added: New methods on Hierarchy class: GetChild to retrieve a child at specified index, GetChildrenCountRecursive to get number of children including children of children, DoesChildrenNeedsSorting to get whether or not a node requires its children to be sorted, and EnumerateChildren to get a children enumerable to iterate children without copying them.<br>
    New methods on HierarchyFlattened class: EnumerateChildren to get a children enumerable for the specified node, GetChildrenCountRecursive to get number of children including children of children.<br>
    New methods on HierarchyViewModel class: several methods to manipulate and query bit flags on nodes, such as SetFlags, ToggleFlags, ClearFlags, HasFlags, DoesNotHaveFlags, GetNodesWithFlags, GetIndicesWithFlags, EnumerateNodesWithFlags and EnumerateNodesWithoutFlags.<br>
    New classes and structs to support new functionality: several new enumerables, such as HierarchyFlattenedNodeChildren, HierarchyNodeChildren and HierarchyViewNodesEnumerable.<br>
    A new enum flags HierarchyNodeFlags used by the HierarchyViewModel.<br>
    A new struct HierarchyNodeMapUnmanaged to store unmanaged data per node that is O\(1\) lookup time, implemented as a sparse array.

- Scripting: Changed: Several methods have had their parameter taking a Span changed to a ReadOnlySpan, to indicate that the content of the span will not be modified and only used as input.<br>
    Hierarchy.RegisterNodeTypeHandler now returns the handler.<br>
    The Hierarchy.SortChildren method got a new parameter, to enable sorting recursively.

- Scripting: Changed: The HierarchyViewModel methods used to query flags were ambiguous because it did not specify they meant "all flags" versus "any flags". These methods are now deprecated, and new methods which specify if it is "all flags" versus "any flags" were added.
    (UUM-58061)

- Scripting: Removed: Removed overloads of method Hierarchy.Add that did not take a parent node.
    (UUM-54851)

- Scripting: Removed: UDP SDK package is now deprecated.

- Shaders: Added: Support for typed texture declarations in HLSL which allow developers to sample integer texture formats robustly on all platforms

- SRP Core: Added: Added `TEMPLATE_X_FLT_HALF` shader macros that defines functions with both `min16float` and `float`.

- SRP Core: Added: Added `TEMPLATE_X_HALF` shader macros that define functions using `min16float` only.

- SRP Core: Added: API to manage global textures

- SRP Core: Added: callbacks when RenderPipeline is created or disposed.
    ([UUM-20646](https://issuetracker.unity3d.com/issues/srp-constructor-is-called-when-the-scene-has-not-been-loaded))

- SRP Core: Added: Foveated rendering API to fix FSR rendering

- SRP Core: Added: New useDynamicScaleExplicit flag to render graph's TextureDesc which can be used to control the underlying RenderTexture's dynamic scaling behavior

- SRP Core: Changed: Fixed typo in RenderGraph API, using lowercase for nativeRenderPassesEnabled property

- SRP Core: Changed: Major update of the Native Render Pass Render Graph API \(URP\), moving out of Experimental.

- SRP Core: Changed: Recent UISubset API has been adjusted and UI overlay pass made safer with URP RG.

- SRP Core: Removed: Removed `TEMPLATE_X_REAL` shader macros.

- TextCore: Obsoleted: Obsolete TextSettings.fallbackSpriteAssets.
    ([UUM-52191](https://issuetracker.unity3d.com/issues/glyphs-are-not-loaded-from-addressables-when-using-the-ui-toolkit))

- UI Toolkit: Added: A string array named paths to the drag and drop API to reproduce what was available in the Editor.

- UI Toolkit: Added: API to get the result of the last binding operation for a given binding id.

- UI Toolkit: Added: `disablePlayModeTint` on `VisualElement` to opt-out of playmode tinting. Applies hierarchically so a user could retrieve the `rootVisualElemen`t on an `EditorWindow` to disable playmode tinting entirely on the window.

- UI Toolkit: Added: `toggleOnLabelClick` attribute to Toggle and Foldout. This is enabled by default but can be disabled to prevent clicking on the elements label from triggering the value change.
    (UUM-52184)

- UI Toolkit: Changed: Added Column.comparison and sortingMode on MultiColumnListView and MultiColumnTreeView to give a default sorting algorithm for sortable columns. This replaces the previous sortingEnabled API.

- UI Toolkit: Changed: Exposed the enabledSelf property to both UXML and bindings.

- UI Toolkit: Changed: Make VisualElement.disablePlayModeTint public

- UI Toolkit: Changed: Marked UxmlTraits, UxmlFactory, and associated API as obsolete. This is now replaced by the UxmlElementAttribute.

- Universal RP: Added: Added RG path only function for AddRenderPasses using ContextContainer instead of RenderingData

- Universal RP: Added: ContextContainer items used as frame data for UniversalRenderer and Renderer2D e.g. UniversalLightData &amp; UniversalCameraData.

- Universal RP: Added: Exposed opaqueLayerMask and transparentLayerMask in UniversalRenderingData.

- Universal RP: Added: Made Main Light Shadow Resolution and Additional Light Shadow Resolution settings public in the URP Asset.

- Universal RP: Added: Made the cascade split settings public in the URP Asset.

- Universal RP: Obsoleted: Mark non-rendergraph APIs as obsolete.

- Video: Added: WebCamKind.Unknown to be used as fallback when camera type is not recognized.



## Changes

- 2D: Changed Shadow Caster 2D to provide a message that GPU skinning is not supported when it is enabled.
    (UUM-18815)

- AI: Built-in navigation components are no longer hidden from the *Add Component* menu if the AI Navigation package is not installed. Instead, affected workflows provide shortcuts to install the package.

- AI: Deprecated OffMeshLink component no longer displays in the Add Component Menu under any circumstances.

- Android: The launcher/build.gradle evaluation now depends on unityLibrary/build.gradle evaluation. Therefore, the unityLibrary/build.gradle can no longer have any dependencies on the launcher/build.gradle.

- Android: Unity will no longer need to force debugging symbols if Unity Cloud Diagnostics \(UCD\) is enabled. Users can manually choose the appropriate debug symbol level. Choosing the level affects how stack traces are resolved by UCD. For example, public symbols are enough to properly resolve function names, while debugging symbols provide filenames and line numbers. Debugging symbols, due to their size can increase build time and build size, which might be a limitation for some users.

- Android: Upgraded the default Android Gradle Plugin version to 8.1.3.

- Android: Upgraded the default Gradle version to 8.4.

- Android: Upgraded the default `targetSdkVersion` and `compileSdkVersion` to 34.

- Android: Upgraded the Java Development Kit \(JDK\) version for building Android apps to 17.

- Android: When producing the `symbols.zip` package, the symbols will contain `.so.sym` or `.so.dbg` extension depending on the `debugSymbolLevel`. These extensions are provided by the Android Gradle plugin for backwards compatibility but you can still force the .so extension \(for more information, check out Debug Symbol &gt; format in the Build Settings window\).

- Asset Bundles: Modified the AssetBundle hash so it now depends only on the respective Multiplayer Role settings it targets.

- Asset Bundles: Updated AssetBundle so that the AssetBundle hash now depends on Multiplayer Roles only if the feature is enabled.

- Build Pipeline: Font assets are not stripped from Dedicated Server builds when Dedicated Server Optimizations are enabled.
    ([UUM-713](https://issuetracker.unity3d.com/issues/font-data-is-forced-to-be-included-when-building-to-dedicated-server-platform))

- Build Pipeline: Made the *Player Settings &gt; Dedicated Server optimizations* option, that strips all shaders and fonts, enabled by default.

- Burst: Disabled Direct call for methods that are decorated with both `[BurstCompile]` and `[UnmanagedCallersOnly]` attributes because such methods shouldn't be called directly from managed code.

- Burst: Removed all code specific to DOTS Runtime.

- Burst: Updated the default LLVM version to 16.

- Burst: Used `mimalloc` as the native allocator on Windows to speed up the concurrently executing LLVM work.

- Documentation: The documentation for the Universal Render Pipeline \(URP\) in Unity 6 Preview has moved from a separate URP site to the Unity Manual. URP site pages now redirect to the Unity Manual pages.

- Editor: Accessing Transform data from 'OnDestroy' during an Undo operation is no longer allowed and an error message is logged.
    ([UUM-31100](https://issuetracker.unity3d.com/issues/transform-is-used-before-awake-or-illegal-transform-access-error-appears-when-accessing-gameobject-transform-from-ondestroy-if-the-gameobject-is-deleted-by-an-undo-operation))

- Editor: Added a new RenderingLayerMask type for serialized property and a RenderingLayerMaskField to draw it.

- Editor: Added command to support Hub creating a new project, and connecting a project to Unity Version Control.

- Editor: Added support for hiding RenderPipelineGraphicsSettings in GraphicsSettings page, persistent Scroll position and persistent active Tab.

- Editor: Build Report printed to the Editor log no longer contains entries for "Scripts" and "Included DLLs".
    ([UUM-56321](https://issuetracker.unity3d.com/issues/the-values-for-levels-and-included-dlls-are-consistently-zero-in-the-editor-dot-log-build-report-when-the-project-is-built))

- Editor: Changed the layout of overlays when dragging over a container that would enforce a specific layout.

- Editor: Do not write cloudProjectId in ProjectSettings.asset anymore since it should only be managed by Services.

- Editor: Improved the visual anchoring of overlays.

- Editor: Modified the ghost behavior of overlays.

- Editor: Remove `CalculateDirtyPaths` and added functionality to use `PersistentManager::GetStreamsWithDestroyedObjects` directly.
    (UUM-48038)

- Editor: Renamed the shortcut that opens the context menu in the Scene view from "Show Action Menu" to "Show Scene view context menu".

- Editor: Reverted the new contextual menu.

- Editor: Reworked the Physics project settings window and converted it to use UI Toolkit.

- Editor: Switched to use drawers for Rendering Layers connected to Tags &amp; Layers.

- Editor: Updated the macOS Editor's minimum OS version requirement to macOS 11.

- Editor: \[Android\] Moved Play Library checks for plugins and gradle dependencies into methods in 23.2 for use in Editor Tests, to avoid building player in every test.
    ([UUM-44744](https://issuetracker.unity3d.com/issues/android-regex-in-checkplaylibraryadded-incorrectly-identifies-play-core-common-libraries))

- Editor: \[Android\] Removed exceptions for unspecified versions when including Play Libraries due to logic changes when fixing Regex for Core-Common.
    ([UUM-44744](https://issuetracker.unity3d.com/issues/android-regex-in-checkplaylibraryadded-incorrectly-identifies-play-core-common-libraries))

- GI: Added code signing for Unity denoising DLLs.

- GI: Moved code related to sampling to its own subfolder in the Light Transport package.

- Graphics: BatchRendererGroup now supports procedural and indirect draw commands

- Graphics: Camera API that wasn't compatible with SRP's now correctly logs warnings/errors where applicable. Also, updated documentation to reflect SRP capabilities in Camera API.

- Graphics: Moved the editor for GlobalSettingsAssets directly to ProjectSettings &gt; Graphics.

- Graphics: Use the unified RenderGraph compiler instead of defaulting to the older HDRP implementation for OpenGLES.

- Graphics: When `IRenderPipelineGraphicsSettingsStripper` is defined, it owns the stripping of the `IRenderPipelineGraphicsSettings`, which previously required `isAvailableInPlayerBuild`.
    (XPIPELINE-804)

- HDRP: Added Volumetrics settings to Area lights similar to other light types, to control their influence on volumetric fog when using the path tracer.

- HDRP: Changed how the mask map ambient occlusion channel is taken into account in rendering to have better consistency between area lights and emissive quads.

- HDRP: Improved the usage of the HDRP runtime resources.

- HDRP: Made the *Texture Streaming* scene view debug draw mode unavailable. Use the reworked Mipmap Streaming debug views in the Rendering Debugger instead.

- HDRP: Rectangle light and Line light now share same implementation.

- IL2CPP: Prevented references to unused shared generic types from being collected when the script debugging is enabled.

- License: Added the option on Unity Personal to disable or customize the Made with Unity splash screen.

- macOS: Updated the macOS Runtime's minimum OS version requirement to macOS 11.

- Package: Promoted deprecated version of Sequences package.

- Package: Updated the package version of com.unity.scripting.python to 7.0.1.

- Package Manager: Changed the min-width of the package manager window, sidebar, and package list.
    ([UUM-72856](https://issuetracker.unity3d.com/issues/package-manager-window-remove-slash-install-button-is-not-visible-when-the-window-has-low-width))

- Package Manager: Deprecated the UPM environment variable `UPM_NPM_CACHE_PATH`. Use the `UPM_CACHE_ROOT` environment variable instead.

- Package Manager: Modied `Client.AddAndRemove` so it does not throw an error if the same packages are specified in `packagesToAdd` and `packagesToRemove`.

- Package Manager: The package installation folder names have been shortened from `<packageName>@<version>` to `<packageName>` in the `Library/PackageCache` folder.

- Physics: Errors related to mesh data will no longer print the assets path. This change was done in order to decouple error generation from some specific editor only functionality. We will be reworking the error messaging in the following patch releases.

- Physics: Removed compatibility code that allowed Unity to load joints directly from assets created in Unity 4.x and older.

- Physics: `OnTriggerEnter` events now have their matching `OnTriggerStay` dispatched after an `OnTriggerEnter` event, rather than wait for all `OnTriggerEnter` events to be dispatched.

- Profiler: Removed extraneous calls to `UpdateRendererBoundingVolumes` when executing an empty `CommandBuffer`.
    ([UUM-33237](https://issuetracker.unity3d.com/issues/gaphics-dot-executecommandbuffer-adds-unwanted-updaterendererboundingvolumes-calls-in-profiler))

- Profiler: The Highlights profiler module is now visible by default.

- Shadergraph: Now all the nodes connected to the BaseColor block are taken into shader codegen when generating the picking pass, allowing custom picking-specific code to be included through custom function nodes.
    (UUM-62636)

- UI: Added *Unsupported MSAA Fallback* in Player settings to specify how to handle cases with unsupported sample counts.
    ([UUM-741](https://issuetracker.unity3d.com/issues/android-2xmsaa-does-not-work-on-mali-devices-when-post-processing-is-enabled))

- UI Toolkit: Added a checked background to GradientField so the transparency is easier to see.
    ([UUM-60804](https://issuetracker.unity3d.com/issues/alpha-channel-is-not-shown-as-a-checkboard-when-using-uitoolkit-gradient))

- UI Toolkit: Removed unused border element from GradientField.

- UI Toolkit: Users can no longer drag disabled selectors when using in-context editing in the UI Builder.
    (UUM-16090)

- Universal RP: Added per-renderer filtering for renderer features.

- Universal RP: Modified the Scene view camera so it now uses the same renderer that `MainCamera` uses in the scene instead of always using Default Renderer.

- Universal RP: Moved the `RenderObjects` renderer feature out of the `Experimental` namespace.

- Universal RP: The Auto option in SH Evaluation Mode, in the URP Asset, now chooses Per Vertex instead of Per Pixel on mobile and similar devices.
    ([UUM-60483](https://issuetracker.unity3d.com/issues/auto-sh-evaluation-mode-doesnt-use-per-vertex-on-mobile-and-switch))

- URP: Added `RenderGraph` support to URP Samples.

- URP: In the Render Graph Viewer, you can now open the tool when the compatibility mode is enabled.
    (UUM-74128)

- URP: Vulkan URP will use MSAA samples count fallback from Player settings. Prior to this x2 fallback would have been required upgrade to x4.
    ([UUM-741](https://issuetracker.unity3d.com/issues/android-2xmsaa-does-not-work-on-mali-devices-when-post-processing-is-enabled))

- Version Control: Added a message that appears after the first check-in, which contains a link to invite users to the organization.

- Version Control: Added button for organization owner/admins to upgrade to DevOps subscription.

- Version Control: Added new decorators for retained &amp; locked files.

- Version Control: Moved the button to invite users to the organization from the sub-menu to the toolbar.

- Version Control: Updated description in the package.json, including an updated link to get started.

- XR: Changed the reported `Screen.width` and `Screen.height` when using MagicLeap device.

- XR: Removed the use of an intermediate texture when not required for XR rendering when scaling is used.

- XR: The Oculus XR Plugin package is updated to 4.2.0.

- XR: Updated the Oculus XR Plugin package to 4.1.2.

## Final 6000.0.23f1 Package changes

## Packages updated

- com.unity.collections: [1.2.4](https://docs.unity3d.com/Packages/com.unity.collections@1.2//changelog/CHANGELOG.html) to [2.5.1](https://docs.unity3d.com/Packages/com.unity.collections@2.5//changelog/CHANGELOG.html)

- com.unity.2d.animation: [10.0.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.0//changelog/CHANGELOG.html) to [10.1.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.1//changelog/CHANGELOG.html)

- com.unity.2d.common: [9.0.1](https://docs.unity3d.com/Packages/com.unity.2d.common@9.0//changelog/CHANGELOG.html) to [9.0.6](https://docs.unity3d.com/Packages/com.unity.2d.common@9.0//changelog/CHANGELOG.html)

- com.unity.2d.psdimporter: [9.0.0](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.0//changelog/CHANGELOG.html) to [9.0.3](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.0//changelog/CHANGELOG.html)

- com.unity.2d.spriteshape: [10.0.1](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html) to [10.0.6](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html)

- com.unity.2d.tilemap.extras: [4.0.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.0//changelog/CHANGELOG.html) to [4.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.0//changelog/CHANGELOG.html)

- com.unity.2d.aseprite: [1.0.0](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.0//changelog/CHANGELOG.html) to [1.1.6](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.adaptiveperformance: [5.0.1](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@5.0//changelog/CHANGELOG.html) to [5.1.0](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@5.1//changelog/CHANGELOG.html)

- com.unity.adaptiveperformance.google.android: [1.1.2](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.google.android@1.1//changelog/CHANGELOG.html) to [1.3.1](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.google.android@1.3//changelog/CHANGELOG.html)

- com.unity.addressables: [1.21.12](https://docs.unity3d.com/Packages/com.unity.addressables@1.21//changelog/CHANGELOG.html) to [2.2.2](https://docs.unity3d.com/Packages/com.unity.addressables@2.2//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.7](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.18](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.cinemachine: [2.9.5](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.9//changelog/CHANGELOG.html) to [2.10.1](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.0.5](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.0//changelog/CHANGELOG.html) to [2.5.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.5//changelog/CHANGELOG.html)

- com.unity.formats.alembic: [2.3.2](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.3//changelog/CHANGELOG.html) to [2.4.0](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.24](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.31](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.ide.visualstudio: [2.0.18](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html) to [2.0.22](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.6.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.6//changelog/CHANGELOG.html) to [1.11.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.11//changelog/CHANGELOG.html)

- com.unity.live-capture: [4.0.0-pre.5](https://docs.unity3d.com/Packages/com.unity.live-capture@4.0//changelog/CHANGELOG.html) to [4.0.0](https://docs.unity3d.com/Packages/com.unity.live-capture@4.0//changelog/CHANGELOG.html)

- com.unity.localization: [1.4.4](https://docs.unity3d.com/Packages/com.unity.localization@1.4//changelog/CHANGELOG.html) to [1.5.2](https://docs.unity3d.com/Packages/com.unity.localization@1.5//changelog/CHANGELOG.html)

- com.unity.mathematics: [1.2.6](https://docs.unity3d.com/Packages/com.unity.mathematics@1.2//changelog/CHANGELOG.html) to [1.3.2](https://docs.unity3d.com/Packages/com.unity.mathematics@1.3//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat: [1.3.2](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.3//changelog/CHANGELOG.html) to [1.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.mobile.notifications: [2.2.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.2//changelog/CHANGELOG.html) to [2.3.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.3//changelog/CHANGELOG.html)

- com.unity.polybrush: [1.1.4](https://docs.unity3d.com/Packages/com.unity.polybrush@1.1//changelog/CHANGELOG.html) to [1.1.8](https://docs.unity3d.com/Packages/com.unity.polybrush@1.1//changelog/CHANGELOG.html)

- com.unity.postprocessing: [3.3.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.3//changelog/CHANGELOG.html) to [3.4.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.4//changelog/CHANGELOG.html)

- com.unity.probuilder: [5.1.0](https://docs.unity3d.com/Packages/com.unity.probuilder@5.1//changelog/CHANGELOG.html) to [6.0.4](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html)

- com.unity.services.cloud-diagnostics: [1.0.6](https://docs.unity3d.com/Packages/com.unity.services.cloud-diagnostics@1.0//changelog/CHANGELOG.html) to [1.0.10](https://docs.unity3d.com/Packages/com.unity.services.cloud-diagnostics@1.0//changelog/CHANGELOG.html)

- com.unity.services.user-reporting: [2.0.6](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) to [2.0.11](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- com.unity.purchasing: [4.9.3](https://docs.unity3d.com/Packages/com.unity.purchasing@4.9//changelog/CHANGELOG.html) to [4.12.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.12//changelog/CHANGELOG.html)

- com.unity.recorder: [5.0.0-pre.1](https://docs.unity3d.com/Packages/com.unity.recorder@5.0//changelog/CHANGELOG.html) to [5.1.1](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- com.unity.remote-config: [3.3.2](https://docs.unity3d.com/Packages/com.unity.remote-config@3.3//changelog/CHANGELOG.html) to [4.1.1](https://docs.unity3d.com/Packages/com.unity.remote-config@4.1//changelog/CHANGELOG.html)

- com.unity.remote-config-runtime: [4.0.1](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@4.0//changelog/CHANGELOG.html) to [4.0.2](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@4.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.core: [16.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@16.0//changelog/CHANGELOG.html) to [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@17.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition: [16.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@16.0//changelog/CHANGELOG.html) to [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@17.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition-config: [16.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@16.0//changelog/CHANGELOG.html) to [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@17.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.universal: [16.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@16.0//changelog/CHANGELOG.html) to [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@17.0//changelog/CHANGELOG.html)

- com.unity.rendering.denoising: [1.0.3](https://docs.unity3d.com/Packages/com.unity.rendering.denoising@1.0//changelog/CHANGELOG.html) to [1.0.5](https://docs.unity3d.com/Packages/com.unity.rendering.denoising@1.0//changelog/CHANGELOG.html)

- com.unity.rendering.light-transport: [1.0.0](https://docs.unity3d.com/Packages/com.unity.rendering.light-transport@1.0//changelog/CHANGELOG.html) to [1.0.1](https://docs.unity3d.com/Packages/com.unity.rendering.light-transport@1.0//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.21.5](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.21//changelog/CHANGELOG.html) to [2.1.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.1//changelog/CHANGELOG.html)

- com.unity.services.analytics: [4.4.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@4.4//changelog/CHANGELOG.html) to [6.0.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html)

- com.unity.services.authentication: [2.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@2.6//changelog/CHANGELOG.html) to [3.3.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.3//changelog/CHANGELOG.html)

- com.unity.services.ccd.management: [2.2.2](https://docs.unity3d.com/Packages/com.unity.services.ccd.management@2.2//changelog/CHANGELOG.html) to [3.0.0](https://docs.unity3d.com/Packages/com.unity.services.ccd.management@3.0//changelog/CHANGELOG.html)

- com.unity.services.cloudcode: [2.4.0](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.4//changelog/CHANGELOG.html) to [2.7.1](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.7//changelog/CHANGELOG.html)

- com.unity.services.cloudsave: [2.0.1](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@2.0//changelog/CHANGELOG.html) to [2.2.1](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@2.2//changelog/CHANGELOG.html)

- com.unity.services.core: [1.10.1](https://docs.unity3d.com/Packages/com.unity.services.core@1.10//changelog/CHANGELOG.html) to [1.13.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.13//changelog/CHANGELOG.html)

- com.unity.services.economy: [3.1.1](https://docs.unity3d.com/Packages/com.unity.services.economy@3.1//changelog/CHANGELOG.html) to [3.4.1](https://docs.unity3d.com/Packages/com.unity.services.economy@3.4//changelog/CHANGELOG.html)

- com.unity.services.leaderboards: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@1.0//changelog/CHANGELOG.html) to [2.1.0](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.1//changelog/CHANGELOG.html)

- com.unity.services.lobby: [1.0.3](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.0//changelog/CHANGELOG.html) to [1.2.2](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.2//changelog/CHANGELOG.html)

- com.unity.services.matchmaker: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.matchmaker@1.0//changelog/CHANGELOG.html) to [1.1.5](https://docs.unity3d.com/Packages/com.unity.services.matchmaker@1.1//changelog/CHANGELOG.html)

- com.unity.services.multiplay: [1.0.3](https://docs.unity3d.com/Packages/com.unity.services.multiplay@1.0//changelog/CHANGELOG.html) to [1.2.5](https://docs.unity3d.com/Packages/com.unity.services.multiplay@1.2//changelog/CHANGELOG.html)

- com.unity.services.qos: [1.2.0](https://docs.unity3d.com/Packages/com.unity.services.qos@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.qos@1.3//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.1.8](https://docs.unity3d.com/Packages/com.unity.services.wire@1.1//changelog/CHANGELOG.html) to [1.2.7](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html)

- com.unity.shadergraph: [16.0.3](https://docs.unity3d.com/Packages/com.unity.shadergraph@16.0//changelog/CHANGELOG.html) to [17.0.3](https://docs.unity3d.com/Packages/com.unity.shadergraph@17.0//changelog/CHANGELOG.html)

- com.unity.splines: [2.3.0](https://docs.unity3d.com/Packages/com.unity.splines@2.3//changelog/CHANGELOG.html) to [2.6.1](https://docs.unity3d.com/Packages/com.unity.splines@2.6//changelog/CHANGELOG.html)

- com.unity.test-framework: [1.3.7](https://docs.unity3d.com/Packages/com.unity.test-framework@1.3//changelog/CHANGELOG.html) to [1.4.5](https://docs.unity3d.com/Packages/com.unity.test-framework@1.4//changelog/CHANGELOG.html)

- com.unity.testtools.codecoverage: [1.2.4](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html) to [1.2.6](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html)

- com.unity.timeline: [1.8.4](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) to [1.8.7](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- com.unity.visualeffectgraph: [16.0.3](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@16.0//changelog/CHANGELOG.html) to [17.0.3](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@17.0//changelog/CHANGELOG.html)

- com.unity.visualscripting: [1.8.0](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.8//changelog/CHANGELOG.html) to [1.9.4](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- com.unity.xr.arcore: [5.1.0-pre.8](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.1//changelog/CHANGELOG.html) to [6.0.3](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.0//changelog/CHANGELOG.html)

- com.unity.xr.arfoundation: [5.1.0-pre.8](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.1//changelog/CHANGELOG.html) to [6.0.3](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.0//changelog/CHANGELOG.html)

- com.unity.xr.arkit: [5.1.0-pre.8](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.1//changelog/CHANGELOG.html) to [6.0.3](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.0//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.2.1](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.2//changelog/CHANGELOG.html) to [2.3.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.3//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.2.1](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.2//changelog/CHANGELOG.html) to [1.5.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.5//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.4//changelog/CHANGELOG.html) to [3.0.5](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html)

- com.unity.xr.legacyinputhelpers: [2.1.10](https://docs.unity3d.com/Packages/com.unity.xr.legacyinputhelpers@2.1//changelog/CHANGELOG.html) to [2.1.11](https://docs.unity3d.com/Packages/com.unity.xr.legacyinputhelpers@2.1//changelog/CHANGELOG.html)

- com.unity.xr.management: [4.3.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.3//changelog/CHANGELOG.html) to [4.5.0](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html)

- com.unity.xr.oculus: [4.0.0](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.0//changelog/CHANGELOG.html) to [4.3.0](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.3//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.8.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.8//changelog/CHANGELOG.html) to [1.12.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.12//changelog/CHANGELOG.html)

- com.unity.formats.fbx: [5.1.0-pre.1](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html) to [5.1.1](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html)

- com.autodesk.fbx: 5.1.0-pre.1 to 5.1.1

- com.unity.learn.iet-framework: [3.1.3](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@3.1//changelog/CHANGELOG.html) to [4.0.2](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@4.0//changelog/CHANGELOG.html)

- com.unity.sequences: [2.1.0](https://docs.unity3d.com/Packages/com.unity.sequences@2.1//changelog/CHANGELOG.html) to [2.1.3](https://docs.unity3d.com/Packages/com.unity.sequences@2.1//changelog/CHANGELOG.html)

- com.unity.terrain-tools: [5.1.0](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.1//changelog/CHANGELOG.html) to [5.1.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.1//changelog/CHANGELOG.html)

- com.unity.profiling.systemmetrics.mali: [1.0.2](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.0//changelog/CHANGELOG.html) to [1.0.3](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.0//changelog/CHANGELOG.html)

- com.unity.scripting.python: [7.0.0](https://docs.unity3d.com/Packages/com.unity.scripting.python@7.0//changelog/CHANGELOG.html) to [7.0.1](https://docs.unity3d.com/Packages/com.unity.scripting.python@7.0//changelog/CHANGELOG.html)

- com.unity.transport: [1.4.0](https://docs.unity3d.com/Packages/com.unity.transport@1.4//changelog/CHANGELOG.html) to [2.3.0](https://docs.unity3d.com/Packages/com.unity.transport@2.3//changelog/CHANGELOG.html)

- com.unity.memoryprofiler: [1.0.0](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.0//changelog/CHANGELOG.html) to [1.1.1](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.5.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.5//changelog/CHANGELOG.html) to [1.10.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.10//changelog/CHANGELOG.html)

- com.unity.multiplayer.tools: [1.1.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@1.1//changelog/CHANGELOG.html) to [2.2.1](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- com.unity.ai.navigation: [2.0.0-pre.3](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) to [2.0.4](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- com.unity.services.deployment: [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.1//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.3//changelog/CHANGELOG.html)

- nuget.castle-core: 2.0.0-pre.4 to 2.0.0

- nuget.moq: 2.0.0-pre.2 to 2.0.0

- com.unity.sysroot: [2.0.5](https://docs.unity3d.com/Packages/com.unity.sysroot@2.0//changelog/CHANGELOG.html) to [2.0.10](https://docs.unity3d.com/Packages/com.unity.sysroot@2.0//changelog/CHANGELOG.html)

- com.unity.sysroot.linux-x86_64: [2.0.4](https://docs.unity3d.com/Packages/com.unity.sysroot.linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.9](https://docs.unity3d.com/Packages/com.unity.sysroot.linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.toolchain.linux-x86_64: [2.0.4](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.9](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.toolchain.macos-x86_64-linux-x86_64: [2.0.4](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.9](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.toolchain.win-x86_64-linux-x86_64: [2.0.4](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.9](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.zivart-player: [2.0.0](https://docs.unity3d.com/Packages/com.unity.zivart-player@2.0//changelog/CHANGELOG.html) to [2.1.0](https://docs.unity3d.com/Packages/com.unity.zivart-player@2.1//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.sentis@2.1.0](https://docs.unity3d.com/Packages/com.unity.sentis@2.1//changelog/CHANGELOG.html)

- [com.unity.entities@1.3.2](https://docs.unity3d.com/Packages/com.unity.entities@1.3//changelog/CHANGELOG.html)

- [com.unity.netcode@1.3.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.3//changelog/CHANGELOG.html)

- [com.unity.charactercontroller@1.2.4](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.2//changelog/CHANGELOG.html)

- [com.unity.physics@1.3.2](https://docs.unity3d.com/Packages/com.unity.physics@1.3//changelog/CHANGELOG.html)

- com.havok.physics@1.3.2

- [com.unity.logging@1.3.2](https://docs.unity3d.com/Packages/com.unity.logging@1.3//changelog/CHANGELOG.html)

- [com.unity.entities.graphics@1.3.2](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.3//changelog/CHANGELOG.html)

- [com.unity.serialization@3.1.2](https://docs.unity3d.com/Packages/com.unity.serialization@3.1//changelog/CHANGELOG.html)

- [com.unity.bindings.openimageio@1.0.0](https://docs.unity3d.com/Packages/com.unity.bindings.openimageio@1.0//changelog/CHANGELOG.html)

- [com.unity.render-pipelines.universal-config@17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal-config@17.0//changelog/CHANGELOG.html)

- [com.unity.path-tracing@1.0.0](https://docs.unity3d.com/Packages/com.unity.path-tracing@1.0//changelog/CHANGELOG.html)

- [com.unity.services.friends@1.1.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html)

- [com.unity.services.vivox@16.5.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.5//changelog/CHANGELOG.html)

- [com.unity.test-framework.performance@3.0.3](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.0//changelog/CHANGELOG.html)

- [com.unity.xr.meta-openxr@2.0.1](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.0//changelog/CHANGELOG.html)

- [com.unity.multiplayer.playmode@1.3.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.3//changelog/CHANGELOG.html)

- [com.unity.dedicated-server@1.3.0](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.3//changelog/CHANGELOG.html)

- [com.unity.services.apis@1.1.0](https://docs.unity3d.com/Packages/com.unity.services.apis@1.1//changelog/CHANGELOG.html)

- [com.unity.services.tooling@1.1.0](https://docs.unity3d.com/Packages/com.unity.services.tooling@1.1//changelog/CHANGELOG.html)

- [com.unity.toolchain.macos-arm64-linux-x86_64@2.0.3](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-arm64-linux-x86_64@2.0//changelog/CHANGELOG.html)

- [com.unity.toolchain.win-arm64-linux-x86_64@1.0.3](https://docs.unity3d.com/Packages/com.unity.toolchain.win-arm64-linux-x86_64@1.0//changelog/CHANGELOG.html)

- [com.unity.services.ugc@3.0.1](https://docs.unity3d.com/Packages/com.unity.services.ugc@3.0//changelog/CHANGELOG.html)

- [com.unity.services.ugc.bridge@3.0.0](https://docs.unity3d.com/Packages/com.unity.services.ugc.bridge@3.0//changelog/CHANGELOG.html)

- [com.unity.dt.app-ui@1.1.0](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.1//changelog/CHANGELOG.html)

- [com.unity.addressables.android@1.0.4](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)

- [com.unity.microsoft.gdk@1.2.3](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.2//changelog/CHANGELOG.html)

- [com.unity.microsoft.gdk.tools@1.2.3](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.2//changelog/CHANGELOG.html)

- [com.unity.sharp-zip-lib@1.3.8](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.3//changelog/CHANGELOG.html)

- [com.unity.muse.common@2.0.3](https://docs.unity3d.com/Packages/com.unity.muse.common@2.0//changelog/CHANGELOG.html)

- [com.unity.muse.sprite@1.1.1](https://docs.unity3d.com/Packages/com.unity.muse.sprite@1.1//changelog/CHANGELOG.html)

- [com.unity.muse.texture@1.1.1](https://docs.unity3d.com/Packages/com.unity.muse.texture@1.1//changelog/CHANGELOG.html)

- [com.unity.services.levelplay@8.3.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.3//changelog/CHANGELOG.html)

- [com.unity.multiplayer.center@1.0.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.center@1.0//changelog/CHANGELOG.html)

- [com.unity.polyspatial@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial@2.0//changelog/CHANGELOG.html)

- [com.unity.polyspatial.visionos@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@2.0//changelog/CHANGELOG.html)

- [com.unity.polyspatial.xr@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@2.0//changelog/CHANGELOG.html)

- [com.unity.polyspatial.extensions@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@2.0//changelog/CHANGELOG.html)

- [com.unity.xr.visionos@2.0.4](https://docs.unity3d.com/Packages/com.unity.xr.visionos@2.0//changelog/CHANGELOG.html)

- [com.unity.ext.flatsharp@1.1.1](https://docs.unity3d.com/Packages/com.unity.ext.flatsharp@1.1//changelog/CHANGELOG.html)

- [com.unity.services.multiplayer@1.0.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@1.0//changelog/CHANGELOG.html)

- [com.unity.multiplayer.widgets@1.0.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.widgets@1.0//changelog/CHANGELOG.html)

**Packages deprecated**

- com.unity.purchasing.udp - "This package is no longer supported on this editor version."

**Packages no longer available**

- com.ptc.vuforia.engine

**Pre-release packages added**

- [com.unity.purchasing@5.0.0-pre.1](https://docs.unity3d.com/Packages/com.unity.purchasing@5.0//changelog/CHANGELOG.html)

- [com.unity.xr.arcore@6.1.0-pre.1](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.1//changelog/CHANGELOG.html)

- [com.unity.xr.arfoundation@6.1.0-pre.1](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.1//changelog/CHANGELOG.html)

- [com.unity.xr.arkit@6.1.0-pre.1](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.1//changelog/CHANGELOG.html)

- [com.unity.dt.app-ui@2.0.0-pre.6](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.0//changelog/CHANGELOG.html)

- [com.unity.services.moderation@1.0.0-pre.3](https://docs.unity3d.com/Packages/com.unity.services.moderation@1.0//changelog/CHANGELOG.html)

- [com.unity.muse.chat@1.0.0-pre.15](https://docs.unity3d.com/Packages/com.unity.muse.chat@1.0//changelog/CHANGELOG.html)


# 6000.0.23f1 Release Notes

## Features

- Package: Added the Character Controller package, version 1.2.4.



## Improvements

- Documentation: Added a Multiplayer overview page to summarize Unity's multiplayer packages and services.

- HDRP: Added a slider to High Quality Line Rendering Volume Component to specify when to omit depth and motion vector write if alpha is too low.

- HDRP: Added the option to compose hair before color pyramid but after clouds.

- HDRP: Allow using Solid Angle Culling Mode in Ray Tracing Settings volume override. This ray tracing culling mode rejects objects that are small enough or that are far away from the camera position based on their projected solid angle. These will not be added to the ray tracing acceleration structure.

- Package Manager: Concurrent operations made via the `UnityEditor.PackageManager.Client` class will now be processed sequentially instead of failing with a concurrency error.

- Package Manager: Optimized handling of built-in packages with type module to avoid unnecessary network calls and file operations.



## Changes

- Documentation: The documentation for the Universal Render Pipeline \(URP\) in Unity 6 Preview has moved from a separate URP site to the Unity Manual. URP site pages now redirect to the Unity Manual pages.

- Graphics: Use the unified RenderGraph compiler instead of defaulting to the older HDRP implementation for OpenGLES.

- Package: Promoted deprecated version of Sequences package.

- Package Manager: Changed the min-width of the package manager window, sidebar, and package list.
    ([UUM-72856](https://issuetracker.unity3d.com/issues/package-manager-window-remove-slash-install-button-is-not-visible-when-the-window-has-low-width))

- URP: In the Render Graph Viewer, you can now open the tool when the compatibility mode is enabled.
    (UUM-74128)



## Fixes

- 2D: Fixed a crash on `SpriteRenderer::SetupProperties` that was caused when opening a specific project.
    ([UUM-83130](https://issuetracker.unity3d.com/issues/crash-on-spriterenderer-setupproperties-when-opening-a-specific-project))

- 2D: Fixed a Metal error when rendering a Tilemap in chunk mode while the SRP Batcher and GPU Skinning were enabled with Skinned Sprites.

- 2D: Fixed an overlay issue to allow docking above the Sprite Editor toolbar.
    (UUM-83326)

- 2D: Fixed incorrect sampling for TextMesh when used with Pixel Perfect Camera.
    ([UUM-51358](https://issuetracker.unity3d.com/issues/textmeshpro-text-moves-out-of-sync-when-the-grid-snapping-is-set-to-upscale-render-texture-and-the-current-pixel-ratio-is-not-1-1))

- 2D: Fixed the issue with unnecessary calls to `SpriteRenderer.InvokeSpriteChanged` when no Listeners are registered.
    (UUM-83203)

- Android: Fixed an  issue with `Display.main.systemWidth/Display.main.systemHeight` returning incorrect values when the app was in split screen mode.
    ([UUM-77283](https://issuetracker.unity3d.com/issues/android-gameactivity-unity-app-in-split-screen-constantly-resizes-when-rotating-to-portraitupsidedown-orientations))

- Android: Fixed an issue with the `UnitySendMessage` call in C\#. You can now do  `[DllImport("unity")]static extern void UnitySendMessage(string goName, string method, string arg);` if you want to use this function.
    (UUM-74627)

- Android: Updated the Compile SDK version when the Target SDK is below 32.
    (UUM-76199)

- Animation: Fixed a crash that was caused when recreating the Animator bindings by enabling a RigBuilder that binds a transform stream handle; for example, while the Animator was being evaluated.
    ([UUM-80043](https://issuetracker.unity3d.com/issues/crash-on-unityengine-animation-setgenericfloatpropertyvalues-when-keyframing-the-rigbuilder-component-to-enabled-and-disabled))

- Animation: Fixed an issue within animations with events at time "1" throw import warnings when using particular animation lengths.
    (UUM-79396)

- Editor: Fixed a crash in the asset import worker process that occurred when using the External Material location mode in the model importer.
    ([UUM-57498](https://issuetracker.unity3d.com/issues/imported-fbx-models-are-not-visible-in-the-scene-or-previewable-in-the-project-files-when-the-parallel-import-option-is-enabled))

- Editor: Fixed a crash that would occur in the Editor after wireframe selection if strict variant matching was on.
    (UUM-83290)

- Editor: Fixed a crash when sequentially setting values in a managed reference array of strings.
    ([UUM-73968](https://issuetracker.unity3d.com/issues/crash-on-serializedproperty-custom-setstringvalueinternal-when-setting-serializedproperty-string-value))

- Editor: Fixed an error related to Final Blit/Screen Space UIToolkit/uGUI Pass Overlay where the dimensions or sample count of attachment 0 did not match with the RenderPass specifications \(2560 x 20 1AA\) vs \(1469 x 786 1AA\).
    (UUM-71240)

- Editor: Fixed an invalid `m_BackBufferDepth` GfxDevice cached var when `swapChain` was deleted.
    (UUM-78039)

- Editor: Fixed an issue so a drag from an external source will now copy into the project on Linux.
    ([UUM-74904](https://issuetracker.unity3d.com/issues/linux-wayland-error-is-thrown-and-a-file-is-not-copied-to-assets-when-dragging-and-dropping-a-file-in-the-project-view))

- Editor: Fixed an issue to exclude web and gl graphics API in GPU Driven shaders.
    ([UUM-76185](https://issuetracker.unity3d.com/issues/a-bunch-of-shader-warnings-are-thrown-after-switching-platform-to-android-when-using-universal-3d-template))

- Editor: Fixed an issue to prevent users from deleting a parent material without reparenting its children.
    ([UUM-73507](https://issuetracker.unity3d.com/issues/crash-when-selecting-a-certain-material))

- Editor: Fixed an issue where build profiles that show a warning in their settings UI based on the scripting backend were using a method that retrieved the project settings player settings value, instead of the build profile player settings value.
    ([UUM-70188](https://issuetracker.unity3d.com/issues/playersettings-common-scripting-backend-non-active-build-profile-should-check-its-player-settings-scripting-backend-and-not-global-one-to-display-warning))

- Editor: Fixed an issue where cancelable progress bars on macOS would close immediately after the first time one is cancelled.
    (UUM-82263)

- Editor: Fixed an issue where shortcuts didn't work on macOS after completing a rename operation.
    ([UUM-56765](https://issuetracker.unity3d.com/issues/shortcut-for-the-create-empty-child-command-works-just-once-if-setting-any-command-shortcut-to-n))

- Editor: Fixed an issue where the texture size was not reported correctly in the Inspector, if **Load texture data on demand** was enabled.
    ([UUM-77739](https://issuetracker.unity3d.com/issues/texture-does-not-display-its-size-when-observing-through-inspector-preview))

- Editor: Fixed renaming issues with the build profiles in the Build Profile menu when using leading, trailing, or only white space.
    ([UUM-77663](https://issuetracker.unity3d.com/issues/build-profile-gets-a-name-asset-during-its-renaming))

- Editor: Fixed the issue with custom Material GUIs not updating when properties are animated.
    ([UUM-74040](https://issuetracker.unity3d.com/issues/background-color-of-value-b-property-doesnt-change-when-the-preview-mode-is-turned-on-in-the-animation-window))

- Editor: Fixed the label colors of the shortcut help bar buttons.
    (UUM-80313)

- Editor: Removed double ensure frame settings for volumetric clouds.
    (UUM-83033)

- Editor: Restored the F-key functionality and menu items to enable and disable correctly.
    ([UUM-83883](https://issuetracker.unity3d.com/issues/ubuntu-cant-type-the-letter-f))

- Editor: The Linux Editor no longer crashes when creating a prefab variant from the context menu in a read-only directory.
    ([UUM-76157](https://issuetracker.unity3d.com/issues/linux-crash-on-createvariant-when-a-prefab-variant-is-created-in-the-packages-folder))

- Editor: Updated the SG heatmap default values in the Editor.
    ([UUM-76531](https://issuetracker.unity3d.com/issues/shadergraphs-defaultheatmapvalues-asset-does-not-have-hdrp-specific-nodes-added-by-default))

- GI: Fixed seams between adjacent lightmapped terrains.
    ([UUM-82256](https://issuetracker.unity3d.com/issues/light-slash-shadow-information-on-an-edge-of-a-terrain-tile-creates-a-seam-with-an-adjacent-terrain-tile-when-baking-a-lightmap))

- Graphics: Added transient usage flag when creating images even if lazily allocated memory is not available on the devices running Vulkan API.
    ([UUM-71363](https://issuetracker.unity3d.com/issues/android-vulkan-vk-image-usage-transient-attachment-bit-not-added-on-some-android-devices-in-com-dot-unity3d-dot-player-dot-unityplayeractivity-slash-2d-colour-attachement))

- Graphics: Fixed an issue with CommandBuffer warning that appeared when opening the game view.
    ([UUM-74509](https://issuetracker.unity3d.com/issues/urp-commandbuffer-built-in-render-texture-type-3-not-found-while-executing-warning-is-thrown-when-game-view-is-open-and-opengl-is-used))

- Graphics: Fixed `RendererFeature` to render the correct `Texture2DArray` slice for OpenGL.
    (UUM-75624)

- HDRP: Fixed an issue that would cause volumetric shadow clipping issues in some camera angles.
    (UUM-79424)

- HDRP: Fixed uninitalized/unused shader warnings.
    ([UUM-81586](https://issuetracker.unity3d.com/issues/shader-warnings-are-thrown-after-building-high-definition-3d-template))

- HDRP: Fixed `WorldLightManager.Collect` so it no longer has poor performance when a large amount of GameObjects are present in the scene.
    ([UUM-79279](https://issuetracker.unity3d.com/issues/worldlightmanager-dot-collect-has-poor-performance-when-a-large-amount-of-gameobjects-are-present-in-the-scene))

- iOS: Fixed the simulator architecture drop down being disabled in player settings of a custom build profile unless main player settings had simulator selected.
    ([UUM-79676](https://issuetracker.unity3d.com/issues/player-settings-ios-tvos-inactive-simulator-architecture-options-in-custom-player-settings-when-profile-is-not-set-as-active))

- iOS: Fixed Unity launching in background on background app activation.
    (UUM-82451)

- Package Manager: Dependency resolution no longer breaks when there is a dependency on a core package with a different version. Instead, the Package Manager will use the built-in package version. Alternatively, you can preserve the previous behavior and override specific core packages with a version pulled from a custom scoped registry by setting the following scoped registry configuration: `"overrideBuiltIns": true`.

- Package Manager: Fixed the lock icon not showing for some feature set packages.
    (UUM-74838)

- Package Manager: Moved the action buttons to the bottom of the details header.

- Particles: Fixed an issue where there were artifacts while displaying gizmo.
    ([UUM-55691](https://issuetracker.unity3d.com/issues/metal-mesh-gizmos-in-shape-module-produce-visual-artifacts))

- Physics: Fixed an issue where the re-generation of filter data for colliders would discard the vehicle \(if those colliders were part of a vehicle setup\). This issue resulted in the vehicle setup exploding due to the internal wheel queries hitting the colliders.
    (PHYS-379)

- Physics: Fixed an issue where WheelCollider component's raycasts failed to hit colliders due to incorrect filtering data.
    ([UUM-82839](https://issuetracker.unity3d.com/issues/wheel-colliders-fall-into-the-ground-when-changing-parent-rigidbody-attributes-and-the-colliders-are-touching-a-sibling-gameobjects-collider))

- Physics: Fixed an issue with Colliders where they would end up ignoring the value passed into the "Layer Override Priority" when doing so via the Collider component's inspector rather than API.
    ([UUM-83048](https://issuetracker.unity3d.com/issues/layeroverridepriority-is-not-used-inside-filter-data-calculations))

- Physics 2D: Fixed the issue with Rigidbody2D interpolation called jitter when multiple `FixedUpdate` occur back-to-back. This typically occurs when the application target frame-rate is set lower than the `FixedUpdate` rate.
    ([UUM-63810](https://issuetracker.unity3d.com/issues/gameobjects-with-a-rigidbody2d-movement-is-jittery-when-interpolation-is-turned-on))

- Scripting: Fixed a compilation issue when inconsistent settings were applied to  player assemblies compatibility level and editor-only assemblies compatibility level.
    (UUM-78289)

- Shadergraph: Fixed the issue with `NullReferenceException` when updating a legacy node for second time through undo.
    ([UUM-76255](https://issuetracker.unity3d.com/issues/shadergraph-legacy-nodes-in-the-graph-can-result-in-a-nullreferenceexception-when-updating-node))

- Shaders: Fixed a copy/paste issue when right-clicking on the property of a shader created with `TexturePropertySingleLine()`.
    (UUM-78130)

- SpeedTree: Fixed GUI assertion errors specific to the LODGroup array size for the SpeedTree 9 importer.
    (UUM-83192)

- SRP Core: Fixed a crash on DX12 due to invalid subpass flags passed by native render pass compiler.
    ([UUM-82663](https://issuetracker.unity3d.com/issues/crash-on-0x00007ff9d3b9ee3f-nvwgf2umx-openadapter10-when-entering-edit-mode-of-shadergraph-asset))

- TextMeshPro: Fixed the iOS crash that occurred when using fallback fonts created at runtime.
    ([UUM-72139](https://issuetracker.unity3d.com/issues/ios-crash-when-using-fallback-fonts-created-at-runtime))

- UI Toolkit: Fixed an issue where basic UI was not being rendered with RenderGraph \(URP\) on D3D12.
    ([UUM-83173](https://issuetracker.unity3d.com/issues/basic-ui-toolkit-panels-do-not-render-when-using-urp-plus-rendergraph-plus-d3d12))

- UI Toolkit: Fixed exceptions that would occur in the UI Builder when an element had a dataSource that was not compatible with `UnityEngine.Object`.
    ([UUM-82308](https://issuetracker.unity3d.com/issues/argumentexception-is-thrown-when-setting-datasource-to-the-c-number-object-that-doesnt-inherit-from-unityengine-dot-object-in-ui-builder))

- UI Toolkit: Fixed the UIBuilder library tabs styling.
    ([UUM-79485](https://issuetracker.unity3d.com/issues/align-section-button-groups-are-partially-cut-off-in-ui-builder-when-inspector-is-at-default-width))

- UI Toolkit: Removed a race condition when registering UXML description data.
    (UUM-82468)

- Universal RP: Added shader stripping logic for STP to avoid URP project build failures when targeting Windows from a non-Windows platform.
    ([UUM-78665](https://issuetracker.unity3d.com/issues/shader-errors-in-dxc-when-building-for-windows-platform-on-a-macos-machine))

- Universal RP: Removed usage of legacy `depthBufferBits` on `RenderTextureDescriptor` in URP 2D and 3D renderers to fix issues with incorrect depth stencil format for render textures.
    (UUM-83481)

- Universal RP: Updated RenderGraph samples \(install through Package Manager\) to the latest APIs and best practices.
    (UUM-82962)

- URP: Fixed compile error in the lighting debug views when using APV with Shadowmask.
    (UUM-82976)

- URP: Fixed missing geometry on Adreno GPUs by disabling GPU occlusion culling as a workaround.
    (UUM-82677)

- URP: Fixed TAA frame index mismatch which was causing incorrect visuals when the camera history reset system was used with STP.
    (UUM-83305)

- URP: Fixed the depth bias for motion vectors that was causing objects to leak through geometry.
    ([UUM-63692](https://issuetracker.unity3d.com/issues/motion-vectors-bleed-through-any-geometry-when-using-urp-temporal-anti-aliasing))

- Version Control: Fixed a token renewal issue: Can't obtain a new token \(Message: Invalid Refresh Token., Code: 132.104\).

- VFX Graph: Improved Water integration to prevent an unexpected error from dispatch.
    (UUM-79643)

- Web: Fixed an issue that prevented use of `unityInstance.SendMessage` right after `createUnityInstance` resolved.
    ([UUM-78675](https://issuetracker.unity3d.com/issues/unityinstance-dot-sendmessage-does-not-work-in-webgl-build-when-called-inside-createunityinstance))

- Web: Fixed errors that were caused by memory exceeding 2GB in WebGPU.

- Web: Fixed the URP 2D skinned sprites with shadows.




## Package changes in 6000.0.23f1

## Packages updated

- com.unity.collections: [2.4.3](https://docs.unity3d.com/Packages/com.unity.collections@2.4//changelog/CHANGELOG.html) to [2.5.1](https://docs.unity3d.com/Packages/com.unity.collections@2.5//changelog/CHANGELOG.html)

- com.unity.entities: [1.2.4](https://docs.unity3d.com/Packages/com.unity.entities@1.2//changelog/CHANGELOG.html) to [1.3.2](https://docs.unity3d.com/Packages/com.unity.entities@1.3//changelog/CHANGELOG.html)

- com.unity.netcode: [1.2.4](https://docs.unity3d.com/Packages/com.unity.netcode@1.2//changelog/CHANGELOG.html) to [1.3.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.3//changelog/CHANGELOG.html)

- com.unity.physics: [1.2.4](https://docs.unity3d.com/Packages/com.unity.physics@1.2//changelog/CHANGELOG.html) to [1.3.2](https://docs.unity3d.com/Packages/com.unity.physics@1.3//changelog/CHANGELOG.html)

- com.havok.physics: 1.2.4 to 1.3.2

- com.unity.logging: [1.2.4](https://docs.unity3d.com/Packages/com.unity.logging@1.2//changelog/CHANGELOG.html) to [1.3.2](https://docs.unity3d.com/Packages/com.unity.logging@1.3//changelog/CHANGELOG.html)

- com.unity.entities.graphics: [1.2.4](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.2//changelog/CHANGELOG.html) to [1.3.2](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.3//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.5.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.5//changelog/CHANGELOG.html) to [2.5.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.5//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.11.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.11//changelog/CHANGELOG.html) to [1.11.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.11//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.2.6](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html) to [1.2.7](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.4.1](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.4//changelog/CHANGELOG.html) to [1.5.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.5//changelog/CHANGELOG.html)

- com.unity.sequences: [2.1.2](https://docs.unity3d.com/Packages/com.unity.sequences@2.1//changelog/CHANGELOG.html) to [2.1.3](https://docs.unity3d.com/Packages/com.unity.sequences@2.1//changelog/CHANGELOG.html)

- com.unity.multiplayer.playmode: [1.2.2](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.3//changelog/CHANGELOG.html)

- com.unity.dedicated-server: [1.2.2](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.3//changelog/CHANGELOG.html)

- com.unity.memoryprofiler: [1.1.0](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.1](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- com.unity.multiplayer.tools: [2.1.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.1//changelog/CHANGELOG.html) to [2.2.1](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.charactercontroller@1.2.4](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.2//changelog/CHANGELOG.html)

- [com.unity.polyspatial@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial@2.0//changelog/CHANGELOG.html)

- [com.unity.polyspatial.visionos@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@2.0//changelog/CHANGELOG.html)

- [com.unity.polyspatial.xr@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@2.0//changelog/CHANGELOG.html)

- [com.unity.polyspatial.extensions@2.0.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@2.0//changelog/CHANGELOG.html)

- [com.unity.xr.visionos@2.0.4](https://docs.unity3d.com/Packages/com.unity.xr.visionos@2.0//changelog/CHANGELOG.html)

- [com.unity.ext.flatsharp@1.1.1](https://docs.unity3d.com/Packages/com.unity.ext.flatsharp@1.1//changelog/CHANGELOG.html)

- [com.unity.services.multiplayer@1.0.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@1.0//changelog/CHANGELOG.html)

- [com.unity.multiplayer.widgets@1.0.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.widgets@1.0//changelog/CHANGELOG.html)