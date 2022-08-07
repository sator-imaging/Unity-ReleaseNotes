# Unity 2023.1.0 Alpha 4
https://unity3d.com/unity/alpha/2023.1.0a4

## Preview of Final 2023.1.0a4 Release Notes


### Features
<ul>
<li><p>Editor: Added 'focusedWindowChanged' callback to EditorWindow class.</p></li>
<li><p>Editor: Added Helper Bar that shows useful shortcuts.</p></li>
<li><p>Editor: Added optional priority argument to Shortcut and ClutchShortcut attributes.</p></li>
<li><p>Graphics: Added new RayTracingAccelerationStructure.AddInstance signature that allows adding Mesh instances into the acceleration structure for GPU ray tracing. This is the equivalent of Graphics.RenderMesh from rasterization pipeline.</p></li>
<li><p>HDRP: Added Ray Tracing Terrain support for HDRP.</p></li>
<li><p>Terrain: Added Quality Settings for being able to control various Terrain settings at different quality levels.</p></li>
<li><p>UI Toolkit: Added Vertex Buffer size configuration.</p></li>
<li><p>URP: Added RenderGraph support to URP postFX.</p></li>
<li><p>URP: SSAO: AO Method dropdown added to select between Interleaved Gradient Noise and Blue Noise.</p></li>
<li><p>URP: SSAO: Blur Quality dropdown added to select between: High (Bilateral), Medium (Gaussian) and Low (Single-Pass Kawase).</p></li>
<li><p>URP: SSAO: Falloff field added to control the distance from the camera the AO should affect.</p></li>
<li><p>Version Control: Added changelist related options to pending changes context menu.</p></li>
<li><p>Version Control: Added option to enable changelists and display them in pending changes tab.</p></li>
</ul>

### Improvements
<ul>
<li><p>Build Pipeline: Improved error handling for builds to show less redundant error messages.</p></li>
<li><p>Burst: Used explicit namespace for UnityEditor.PackageManager.Events to avoid conflicts.</p></li>
<li><p>Documentation: Removed legacy command line argument 'vrmode' from documentation.</p></li>
<li><p>DX12: Improved visuals by setting swapchain background color to make resize more pleasing and disable scaling in resize. (UUM-2444)</p></li>
<li><p>DX12: Optimize D3D12 sampler access by removing unnecessary locking and map finds.</p></li>
<li><p>Editor: Improved layout of Quality settings table, to avoid cropping of the labels.</p></li>
<li><p>GI: Improved error messages when exceeding max allocation size for transmission texture when baking with the GPU lightmapper.</p></li>
<li><p>GI: Made minor refactorings which pave the road for new and improved features.</p></li>
<li><p>Graphics: Avoid redundant render target attachment stores for read-only attachments when using Vulkan.</p></li>
<li><p>HDRP: Changed ACES luminance fit to allow pure whites.</p></li>
<li><p>HDRP: Enabled multi-editing for Diffusion Profiles.</p></li>
<li><p>HDRP: Improved rendering by adding caustics support for cinematic eye shader in HDRP material samples eye graph.</p></li>
<li><p>HDRP: New iteration on the water system.</p></li>
<li><p>HDRP: Removed diffusion profiles from global settings.</p></li>
<li><p>HDRP: Tooltips improvement.</p></li>
<li><p>Physics: Added a field in the PhysicsManager inspector that exposes the number of 16kb chunks used by PhysX's temporary scratch buffer, the default number of chunks is 4 with a total of 64kb of memory allocated. The scratch buffer size can be seen inside the memory profiler as an allocation root.</p></li>
<li><p>Physics: Added a temporary scratch buffer to the Physics simulation, in order to improve performance by avoiding going to the main allocator for small temporary allocations.</p></li>
<li><p>Serialization: Improved performance for cases where endianness needs to be swapped during (de)serialization.</p></li>
<li><p>SRP Core: Tooltips improvement across SRPs.</p></li>
<li><p>URP: Downsampling will now not only affect the AO pass but also the blur passes.</p></li>
<li><p>URP: Improved Depth test to avoid incorrectly adding AO in places where two objects are far away from one another.</p></li>
<li><p>URP: Tooltips improvement.</p></li>
<li><p>XR: Improved GLES3 multiview rendering performance. (1374693)</p></li>
</ul>

### API Changes
<ul>
<li><p>Android: Obsoleted: PlayerSettings.Android.minifyWithR8 is obsolete now. Setting it has no effect and it always returns true.</p></li>
<li><p>Core: Added: A new event Application.memoryUsageChanged, that is fired when applications memory usage changes significantly (for example goes critically low).</p></li>
<li><p>Editor: Obsoleted: PlayerSettings API using BuildTargetGroup is now obsolete, use it with NamedBuildTarget instead.</p></li>
<li><p>Graphics: Added: Introduces Native Renderpass API on CommandBuffer.</p></li>
<li><p>Graphics: Added: Material.GetBufferHandle to get the GraphicsBufferHandle in a material property sheet.</p></li>
<li><p>Graphics: Added: Material.GetPropertyNames(&lt;PropertyType&gt;) to query the property sheet names in a material based on a given property type.</p></li>
<li><p>Graphics: Added: New Foveated Rendering API on the command buffer interface.</p></li>
<li><p>Graphics: Added: New overload for CommandBuffer.SetComputeBufferParam, which allows binding a resource with GraphicsBufferHandle.</p></li>
<li><p>Graphics: Added: RenderPipeline.IsRenderRequestSupported. Protected method, render pipelines can override this to specify their support for RequestData types.</p></li>
<li><p>Graphics: Added: RenderPipeline.ProcessRenderRequest. Protected method, render pipelines can override this to implement the rendering logic for RenderRequests.</p></li>
<li><p>Graphics: Added: RenderPipeline.StandardRequest. Use this as the RequestData parameter in SubmitRenderRequest to trigger a default srp render on the specified camera.</p></li>
<li><p>Graphics: Added: RenderPipeline.SubmitRenderRequest. Triggers a render with the active render pipeline according to the passed in RequestData.</p></li>
<li><p>Graphics: Added: RenderPipeline.SupportsRenderRequest. Checks the active pipeline whether the given RequestData type is supported.</p></li>
<li><p>Graphics: Deprecated: Deprecation of the various DrawX functions on the ScriptableRenderContext in favor of the RendererList API.</p></li>
<li><p>SRP Core: Added: An extension method to fetch the Render Pipeline assets from a BuildTarget.</p></li>
<li><p>UI Toolkit: Added: Added the necessary Experimental APIs to interact with subsections of the Text. (UUM-4313)</p></li>
<li><p>Universal: Added: UniversalRenderPipeline.SingleCameraRequest. Use this as the RequestData parameter in SubmitRenderRequest to render a single camera.</p></li>
<li><p>Universal: Obsoleted: RenderSingleCamera is now obsolete. Please use RenderPipeline.SubmitRenderRequest with RequestData of the SingleCameraRequest type.<br> Graphics: Camera.SubmitRenderRequests is now obsolete. Please use RenderPipeline.SubmitRenderRequest with RequestData of a supported type such as RenderPipeline.StandardRequest.</p></li>
<li><p>URP: Added: Added light cookies stripping.</p></li>
</ul>

### Changes
<ul>
<li><p>Android: Android SDK must have cmdline-tools component installed now. Unity will ignore tools component.</p></li>
<li><p>Android: Default gradle templates have changed significantly with new Gradle and AGP versions. Gradle templates in existing projects will have to be recreated based on new default templates when upgrading projects created with previous Unity versions.</p></li>
<li><p>Android: JDK 11 is required now to build Android apps.</p></li>
<li><p>Android: Removed editor UI option which allowed to choose between R8 and Proguard tools to minify code. New AGP version doesn't have an option to minify using proguard. Instead R8 is always used.</p></li>
<li><p>Android: Unity Now uses Android Gradle Plugin 7.1.2 by default.</p></li>
<li><p>Android: Unity Now uses Gradle 7.2 by default.</p></li>
<li><p>Apple TV: Changed the minimum supported OS version to tvOS13.</p></li>
<li><p>HDRP: Changed DiffusionProfileOverride so that now it accumulates profiles instead of replacing when interpolating at runtime.</p></li>
<li><p>iOS: Changed the minimum supported OS version to iOS13.</p></li>
<li><p>UI Toolkit: ColorField is now UI Toolkit based and does not rely on an IMGUIContainer.</p></li>
<li><p>URP: Changed light and decal layers to rendering layers.</p></li>
<li><p>URP: Changed the samples field to a dropdown: High (12 samples), Medium (8 samples) and Low (4 samples).</p></li>
<li><p>URP: Changed the the final After Opaque passes to be merged with the last blur pass.</p></li>
<li><p>URP: Foveated Rendering is now integrated in URP for supported platforms.</p></li>
</ul>

### Fixes
<ul>
<li><p>2D: Fixed an asset previews Tilemap Prefabs not being generated due to Grid Components being stripped away during this process. (<a href="https://issuetracker.unity3d.com/issues/tile-palette-prefab-preview-does-not-show-the-correct-image">UUM-2503</a>)</p></li>
<li><p>2D: Fixed an issue where Fill and Erase extents were not added to user preferences when showing a Flood Fill preview while painting with Tilemaps.</p></li>
<li><p>2D: Fixed case where Sprite Atlas shows only first page in Preview within Inspector. (<a href="https://issuetracker.unity3d.com/issues/sprite-atlas-shows-only-first-page-in-preview-within-inspector">1427632</a>)</p></li>
<li><p>2D: Fixed duplicate instantiated GameObjects from Tiles on Tilemap Prefabs when instantiating the Tilemap Prefabs. (<a href="https://issuetracker.unity3d.com/issues/instantiating-tilemap-that-has-rule-tile-with-default-gameobject-set-creates-extra-copy-of-gameobject-at-00-0-in-builds-1">UUM-1671</a>)</p></li>
<li><p>Android: Fix Screen.safeArea calculations (UUM-3972)</p></li>
<li><p>Android: Fixed a performance issue caused by redundant depth/stencil stores on some Adreno OpenGL ES drivers. (1429210)</p></li>
<li><p>Android: Fixed an issue where executing Android SDK tool command would fail with missing java error. For ex., "Unable to locate a Java Runtime". Even though everything is set correctly in Preferences-&gt;External Tools-&gt;JDK. Also during the failure, Unity will now print environment variables thus helping identifying such issues in the future. (UUM-2106)</p></li>
<li><p>Android: Fixed an overhead of memory allocations in the Vulkan backend issue for allocation sizes between 128kB and 1024kB. (UUM-5966)</p></li>
<li><p>Android: Fixed crash during low memory kill. (1423456)</p></li>
<li><p>Android: Fixed crash when creating pipeline objects for some URP Lit shader on some older Adreno drivers. (<a href="https://issuetracker.unity3d.com/issues/android-vulkan-player-crashes-during-shader-warmup-when-using-vulkan-api">UUM-3650</a>)</p></li>
<li><p>Android: Fixed Patch (/And Run) failing on some Android 12 devices with "Permission Denied" or "No such file or directory". (<a href="https://issuetracker.unity3d.com/issues/android-incremental-build-pipeline-failed-to-deploy-application-to-device-errors-is-thrown-when-trying-to-patch-pixel-devices">1422895</a>)</p></li>
<li><p>Android: Fixed regression where TouchScreenKeyboard.Open() was not opening. (<a href="https://issuetracker.unity3d.com/issues/tmp-android-keyboard-doesnt-show-up-when-touchscreenkeyboard-dot-open-function-is-called-on-an-android-device">UUM-2112</a>)</p></li>
<li><p>Asset Import: Fixed out of bounds exception on empty array access when importing SpeedTree billboards with no mesh data. (<a href="https://issuetracker.unity3d.com/issues/speedtreeimporter-asserts-when-mesh-is-empty-on-debug-editor">1428865</a>)</p></li>
<li><p>Audio: Fixed an issue where Audio Clip Import Settings were not getting saved when the "Override for Dedicated Server" setting was enabled. (<a href="https://issuetracker.unity3d.com/issues/audio-clip-import-settings-do-not-get-saved-when-the-override-for-dedicated-server-setting-is-enabled">UUM-399</a>)</p></li>
<li><p>Audio: Fixed audio mixer groups not visible from the packages. (<a href="https://issuetracker.unity3d.com/issues/audio-mixer-groups-are-not-displayed-in-object-picker-when-located-in-a-package">UUM-369</a>)</p></li>
<li><p>Build Pipeline: Fixed an issue where clean builds did not remember state about the built files, thus files in a build could not be deleted in subsequent builds.</p></li>
<li><p>Build System: Fixed an issue where thes splashscreen logo could not be removed when it was included in a previous build. (<a href="https://issuetracker.unity3d.com/issues/unity-default-resources-contains-unitysplash-cube-when-the-splash-screen-disabled">1400086</a>)</p></li>
<li><p>Burst: Fixed an issue that whitespace changes in ILPP'd assemblies would not be detected.</p></li>
<li><p>Burst: Fixed some ARM branch instructions not being processed as such.</p></li>
<li><p>Core: Fixed Asset import workers to not inherit open handles from the main editor causing trouble rebinding network sockets. (1418567)</p></li>
<li><p>DX12: Fixed to Allow releasing memory with GL.Flush() within a single frame. (<a href="https://issuetracker.unity3d.com/issues/camera-dot-render-causes-a-memory-leak-in-hdrp-using-directx-12">1400617</a>)</p></li>
<li><p>Editor: -Fixed [UIToolkit] Reorderables reset array count to 0 when multi selecting objects that have arrays with more than 64 elements. (1417862)</p></li>
<li><p>Editor: Fixed a crash when loading TIFFs with bad thumbnail tags. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-freeimage-makethumbnail-after-importing-tif-file">UUM-3783</a>)</p></li>
<li><p>Editor: Fixed a crash when there was a corrupt PrefabInstance. (<a href="https://issuetracker.unity3d.com/issues/crash-on-awakefromloadqueue-checkgameobjectandcomponentstructure-when-loading-a-scene-manually">UUM-1926</a>)</p></li>
<li><p>Editor: Fixed an  issue with Windows Standalone play started on the wrong screen. (<a href="https://issuetracker.unity3d.com/issues/build-is-launched-in-the-wrong-display-when-main-display-is-changed">1423262</a>)</p></li>
<li><p>Editor: Fixed an issue that warning messages are no longer displayed when selecting the color picker after selecting the object picker when editing materials. (<a href="https://issuetracker.unity3d.com/issues/propertiesgui-is-being-called-recursively-warning-produced-when-trying-to-open-color-picker-when-object-picker-is-opened">UUM-647</a>)</p></li>
<li><p>Editor: Fixed an issue where FBX files with custom property animations where considered as not having animation data at all. (1427122)</p></li>
<li><p>Editor: Fixed an issue where GameObjectChangeTracker was not able to detect GameObject sibling order change.</p></li>
<li><p>Editor: Fixed an issue where LODGroup editor was not updating immediately when there were changes. (<a href="https://issuetracker.unity3d.com/issues/lods-array-is-not-updated-instantly-when-inserting-new-lods">UUM-5815</a>)</p></li>
<li><p>Editor: Fixed an issue where ObjectField failed to continue to process ObjectSelector events when it was not in focused. (<a href="https://issuetracker.unity3d.com/issues/object-cannot-be-picked-from-the-object-picker-when-calling-unityengine-dot-gui-dot-focuscontrol-null-in-custom-editor-gui">1415249</a>)</p></li>
<li><p>Editor: Fixed an issue where the New launch screen did not bring notification dialogs to front. (UUM-6395)</p></li>
<li><p>Editor: Fixed an issue where there was a missing Edit button for Light Probe UI. (<a href="https://issuetracker.unity3d.com/issues/edit-light-probes-button-in-light-probe-group-component-is-squished">UUM-919</a>)</p></li>
<li><p>Editor: Fixed CharacterController component colliding with multiple Trigger colliders stacked in a small space. (<a href="https://issuetracker.unity3d.com/issues/charactercontroller-collider-stops-working-when-multiple-gameobjects-with-colliders-are-near-it">1419316</a>)</p></li>
<li><p>Editor: Fixed crash when opening scenes in builds that had missing Prefab sources. (<a href="https://issuetracker.unity3d.com/issues/crash-on-build-when-running-the-build-with-missing-prefabs">UUM-2546</a>)</p></li>
<li><p>Editor: Fixed Folders with the already existing name are moved properly. (<a href="https://issuetracker.unity3d.com/issues/moving-subfolder-to-a-folder-which-contains-another-subfolder-with-the-same-name-copies-original-folders-content">1389121</a>)</p></li>
<li><p>Editor: Fixed InvalidOperationException when closing OpenFolderPanel. (<a href="https://issuetracker.unity3d.com/issues/windows-invalidoperationexception-stack-empty-when-using-editorutility-dot-openfilepanel-or-editorutility-dot-openfolderpanel">1394298</a>)</p></li>
<li><p>Editor: Fixed not being able to summon context menu issue when SceneView was active. (1423212)</p></li>
<li><p>Editor: Fixed performance issue for looping small clip with root motion extraction. (<a href="https://issuetracker.unity3d.com/issues/performance-cost-of-looping-animations-increases-over-time">1428866</a>)</p></li>
<li><p>Editor: Fixed UI error when using graphics volume context menu. (UUM-3911)</p></li>
<li><p>EmbeddedLinux: Fixed Query EGL to get the correct max supported VSync value.</p></li>
<li><p>GI: -Fixed [GPU PLM] OpenCL shader loading time in new projects has become significantly slower. Fixed regression by speeding up OpenCL shader loading stage by caching binaries in the GICache. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-opencl-shader-loading-time-in-the-new-projects-has-become-significantly-slower-1">UUM-1350</a>)</p></li>
<li><p>GI: Changed GPU lightmapper device selection from emitting a Warning to emitting a Log message to not confuse users when requirements are not met.</p></li>
<li><p>GI: Fixed baking stall occuring when baking terrain with holes. (<a href="https://issuetracker.unity3d.com/issues/plm-baking-stalls-with-terrains-containing-lots-of-holes">1408533</a>)</p></li>
<li><p>GI: Fixed regression introduced by fix for baked probes that were sometimes black. The regression caused a crash during a bake on MacOS. (<a href="https://issuetracker.unity3d.com/issues/macos-gpu-plm-crash-in-openclrenderlightprobebuffers-after-pressing-generate-lighting-button">UUM-1207</a>)</p></li>
<li><p>Graphics: Fixed an issue in RayTracingAccelerationStructure.CullInstances when SkinnedMeshRenderers and CPU Skinning are used, preventing skinned geometries to be added into the acceleration structure. (<a href="https://issuetracker.unity3d.com/issues/skinned-mesh-renderer-is-absent-in-raytracing-acceleration-structure">UUM-4798</a>)</p></li>
<li><p>Graphics: Fixed an issue that SkinnedMeshRenderer and MeshRenderer are now in the same SRP Batch during shadow pass. (<a href="https://issuetracker.unity3d.com/issues/draw-calls-that-batch-in-opaque-pass-do-not-batch-in-shadow-pass-when-some-of-the-draw-calls-come-from-skinnedmeshrenderer-and-some-come-from-meshrenderer">UUM-4336</a>)</p></li>
<li><p>Graphics: Fixed an issue where 2D Textures with multiple faces or images did correctly update their hash values when any face/image was changed and not just the first one. (<a href="https://issuetracker.unity3d.com/issues/cubemap-hash-value-changes-only-when-modifying-the-first-face">UUM-2506</a>)</p></li>
<li><p>Graphics: Fixed an issue where Crunched textures appeared too bright in projects in linear color space. (<a href="https://issuetracker.unity3d.com/issues/crunched-asset-bundle-sprites-are-too-bright-when-loaded-from-file-in-play-mode">UUM-3200</a>)</p></li>
<li><p>Graphics: Fixed an issue where Mesh.GetBlendShapeBuffer would cause stalls when called with PerVertex layout.</p></li>
<li><p>Graphics: Fixed code generation for signed bitfieldExtract for OpenGL ES 3 shaders. (UUM-476)</p></li>
<li><p>Graphics: Fixed crash in ScriptableBatchRenderer::ApplyShaderPass when switching between URP and HDRP.</p></li>
<li><p>Graphics: Fixed Graphics.CopyBuffer and GetData/SetData for non-compute targets when using Vulkan. (UUM-3674)</p></li>
<li><p>HDRP: Added async compute support doc. (UUM-6183)</p></li>
<li><p>HDRP: Added missing using statements in one of the example scripts in the documentation for the accumulation API. (UUM-3224)</p></li>
<li><p>HDRP: Disabled Volumetric Clouds for Default Sky Volumes. (UUM-6185)</p></li>
<li><p>HDRP: Fixed a discrepency between recursive rendering and path tracing for refraction models. (<a href="https://issuetracker.unity3d.com/issues/hdrp-recursive-rendering-refraction-is-very-different-compared-to-rasterization-slash-pathtracing">UUM-6179</a>)</p></li>
<li><p>HDRP: Fixed a NullReferenceException when importing empty material.</p></li>
<li><p>HDRP: Fixed a render graph error when rendering a scene with no opaque objects in forward. (<a href="https://issuetracker.unity3d.com/issues/transparent-custom-pass-renders-opaque-with-msaa-disabled-in-player">UUM-6189</a>)</p></li>
<li><p>HDRP: Fixed a rounding issue in ray traced reflections at half resolution. (UUM-6177)</p></li>
<li><p>HDRP: Fixed an issue that Data Driven Lens Flare are not occluded with the volumetric clouds. (1421739)</p></li>
<li><p>HDRP: Fixed an issue where Shadow near plane could not be set to 0,  and clamped to 0.01 can only occur on Cone, Pyramid and Point Lights.</p></li>
<li><p>HDRP: Fixed an issue where the HDRP Wizzard showed up when opening the Standalone Profiler.</p></li>
<li><p>HDRP: Fixed an issue with DOTS and Look Dev tool causing entities in the tool to be drawn in the game view. (<a href="https://issuetracker.unity3d.com/issues/prefabs-using-hybrid-convert-to-entity-component-are-visible-in-the-game-view-if-used-in-hdrp-look-dev-when-entering-play-mode">UUM-6188</a>)</p></li>
<li><p>HDRP: Fixed artifacts on PBR DOF camera cuts such as the COC sticking around with blurry values. (UUM-6187)</p></li>
<li><p>HDRP: Fixed artifacts on quarter and half res depth of field when dynamic resolution jumps between resolutions. (UUM-6184)</p></li>
<li><p>HDRP: Fixed blending artifacts with physically based DoF. (1375978)</p></li>
<li><p>HDRP: Fixed blinking Ray traced reflection with dynamic resolution. (UUM-6180)</p></li>
<li><p>HDRP: Fixed blinking SSGI with dynamic resolution. (<a href="https://issuetracker.unity3d.com/issues/dynamic-resolution-scaling-blinking-ssgi">UUM-6181</a>)</p></li>
<li><p>HDRP: Fixed cull mode toggle in transparent material inspector shifting the UI. (UUM-6186)</p></li>
<li><p>HDRP: Fixed Decal Layer Texture lifetime in rendergraph. (<a href="https://issuetracker.unity3d.com/issues/decal-layer-texture-lifetime-in-rendergraph-1">UUM-6664</a>)</p></li>
<li><p>HDRP: Fixed duplicated code sample in the custom pass documentation. (<a href="https://issuetracker.unity3d.com/issues/hdrp-sample-code-for-custom-pass-scripting-is-incorrect">UUM-6173</a>)</p></li>
<li><p>HDRP: Fixed grey out profile list button instead of throwing error. (UUM-6174)</p></li>
<li><p>HDRP: Fixed incorrect distortion when hardware DRS is enabled. (<a href="https://issuetracker.unity3d.com/issues/hdrp-camera-view-is-rendered-on-objects-with-a-distortion-blur-material-when-dynamic-resolution-is-enabled">UUM-3322</a>)</p></li>
<li><p>HDRP: Fixed incorrect false positives in shadow culling. (UUM-1294)</p></li>
<li><p>HDRP: Fixed isssue with up direction of the light anchor tool sometime getting wrong. (<a href="https://issuetracker.unity3d.com/issues/hdrp-switching-back-and-forth-the-up-direction-f-the-light-anchor-when-the-elevation-is-a-multiple-of-90-looses-the-settings">UUM-6190</a>)</p></li>
<li><p>HDRP: Fixed leaks in ray tracing effects due to missing ambient probe for ray tracing effects. (UUM-589)</p></li>
<li><p>HDRP: Fixed motion vector debug visualization suite to provide a way to visualize intensities. (1430303)</p></li>
<li><p>HDRP: Fixed quad artifacts on TAA and fixed an issue on bicubic filtering. (<a href="https://issuetracker.unity3d.com/issues/taa-quad-like-artifacts-around-moving-silhouettes">UUM-6205</a>)</p></li>
<li><p>HDRP: Fixed re-ordering issue in the custom pass list. (<a href="https://issuetracker.unity3d.com/issues/reordering-custom-passes-not-working">UUM-6176</a>)</p></li>
<li><p>HDRP: Fixed reflection issue upon scene filtering. (UUM-6514)</p></li>
<li><p>HDRP: Fixed specular occlusion fallback on normal when bent normal is not available. (<a href="https://issuetracker.unity3d.com/issues/bent-normals-and-shadergraph-1">UUM-6662</a>)</p></li>
<li><p>HDRP: Fixed SSGI using garbage outside the frustum. (UUM-6175)</p></li>
<li><p>HDRP: Fixed the clamp happening on the sum of ray tracing samples instead of per sample. (<a href="https://issuetracker.unity3d.com/issues/clamping-is-behaving-wrong-for-quality-ray-tracing-global-illumination">UUM-6513</a>)</p></li>
<li><p>HDRP: Fixed the default DXR volume not having any DXR effects enabled. (UUM-6182)</p></li>
<li><p>HDRP: Fixed tiling artifacts with physically based DoF. (<a href="https://issuetracker.unity3d.com/issues/rendering-artifacts-are-produced-when-physically-based-option-is-enabled-on-depth-of-field-volume-override">1413534</a>)</p></li>
<li><p>HDRP: Fixed Virtual texturing streaming loading to be no longer hindered by transparent materials. Transparent materials, depending on their transmitance or alpha, will let the VT streaming system requests textures appropiately. (1423890)</p></li>
<li><p>HDRP: Fixed [HDRP] Noisy top shadows when using 'High' Filtering Quality with Tesselated Meshes (Lit Tesselation). (<a href="https://issuetracker.unity3d.com/issues/hdrp-noisy-top-shadows-when-using-high-filtering-quality-with-tesselated-meshes-lit-tesselation">UUM-3341</a>)</p></li>
<li><p>HDRP: Updated misleading tooltip in the environment lighting in HDRP. (UUM-6178)</p></li>
<li><p>IL2CPP: Fixed  crash when a Unity player is unloaded and reloaded. (<a href="https://issuetracker.unity3d.com/issues/use-after-free-crash-bug-in-il2cpp">UUM-2660</a>)</p></li>
<li><p>IL2CPP: Fixed a crash in il2cpp memory allocator. (UUM-4708)</p></li>
<li><p>IL2CPP: Fixed Cache shared code used by il2cpp between projects for faster initial compiles.</p></li>
<li><p>IL2CPP: Fixed leak of internal thread objects that could manifest in a pause on player exit (<a href="https://issuetracker.unity3d.com/issues/il2cpp-player-hangs-for-20-seconds-after-closing-it-when-running-threads">UUM-607</a>)</p></li>
<li><p>IL2CPP: Fixed performance issues in metadata access with thread contention. (UUM-609)</p></li>
<li><p>IL2CPP: Fixed performance regression in regular expressions. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-regex-perfomance-regression-when-using-il2cpp-scripting-backend">UUM-590</a>)</p></li>
<li><p>IL2CPP: Updated zlib to version 1.2.12 for CVE-2018-25032. (UUM-599)</p></li>
<li><p>iOS: Fixed a forcing jobified metal rendering issue where it was disregarding player settings. (UUM-7195)</p></li>
<li><p>Linux: Fixed Aux drop down window will close when it's main container window is closed. (<a href="https://issuetracker.unity3d.com/issues/linux-profiler-profiling-mode-dropdown-remains-open-after-closing-the-profiler-window">UUM-1574</a>)</p></li>
<li><p>Linux: Fixed nullpointer exception for rapidly open and close selection icon dropdown. (<a href="https://issuetracker.unity3d.com/issues/linux-select-icon-dropdown-throws-missingreferenceexception-errors-when-being-rapidly-opened-and-closed">UUM-1572</a>)</p></li>
<li><p>Linux: Fixed print stack trace frequently crashing. (UUM-1595)</p></li>
<li><p>macOS: Fixed  the issue of the appearance of multiple "Unsaved Changes Detected" reports. (<a href="https://issuetracker.unity3d.com/issues/multiple-unsaved-changed-detected-reports-appear-when-zooming-with-the-touchpad-after-not-saving-the-shader-graph">1369562</a>)</p></li>
<li><p>macOS: Fixed an issue with exposing profiler markers in non-development players. (<a href="https://issuetracker.unity3d.com/issues/externalgraphicsprofiler-dot-h-exposes-392-profiler-markers-to-release-players-without-kavailabilitynondevelopment-flag-set">UUM-2990</a>)</p></li>
<li><p>Mono: Fixed a crash during stack trace construction if a this object is null. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-invoking-delegate-with-null-argument">UUM-611</a>)</p></li>
<li><p>Package: Fixed errors when inspecting tutorial pages on Unity 2021 or later.</p></li>
<li><p>Package Manager: Fixed an issue where Package Manager Window would throw an error when a package url links was not available and now are disabled.</p></li>
<li><p>Package Manager: Fixed Package Tag text in details header is not visible. (<a href="https://issuetracker.unity3d.com/issues/packman-local-preview-slash-experimental-packages-have-only-a-tag-outline-displayed-in-packman-when-added-from-disk-or-tarball">1420347</a>)</p></li>
<li><p>Package Manager: Updated package count in "My Assets" when current number of packages is larger than total number. (1431169)</p></li>
<li><p>Physics: Fixed an issue where rotating a GameObject hierarchy with a Rigidbody at it's root, would recompute the body's mass properties for each child collider present in the hierarchy. (<a href="https://issuetracker.unity3d.com/issues/time-spent-in-physics-dot-synccollidertransforms-for-dynamic-rigidbodies-scales-exponentially-with-collider-count">1318791</a>)</p></li>
<li><p>Physics: Fixed Articulation Bodies accepting drives with non-finite values as input. (<a href="https://issuetracker.unity3d.com/issues/articulation-body-drives-teleport-the-whole-chain-to-nan-coordinates-when-given-nan-input">1429317</a>)</p></li>
<li><p>Physics: Improved and jobified Physics.SyncTransforms in order to providing up to 70% speed up in general.</p></li>
<li><p>Prefabs: Fixed Events prefabInstanceReverting and prefabInstanceReverted which are now automatically raised upon any revert operation, whether full or partial. (1409546)</p></li>
<li><p>Prefabs: Fixed Handle ManagedReferences that cannot be applied or reverted. Also made sure the root of the Managed Reference can be applied to apply sub fields that are overriden. (<a href="https://issuetracker.unity3d.com/issues/applysingleproperty-copy-state-error-when-applying-overrides-to-a-prefab-with-serialized-references">1409175</a>)</p></li>
<li><p>Profiler: Fixed an issue that taking a memory capture no longer logs a message to the console displaying the temporary file location.</p></li>
<li><p>Scene/Game View: Fixed an issue where gizmos with bounds near the camera were incorrectly culled. (1429779)</p></li>
<li><p>Scene/Game View: Fixed case where Overlays placed partially outside of a view would reset their position. (1422226)</p></li>
<li><p>Scene/Game View: Fixed Overlay popups not clipping to window size. (1419903)</p></li>
<li><p>Scripting: Fixed a validate assemblies issue after build target was changed. (UUM-3562)</p></li>
<li><p>Scripting: Fixed an issue where Application.logMessageReceived can be called from a job, when the job is scheduled on the main thread. (<a href="https://issuetracker.unity3d.com/issues/application-dot-logmessagereceived-is-called-from-worker-thread-when-logging-errors-from-bursted-ijob">UUM-3085</a>)</p></li>
<li><p>Scripting: Fixed Assemblies without any class or structs produces warnings. (<a href="https://issuetracker.unity3d.com/issues/internal-errors-show-up-when-theres-an-assembly-definition-asset-an-empty-script-asset-attached-to-it-and-the-suppress-common-warnings-option-is-disabled">UUM-4342</a>)</p></li>
<li><p>Scripting: Fixed broken performance test. (UUM-3563)</p></li>
<li><p>Scripting: Fixed Disabled Plugin Assembly validation not working on startup. (UUM-4560)</p></li>
<li><p>Scripting: Improved diagnostic message and do not enter in safe-mode on some unsupported ApiUpdater scenarios involving .asmref adding code into .asmdef. (1406100)</p></li>
<li><p>Serialization: Avoid crash and log error message when boxedValue is set to null for non nullable property types. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-serializedproperty-dot-boxedvalue-is-set-to-null">UUM-658</a>)</p></li>
<li><p>Serialization: Fixed Issue when performing an undo on an object that uses SerializeReference reuse existing C# objects, instead of recreating them. (<a href="https://issuetracker.unity3d.com/issues/serialized-references-are-recreated-when-modifiying-any-field-and-then-doing-ctrl-plus-z">UUM-651</a>)</p></li>
<li><p>Shadergraph: Fixed a compilation bug in BiRP Target in some variants with lightmaps. (UUM-7354)</p></li>
<li><p>Shaders: Changed texture declaration macros in HLSLSupport.cginc and SRP core package to use explicitly typed texture declaration so that the precision information will propagate properly on mobile shader targets. (<a href="https://issuetracker.unity3d.com/issues/android-shader-system-fps-drop-on-some-android-devices-caused-by-shader-compiler">1363451</a>)</p></li>
<li><p>SRP Core: Fixed a null reference exception when settings null Render Pipeline Global settings on the Settings provider. (1423712)</p></li>
<li><p>SRP Core: Fixed a serialization error when Recovering Default Volume Profile after it was deleted from the project folder. (1423734)</p></li>
<li><p>SRP Core: Fixed a SerializedObjectNotCreatableException on Volume Component Editors. (1423153)</p></li>
<li><p>SRP Core: Fixed a swaping Volume Component issue in a Volume profile when there was mixed pipeline Volume Components did not override correctly. (1427585)</p></li>
<li><p>SRP Core: Fixed a Volume Component Editor issue where Foldouts states were stored by position instead of state. (1422120)</p></li>
<li><p>Text: Fixed Text component not rendering elements with floating point coordinates correctly on machines with locale set to one that uses commas as decimal separators. (UUM-868)</p></li>
<li><p>uGUI: Fixed incorrect scroll bar handle calculations when clicking inside a scroll container that had a smaller handle rect. (<a href="https://issuetracker.unity3d.com/issues/ugui-scrollbar-ping-pongs-between-two-value-values-when-click-and-holding-in-the-interactable-area-around-the-scrollbar">1415690</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where newline caused incorrect text size rounding error. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-labels-width-is-not-extended-causing-additional-empty-lines-when-using-specific-resolutions">UUM-4169</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where the expanded state of the ListView would not be serialized across selections. (UUM-1461)</p></li>
<li><p>UI Toolkit: Fixed an issue where the VisualElement's uxml attributes would not get properly cleared after calling "Unset" or "Unset All". (UI Builder). (1385056)</p></li>
<li><p>UI Toolkit: Fixed antialiasing on 9-sliced backgrounds. (1400056)</p></li>
<li><p>UI Toolkit: Fixed EventSystem error logged in Editor when entering and leaving Play mode if there's a UIDocument in the scene. (1428877)</p></li>
<li><p>UI Toolkit: Fixed NullReferenceException followed by ArgumentException when removing an element from its panel during a style transition. (<a href="https://issuetracker.unity3d.com/issues/uitoolkit-argumentexceptions-are-thrown-and-spammed-after-transition-with-empty-property">1413513</a>)</p></li>
<li><p>UI Toolkit: Fixed rendering glitch on circles caused by incorrect geometry. (<a href="https://issuetracker.unity3d.com/issues/ios-uitoolkit-renders-incorrectly-while-scrolling">1357998</a>)</p></li>
<li><p>UI Toolkit: Fixed some Layout Update Struggling issues related to ScrollViews. (1417765)</p></li>
<li><p>UI Toolkit: Fixed the position of the drag element of slider not being updated when resizing the label element. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkits-sliders-handle-goes-out-of-bounds-when-changing-the-sliders-width">1422677</a>)</p></li>
<li><p>UI Toolkit: Fixed UI Toolkit runtime panels sometimes ignoring clicks in a build. (<a href="https://issuetracker.unity3d.com/issues/ui-elements-buttons-no-longer-register-clicks-in-build">1419208</a>)</p></li>
<li><p>UI Toolkit: Fixed visual artifact when border width is larger than border radius. (<a href="https://issuetracker.unity3d.com/issues/ui-builder-artifacts-appear-on-the-visualelement-corners-when-borders-width-is-10px-and-radius-0px">1420601</a>)</p></li>
<li><p>UI Toolkit: Fixed VisualElements change scaling when mouse moves over a different window on a higher DPI display. (<a href="https://issuetracker.unity3d.com/issues/visualelements-change-scaling-when-mouse-moves-over-ui-builder-window-on-a-higher-dpi-display-1">UUM-7260</a>)</p></li>
<li><p>Universal Windows Platform: Fixed a crash when entering a composition string longer than 64 characters into the IME. (<a href="https://issuetracker.unity3d.com/issues/uwp-player-crashes-when-typing-in-japanese-full-width-katakana">UUM-928</a>)</p></li>
<li><p>Universal Windows Platform: Fixed Application.OpenURL asserting due to not freeing temporary memory. (<a href="https://issuetracker.unity3d.com/issues/backport-uwp-universal-windows-platform-build-crashes-when-using-application-dot-openurl">UUM-2205</a>)</p></li>
<li><p>Universal Windows Platform: Fixed Build &amp; Run picking the wrong instance of Visual Studio which potentially doesn't have required components installed to deploy the application. (<a href="https://issuetracker.unity3d.com/issues/uwp-build-and-run-picks-the-wrong-instance-of-visual-studio-to-build-when-there-are-multiple-installed">UUM-931</a>)</p></li>
<li><p>URP: Fixed a Gizmo and grid artifact in the editor view. (<a href="https://issuetracker.unity3d.com/issues/urp-ghosting-over-the-mesh-in-the-scene-view-that-affects-gizmos-and-grid">UUM-2299</a>)</p></li>
<li><p>URP: Fixed an issue where camera UI inspector's clearFlag was not respected. (<a href="https://issuetracker.unity3d.com/issues/transition-fading-disappears-and-the-cameras-blue-background-appears-when-using-animator-in-urp">1422234</a>)</p></li>
<li><p>URP: Fixed an issue where the material upgrader was showing up when the URP package was being installed. (UUM-2434)</p></li>
<li><p>URP: Fixed missing Depth Copy texture in Scene view. (1431872)</p></li>
<li><p>URP: Fixed URP 2D - Fix Light2D upgrading issue with m_AlphaBlendOnOverlap property. (<a href="https://issuetracker.unity3d.com/issues/light-2d-alpha-blend-on-overlap-setting-does-not-update-when-upgrading-project-to-urp-11">UUM-1845</a>)</p></li>
<li><p>URP: Fixed URP 2D - incorrect output when post process is enabled. (UUM-5871)</p></li>
<li><p>URP: Fixed URP 2D - vertex color for sprite shapes. (<a href="https://issuetracker.unity3d.com/issues/2d-sprite-shape-urp-spriteshape-alpha-value-of-color-not-working-when-using-urp-and-sprite-lit-default-mat">UUM-1921</a>)</p></li>
<li><p>VFX Graph: Fixed an isse where the mirrored curve presets to match Shuriken curve editor was missing. (1411514)</p></li>
<li><p>VFX Graph: Fixed an issue when motion vector is applied on line using <code>targetOffset</code>, the VFXLoadParameter was missing. (UUM-3303)</p></li>
<li><p>VFX Graph: Fixed an issue where Position ArcSphere was failing with BlendDirection. (<a href="https://issuetracker.unity3d.com/issues/vfx-graph-blend-direction-arcsphere-bug">UUM-1295</a>)</p></li>
<li><p>VFX Graph: Fixed unexpected assert when capacity is really high. (<a href="https://issuetracker.unity3d.com/issues/thread-group-size-must-be-above-zero-error-is-thrown-when-setting-the-vfx-particle-capacity-size-to-a-10-digit-number">UUM-534</a>)</p></li>
<li><p>Video: Fixed an issue where Audio channel order from the VideoPlayer was not matching what FMOD expects for 5.1/7.1 on Android, both with Vorbis and AAC audio codecs.</p></li>
<li><p>WebGL: Fixed a bug where the soft keyboard had incorrect formatting leading to excess whitespace. (<a href="https://issuetracker.unity3d.com/issues/tmp-soft-keyboard-web-slash-mobile-blank-slash-unused-space-between-mobile-input-field-and-soft-keyboard">UUM-1161</a>)</p></li>
<li><p>WebGL: Fixed connection issue between the WebGL player and the profiler. (<a href="https://issuetracker.unity3d.com/issues/backport-webgl-profiler-does-not-autoconnect-on-webgl-builds">UUM-798</a>)</p></li>
<li><p>Windows: Fixed "Failed to determine current display mode, falling back to main display mode." error getting spammed in certain RDP scenarios. (UUM-3700)</p></li>
<li><p>XR: Fixed XR devices not following RunInBackground setting in Player Setting on PC standalone and playmode in Editor.</p></li>
</ul>

### Preview of Final 2023.1.0a4 Package changes

### Packages updated
<ul>
<li><p>com.unity.collections: <a href="https://docs.unity3d.com/Packages/com.unity.collections@1.2//changelog/CHANGELOG.html">1.2.3</a> → <a href="https://docs.unity3d.com/Packages/com.unity.collections@1.2//changelog/CHANGELOG.html">1.2.4</a></p></li>
<li><p>com.unity.2d.animation: <a href="https://docs.unity3d.com/Packages/com.unity.2d.animation@9.0//changelog/CHANGELOG.html">9.0.0-pre.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.2d.animation@9.0//changelog/CHANGELOG.html">9.0.0-pre.3</a></p></li>
<li><p>com.unity.2d.common: <a href="https://docs.unity3d.com/Packages/com.unity.2d.common@8.0//changelog/CHANGELOG.html">8.0.0-pre.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.2d.common@8.0//changelog/CHANGELOG.html">8.0.0-pre.2</a></p></li>
<li><p>com.unity.2d.psdimporter: <a href="https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.0//changelog/CHANGELOG.html">8.0.0-pre.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.0//changelog/CHANGELOG.html">8.0.0-pre.3</a></p></li>
<li><p>com.unity.addressables: <a href="https://docs.unity3d.com/Packages/com.unity.addressables@1.20//changelog/CHANGELOG.html">1.20.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.addressables@1.20//changelog/CHANGELOG.html">1.20.3</a></p></li>
<li><p>com.unity.burst: <a href="https://docs.unity3d.com/Packages/com.unity.burst@1.7//changelog/CHANGELOG.html">1.7.2</a> → <a href="https://docs.unity3d.com/Packages/com.unity.burst@1.7//changelog/CHANGELOG.html">1.7.3</a></p></li>
<li><p>com.unity.collab-proxy: <a href="https://docs.unity3d.com/Packages/com.unity.collab-proxy@1.15//changelog/CHANGELOG.html">1.15.18</a> → <a href="https://docs.unity3d.com/Packages/com.unity.collab-proxy@1.17//changelog/CHANGELOG.html">1.17.1</a></p></li>
<li><p>com.unity.ide.rider: <a href="https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html">3.0.14</a> → <a href="https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html">3.0.15</a></p></li>
<li><p>com.unity.ide.visualstudio: <a href="https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html">2.0.15</a> → <a href="https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html">2.0.16</a></p></li>
<li><p>com.unity.inputsystem: <a href="https://docs.unity3d.com/Packages/com.unity.inputsystem@1.3//changelog/CHANGELOG.html">1.3.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.inputsystem@1.4//changelog/CHANGELOG.html">1.4.1</a></p></li>
<li><p>com.unity.mobile.notifications: <a href="https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.0//changelog/CHANGELOG.html">2.0.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.0//changelog/CHANGELOG.html">2.0.2</a></p></li>
<li><p>com.unity.purchasing: <a href="https://docs.unity3d.com/Packages/com.unity.purchasing@4.1//changelog/CHANGELOG.html">4.1.5</a> → <a href="https://docs.unity3d.com/Packages/com.unity.purchasing@4.2//changelog/CHANGELOG.html">4.2.1</a></p></li>
<li><p>com.unity.remote-config: <a href="https://docs.unity3d.com/Packages/com.unity.remote-config@3.0//changelog/CHANGELOG.html">3.0.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.remote-config@3.1//changelog/CHANGELOG.html">3.1.3</a></p></li>
<li><p>com.unity.remote-config-runtime: <a href="https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@3.0//changelog/CHANGELOG.html">3.0.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@3.1//changelog/CHANGELOG.html">3.1.3</a></p></li>
<li><p>com.unity.render-pipelines.core: <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@14.0//changelog/CHANGELOG.html">14.0.3</a> → <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@15.0//changelog/CHANGELOG.html">15.0.0</a></p></li>
<li><p>com.unity.render-pipelines.high-definition: <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@14.0//changelog/CHANGELOG.html">14.0.3</a> → <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@15.0//changelog/CHANGELOG.html">15.0.0</a></p></li>
<li><p>com.unity.render-pipelines.high-definition-config: <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@14.0//changelog/CHANGELOG.html">14.0.3</a> → <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@15.0//changelog/CHANGELOG.html">15.0.0</a></p></li>
<li><p>com.unity.render-pipelines.universal: <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@14.0//changelog/CHANGELOG.html">14.0.3</a> → <a href="https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@15.0//changelog/CHANGELOG.html">15.0.0</a></p></li>
<li><p>com.unity.scriptablebuildpipeline: <a href="https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.20//changelog/CHANGELOG.html">1.20.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.20//changelog/CHANGELOG.html">1.20.2</a></p></li>
<li><p>com.unity.services.authentication: <a href="https://docs.unity3d.com/Packages/com.unity.services.authentication@2.0//changelog/CHANGELOG.html">2.0.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.services.authentication@2.1//changelog/CHANGELOG.html">2.1.1</a></p></li>
<li><p>com.unity.services.cloudcode: <a href="https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.0//changelog/CHANGELOG.html">2.0.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.0//changelog/CHANGELOG.html">2.0.1</a></p></li>
<li><p>com.unity.services.cloudsave: <a href="https://docs.unity3d.com/Packages/com.unity.services.cloudsave@2.0//changelog/CHANGELOG.html">2.0.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.services.cloudsave@2.0//changelog/CHANGELOG.html">2.0.1</a></p></li>
<li><p>com.unity.services.core: <a href="https://docs.unity3d.com/Packages/com.unity.services.core@1.4//changelog/CHANGELOG.html">1.4.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.services.core@1.4//changelog/CHANGELOG.html">1.4.2</a></p></li>
<li><p>com.unity.shadergraph: <a href="https://docs.unity3d.com/Packages/com.unity.shadergraph@14.0//changelog/CHANGELOG.html">14.0.3</a> → <a href="https://docs.unity3d.com/Packages/com.unity.shadergraph@15.0//changelog/CHANGELOG.html">15.0.0</a></p></li>
<li><p>com.unity.visualeffectgraph: <a href="https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@14.0//changelog/CHANGELOG.html">14.0.3</a> → <a href="https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@15.0//changelog/CHANGELOG.html">15.0.0</a></p></li>
<li><p>com.unity.xr.oculus: <a href="https://docs.unity3d.com/Packages/com.unity.xr.oculus@3.0//changelog/CHANGELOG.html">3.0.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.xr.oculus@3.0//changelog/CHANGELOG.html">3.0.2</a></p></li>
<li><p>com.unity.learn.iet-framework: <a href="https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@2.2//changelog/CHANGELOG.html">2.2.1</a> → <a href="https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@2.2//changelog/CHANGELOG.html">2.2.2</a></p></li>
<li><p>com.unity.learn.iet-framework.authoring: <a href="https://docs.unity3d.com/Packages/com.unity.learn.iet-framework.authoring@1.0//changelog/CHANGELOG.html">1.0.2</a> → <a href="https://docs.unity3d.com/Packages/com.unity.learn.iet-framework.authoring@1.0//changelog/CHANGELOG.html">1.0.3</a></p></li>
<li><p>com.unity.transport: <a href="https://docs.unity3d.com/Packages/com.unity.transport@1.0//changelog/CHANGELOG.html">1.0.0</a> → <a href="https://docs.unity3d.com/Packages/com.unity.transport@1.1//changelog/CHANGELOG.html">1.1.0</a></p></li>
<li><p>com.unity.netcode.gameobjects: <a href="https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.0//changelog/CHANGELOG.html">1.0.0-pre.9</a> → <a href="https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.0//changelog/CHANGELOG.html">1.0.0</a></p></li>
<li><p>com.unity.multiplayer.tools: <a href="https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@1.0//changelog/CHANGELOG.html">1.0.0-pre.7</a> → <a href="https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@1.0//changelog/CHANGELOG.html">1.0.0</a></p></li>
</ul>

#### Packages added
<ul>
<li><a href="https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.0//changelog/CHANGELOG.html">com.unity.memoryprofiler@1.0.0-pre.2</a></li>
</ul>
