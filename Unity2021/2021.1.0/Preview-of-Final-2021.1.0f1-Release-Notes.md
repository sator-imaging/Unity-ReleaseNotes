# Unity 2021.1.0
https://unity3d.com/unity/whats-new/2021.1.0

## Preview of Final 2021.1.0f1 Release Notes


### Features
<ul>
<li><p>2D: Added a button in the Tile Palette window to let users toggle drawing of Grid Gizmo in the Tile Palette window.</p></li>
<li><p>2D: Added a confirmation dialog for the Sprite Editor window when the Apply or Revert button is pressed. Enable or disable this option in Preferences.</p></li>
<li><p>2D: Added an option to enable/disable Alpha Dilate for SpriteAtlas.<br> This adds ability to use Alpha Transparency for padding pixels around Sprite Borders when packing SpriteAtlas.</p></li>
<li><p>2D: Added C# Job Tessellation support for Fill Area of SpriteShape.</p></li>
<li><p>2D: Added Isometric Grid slicing to Sprite Editor.</p></li>
<li><p>2D: Enabled users to toggle drawing of Grid Gizmo for a Grid component in the SceneView. To enable or disable this feature, use the SceneView Gizmo button or the list in the Gizmo dropdown.</p></li>
<li><p>Burst: Added a compiler warning for any use of throwing an exception from a method <strong>not guarded by</strong> <code>[Conditional("ENABLE_UNITY_COLLECTIONS_CHECKS")]</code>. Since exceptions in Burst are only supported in the editor, this provides a useful warning to users who may be relying on try/catch behaviors for control-flow which is not supported in final game builds.</p></li>
<li><p>Burst: Added ability for exceptions thrown from Burst to contain a callstack.</p></li>
<li><p>Burst: Added experimental support for some ArmV8.2A intrinsics (dotprod, crypto, RDMA).</p></li>
<li><p>Burst: Added experimental support for tvOS.</p></li>
<li><p>Burst: Added first batch of Arm Neon intrinsics. Currently, only ArmV8 (AArch64) targets are supported. The supported intrinsics include all ArmV7 and ArmV8 ones.</p></li>
<li><p>Burst: Added intrinsics support for <code>AtomicSafetyHandle.NewStaticSafetyId</code>.</p></li>
<li><p>Burst: Added preliminary support for loading additional burst compiled libraries in play mode/standalone.</p></li>
<li><p>Burst: Added support for Apple silicon chipsets.</p></li>
<li><p>Burst: Added support for calling Burst code directly from C# without using function pointers.</p></li>
<li><p>Burst: Added support for creating profiler markers from Burst code.</p></li>
<li><p>Burst: Added support for new intrinsics.</p></li>
<li><p>Burst: Added support for stacktraces in Burst exceptions.</p></li>
<li><p>Burst: Added support for try/finally and using/foreach for IDisposable patterns.</p></li>
<li><p>Burst: Added support for version 11 of the LLVM compiler infrastructure.</p></li>
<li><p>Burst: Added support for Visual Studio 2017 for certain platforms.</p></li>
<li><p>Burst: Added support to load additional burst libraries in playmode/standalone for the intention of allowing Modding support on desktop platforms.</p></li>
<li><p>Burst: Added the new option <code>[BurstCompile(DisableSafetyChecks = true)]</code> which allows per job or function-pointer disabling of safety checks.</p></li>
<li><p>Burst: Added the option to display Burst compilation status in the Background Tasks window.</p></li>
<li><p>Burst: Added <code>BurstCompiler.IsEnabled</code> API.</p></li>
<li><p>Burst: An error message if attempting to BurstCompiler.CompileFunctionPointer() on a multicast delegate, since this is not supported in Burst.</p></li>
<li><p>Burst: Improved Editor experience by scheduling compilation immediately after assemblies are changed, instead of waiting until Play Mode is entered.</p></li>
<li><p>Burst: Improved our aliasing detection to allow <code>DynamicBuffer</code> structs to be easily vectorizable.</p></li>
<li><p>Burst: Updated Burst to fully support ARMv7 and ARMv8-A Neon intrinsics.</p></li>
<li><p>Burst: Updated Burst to use version 10.0.0 of the LLVM compiler infrastructure by default.</p></li>
<li><p>Burst: You can now select explicit x86/x64 architecture SIMD target for Universal Windows Platform.</p></li>
<li><p>Editor: Added Device Simulator window as a Core feature of the Editor.</p></li>
<li><p>Editor: Fetch the access token in a synchronous way if username and password are passed in arguments.</p></li>
<li><p>Editor: Improved integration Search in Unity.</p></li>
<li><p>Graphics: Added support for skinned mesh sampling in VFX.</p></li>
<li><p>Mobile: Added a transparency scaler for Adaptive Performance.</p></li>
<li><p>Mobile: Added settings for Adaptive Performance to control the Indexer's thermal and performance actions when using the Device Simulator.</p></li>
<li><p>Package: Added Visual Scripting (previously known as Bolt) as a default package.</p></li>
<li><p>Package Manager: Added a new <em>Add package by name</em> dropdown option and revamped the existing <em>Add from git URL</em> dropdown option.</p></li>
<li><p>Package Manager: Added an information box describing the current flow of the package when the version is not "Released".</p></li>
<li><p>Package Manager: Provided more choices concerning the Load Next value when using the My Assets filter.</p></li>
<li><p>Package Manager: Removed 'See all versions' option in version list for external users, and added Project Setting for internal users to re-enable this option.</p></li>
<li><p>Package Manager: Removed the "Release Candidate (RC)" tags from the Package Manager for released builds. RC packages now show the "Pre-release" tags.</p></li>
<li><p>Package Manager: The Package Manager now supports installing packages from a browser hyperlink (even experimental packages).</p></li>
<li><p>Package Manager: Updated Package Manager UI version tags for new Lifecycle and logic for recommending/showing available versions to users.</p></li>
<li><p>Particles: Added new Emitter velocity mode - Manual. This mode can be used to override the ParticleSystem's calculated emitter velocity value. This gives scripts complete control over the ParticleSystem velocity. It is also possible to use this whilst authoring a system to simulate movement when making an effect that relies on movement.</p></li>
<li><p>Scripting: Added the ability to setup script compilation defines in the assmebly definition inspector, depending on the Unity version the scripts are being compiled for.</p></li>
<li><p>UI Toolkit: Added 2D Sprites use as background style images.</p></li>
<li><p>UI Toolkit: Added in-Canvas style toggles for flex and text alignment.</p></li>
<li><p>UI Toolkit: Added rich text style properties to the Inspector.</p></li>
<li><p>UI Toolkit: Added sprite support in UI Toolkit.</p></li>
<li><p>UI Toolkit: Added support for azimuthAngle, altitudeAngle, twist, and multiple Pen devices in EventSystem when using Input System package.</p></li>
<li><p>UI Toolkit: Added support for mixed values mode in the UI Toolkit when implementing the Property field.</p></li>
<li><p>UI Toolkit: Added the ability to drag and drop and re-order elements in the Canvas.</p></li>
<li><p>UI Toolkit: Added the PanelEventHandler and PanelRaycaster components. These enable the UI Toolkit panels to receive events and selections from a standard UI EventSystem. Added the SetUITookitEventSystemOverride method to  EventSystem. This lets you override the UI Toolkit event system and define whether to create panel components automatically on start. Added PanelSettings sortingOrder to determine drawing and selection order between UI Toolkit panels and UI canvases.</p></li>
<li><p>UI Toolkit: Added UI Builder, a visual UI authoring tool for UI Toolkit, to the Unity Editor. This was previously released as a package (com.unity.ui.builder).</p></li>
<li><p>UI Toolkit: Added user theme stylesheet enumeration and preview in the Canvas.</p></li>
<li><p>UI Toolkit: Added USS variable search in Inspector style fields.</p></li>
<li><p>UI Toolkit: Implemented dynamic texture slots to reduce batch breaking.</p></li>
<li><p>XR: Implemented Late Latching for XR to reduce rendering latency.</p></li>
<li><p>XR: Implemented Late Latching to reduce VR latency.</p></li>
</ul>

### Improvements
<ul>
<li><p>2D: Added information foldout in Tilemap Inspector for showing the Tile and Sprite assets used in the Tilemap.</p></li>
<li><p>2D: Better placements of Tiles generated from Sprites whose Texture was Isometric Sliced in the Sprite Editor.</p></li>
<li><p>2D: Improve performance when applying changes after slicing a texture for the Sprite Editor.</p></li>
<li><p>2D: Improved Automatic Palette Sizing by setting a better fitting size when sizes of Sprites are of multiples of each other. Otherwise, the largest size for Sprites is used.</p></li>
<li><p>2D: Improved memory and speed of Animation SpritePostProcess for large sprite count.</p></li>
<li><p>2D: Improved performance in SceneView for SceneViewOpenTilePaletteHelper.</p></li>
<li><p>2D: Improved slicing performance. (<a href="https://issuetracker.unity3d.com/issues/2d-slicing-of-a-sprite-became-never-ending-process-when-cell-size-8-by-8-selected">1271316</a>)</p></li>
<li><p>2D: Show grid preview when slicing spritesheets.</p></li>
<li><p>2D: Store and reuse last used location when creating Tiles from the Tile Palette window.</p></li>
<li><p>2D: Update 2D template to use current verified version of 2D packages.</p></li>
<li><p>Android: Enabled use of Android 11 setFrameRate API when Optimized Frame Pacing is enabled and Vulkan is used, similar to OpenGL ES.</p></li>
<li><p>Android: Expanded the Create symbols.zip build setting for Android. The options are Disabled/Public/Debugging. Modified the symbols to always have the .so extension. Symbols are included for libil2cpp (if IL2CPP is selected), libmonobdwgc-2.0 (if Mono is selected), libunity, libmain. If uploading the zip package to Google Play Console for automatic stacktrace resolving, use Public symbols. (1288739)</p></li>
<li><p>Android: Improved load and reload time for OBBs.</p></li>
<li><p>Android: Improved Time.deltaTime consistency for OpenGL ES and Vulkan graphics APIs.</p></li>
<li><p>Android: Updated Android NDK to r21d.</p></li>
<li><p>Asset Import: Improved performance when registering Scripted Importers, especially when large numbers of scripted importers are being registered together. (<a href="https://issuetracker.unity3d.com/issues/compilation-with-5000-scriptedimporters-is-very-slow-takes-250-seconds">1228635</a>)</p></li>
<li><p>Asset Import: Optimized the import processing when using "Alpha is Transparency" texture import option. The processing is now several times faster.</p></li>
<li><p>Asset Import: Reduced cost of domain reloads on asset import worker process by removing unnecessary additional domain reloads.</p></li>
<li><p>Asset Pipeline: Added documentation for: IsDirectoryMonitoringEnabled, IsAssetImportWorkerProcess, GetTextMetaFilePathFromAssetPath, CacheServerConnectionChangedParameters, cacheServerConnectionChanged.</p></li>
<li><p>Asset Pipeline: Calling ForceProduceArtifact now also omits the use of local cached artifacts, in addition to omitting cache server artifacts.</p></li>
<li><p>Asset Pipeline: Changed API doc:AssetDatabase.LoadAssetAtPath.</p></li>
<li><p>Asset Pipeline: Changed how logging behaves when an import worker is importing. Logging is now forwarded to the main editor log.</p></li>
<li><p>Asset Pipeline: Improved calling ProduceArtifact rapidly so that it doesn't produce multiple artifacts.</p></li>
<li><p>Asset Pipeline: SpriteAtlas importer gathers its differences differently now.</p></li>
<li><p>Build Pipeline: (DS-1018) Added WithDebugInformationFormat to the compiler settings for MsvcCompiler.</p></li>
<li><p>Build Pipeline: Upgraded udp package to 2.1.0.</p></li>
<li><p>Burst: Improved codegen.</p></li>
<li><p>Core: Improved error message in certain cases where the disk is full.</p></li>
<li><p>Core: Reduced thread contention on JobQueue internal memory allocation.</p></li>
<li><p>Documentation: Clarified an aspect of Mip Stripping docs.</p></li>
<li><p>DX12: Optimize ray tracing acceleration structure building on the render thread (roughly 2x speedup).</p></li>
<li><p>DX12: When reading vertex attributes from vertex buffers (closest hit / any hit shaders), we now fill only the channels that are available instead of returning 0 when trying to read more attribute channels than available.</p></li>
<li><p>Editor: A newly-created Scene View window now copies last active Scene View settings. (1264773)</p></li>
<li><p>Editor: Added "Localize compiler messages" to Preference Window&gt;Language to localize compiler messages in the current language.</p></li>
<li><p>Editor: Arrays/lists inspector UI control now supports multi-selection of array elements.</p></li>
<li><p>Editor: Clear on Recompile' option added to console's 'Clear' context menu. (<a href="https://issuetracker.unity3d.com/issues/console-window-add-clear-on-recompile-option">1264753</a>)</p></li>
<li><p>Editor: Improve the multi-selection display of Culling Mask and Static fields of certain components. (<a href="https://issuetracker.unity3d.com/issues/imgui-maskfield-and-staticflags-multi-edit-control-behavior-should-be-improved">1190806</a>)</p></li>
<li><p>Editor: Improved the reliability of our SQLite implementation.</p></li>
<li><p>Editor: LODGroup values can now be edited via input fields in addition to the slider. Input field editing also works in multi-selection mode.</p></li>
<li><p>Editor: Optimized mobile ASTC texture compression (about two times faster now).</p></li>
<li><p>Editor: Optimized mobile ASTC texture compression again (~10% faster).</p></li>
<li><p>Editor: Optimized mobile ETC/ETC2/EAC texture compression (about two times faster now).</p></li>
<li><p>Editor: Optimized mobile PVRTC texture compression (8% faster).</p></li>
<li><p>Editor: Optimized various parts of texture importing (5%-20% faster depending on settings and texture types used).</p></li>
<li><p>Editor: Optimized various parts of texture importing (~10% faster depending on settings and texture types used).</p></li>
<li><p>Editor: Reduced Editor repaints while rendering HDRP.</p></li>
<li><p>Editor: Removed Enable Code Coverage option from Preferences/General and moved it inside the Code Coverage package.</p></li>
<li><p>Editor: Scene/Game view Gizmos drop-down window now has a Search field. (1274775)</p></li>
<li><p>Editor: Two new events added to ObjectSelector: ObjectSelectorSelectionDone: An item in the list is double-clicked; and ObjectSelectorCanceled: The window was closed by explicitly pressing escape on the keyboard.</p></li>
<li><p>GI: Hid Enlighten-specific settings when it is not supported by the SRP. Affected areas are Mesh Renderer, Light, Scene view, Lighting Explorer and Lightmap Parameters.</p></li>
<li><p>GI: Removed very verbose logging behavior during lighting data asset building.</p></li>
<li><p>GI: Unity now stores memory-related logs in a file instead of just reporting them in the console.</p></li>
<li><p>Graphics: Exposed RayTracingAccelerationStructure.RemoveInstance to C# Scripting API.</p></li>
<li><p>Graphics: Fixed async readback crashing on DX12 if buffer was a SubUpdates buffer.</p></li>
<li><p>Graphics: Improved error on DX12 while trying to set stable power state but windows was not in developer mode.</p></li>
<li><p>Graphics: Improved the compression speed of ASTC textures.</p></li>
<li><p>Graphics: Improved the loading time of single mip cubemaps on GameCore.</p></li>
<li><p>Graphics: Optimized static batching process, e.g. entering play mode with 30k static batched objects in the editor is faster by two seconds.</p></li>
<li><p>Graphics: Removed redundant calls when setting shader program parameters.</p></li>
<li><p>Graphics: UnityEngine.Profiling.Recorder.gpuElapsedNanoseconds now can measure GPU time on OpenGL ES3.</p></li>
<li><p>IL2CPP: Improved IL2CPP failure so it results in one (instead of two) error messages. The error message text is displayed with as little extra information as possible, so that it is more understandable.</p></li>
<li><p>IL2CPP: Improved the error message that was displayed when building for Windows and the required Visual Studio components were not installed.</p></li>
<li><p>IL2CPP: On Android, the public symbol file (for ex., libil2cpp.sym.so) will no longer contain debugging symbols, it will only contain the symbol table. Debugging symbols are present in libil2cpp.dbg.so. This should significantly lower the file size of libil2cpp.sym.so.</p></li>
<li><p>IL2CPP: When script debugging is enabled, stack traces include C# source code line numbers for all assemblies where debug symbols are available.</p></li>
<li><p>Kernel: Fixed instability in FolderContentsMatchesTheOneReturnedByGenerateDirectoryStructure test.</p></li>
<li><p>License: Synced access token with L-Client upon change.</p></li>
<li><p>Mobile: Updated Mobile Notifications package to 1.3.2.</p></li>
<li><p>Networking: Make UnityWebRequest objects properly show up in profiler. (1017004)</p></li>
<li><p>Package: Updated input system package to 1.0.2.</p></li>
<li><p>Package: Updated to ProBuilder 5.0.0.</p></li>
<li><p>Package: Updated udp 2.1.4.</p></li>
<li><p>Package: Visual Scripting: A warning is raised when adding more than one Input unit in a SuperUnit.</p></li>
<li><p>Package: Visual Scripting: Open the inspector button and double clicking a graph in the project browser, now opens the visual scripting editor.</p></li>
<li><p>Package: Visual Scripting: Warns the user when an Input System Package event is referencing an action of the wrong type for that event.</p></li>
<li><p>Physics: Rearrange the ArticulationBody properties so that damping and friction is located right after mass and is not visually separated from it by the anchor properties.</p></li>
<li><p>Prefabs: Optimized the performance of undo operations on objects in nested Prefabs by up to 30%.</p></li>
<li><p>Profiler: Added profiling support for Asset importing via direct IP connection.</p></li>
<li><p>Profiler: Added progress bar for loading and saving Profiler data.</p></li>
<li><p>Profiler: Added the ability to specify a port in the Profiler Window, when connecting to the Profiler to a player via an IP address.</p></li>
<li><p>Profiler: Changed call stacks displayed in the CPU Usage Profiler module so that they only show calls that have more information than just their memory address, by default. Enable <em>Full details for Call Stacks</em> if you want to see the addresses.</p></li>
<li><p>Profiler: Changed call stacks displayed in the selection tool-tip of Timeline view so that they are clickable if they contain file information.</p></li>
<li><p>Profiler: Duplicated sample names in the Call view's tooltip to improve readability. (<a href="https://issuetracker.unity3d.com/issues/profiler-gpu-module-hides-call-names-and-total-time-when-the-call-name-doesnt-fit-in-the-given-row">1241955</a>)</p></li>
<li><p>Scripting: Added c/cpp/mm/m/java/h as defaults to "Project Settings-&gt;Editor-&gt;Additional extensions", so they appear in the code editor, which therefore provides an easy way to edit and inspect them. (1284679)</p></li>
<li><p>Scripting: Added support for new managed code stripping annotation attributes.</p></li>
<li><p>Scripting: Added support for Unity Version Defines in Assembly definition import options.<br> This feature improvement allows scripts to easily specify different code snippets for different Unity version ranges. This is especially useful for introducing calls to newly added public APIs, in which case these API calls need to be guarded by defines based on a Unity version range of a given Unity version or later.<br>
The Unity version range expression syntax is the same as the package version range expressions. The Unity version format differs from the package version format, so Unity version expressions are evaluated based on some rules specific to the Unity version format:<br></p>

<ul>
<li>Comparison of release types follows the following rules: a&lt;b&lt;f=c&lt;p&lt;x. So for example, an alpha version is always smaller (earlier) than a beta version, regardless of the Incremental version.<br></li>
<li>The Unity versions are allowed to have suffixes (e.g 2020.1.3-bonfire) which are ignored by the Unity version comparison code<br></li>
<li>Chinese releases are equivalent to public releases (f) so for the sake of comparison in the version range expression 2020.1f3 would be equal to 2020.1c3.<br></li>
<li>Experimental releases don't include an Incremental Version. For example. everything after 2020.2.1x would be treated as a suffix and ignored by the version comparison.</li>
</ul></li>
<li><p>Scripting: Changed Roslyn analyzers to be run as part of the normal compilation step.<br> This also results in analyzer errors being treated as compiler errors.</p></li>
<li><p>Scripting: Greatly improved the performance of GameObject.FindGameObjectWithTag and GameObject.FindGameObjectsWithTag.</p></li>
<li><p>Scripting: Improved the performance of the ApiUpdater.</p></li>
<li><p>Scripting: Improved the user interface when setting up Unity version defines for asm definitions in the Editor.</p></li>
<li><p>Scripting: Script Compilation is now incremental across player builds.</p></li>
<li><p>Scripting: Script compilation now has a background task progress bar when auto-refresh is disbled.</p></li>
<li><p>Scripting: Script Updater approval dialog now shows you which files will be overwritten before you give permission.</p></li>
<li><p>Scripting: Script Updater now causes fewer script recompiles when importing/upgrading projects.</p></li>
<li><p>Scripting: Scripting: Improved documentation for Application.isPlaying.</p></li>
<li><p>Scripting: The errors that trigger a script updater are no longer displayed in the console window.</p></li>
<li><p>Scripting: The MenuItem for manually running script updater is removed. It now always offers to update when it finds a compilation error it can fix.</p></li>
<li><p>Search: Fixed search doesn't display all results in project view. It now includes the same result as the legacy search engine (i.e. AssetDatabase.FindAssets). (<a href="https://issuetracker.unity3d.com/issues/search-doesnt-display-all-results-in-project-view">1310140</a>)</p></li>
<li><p>Search: Improved the search help text when there is no result for the current search tab.</p></li>
<li><p>Shaders: #pragma require now works from compute shaders as well.</p></li>
<li><p>Shaders: Added shader name to messages in the log about shader state being unsupported,.</p></li>
<li><p>Shaders: Shaders can now use UNITY_PLATFORM_&lt;PLATFORM_NAME&gt; defines to specialize compilation per build target platform (examples: UNITY_PLATFORM_OSX, UNITY_PLATFORM_WINDOWS).</p></li>
<li><p>Terrain: Added "Delete Brush..." button to the brush selection UI.</p></li>
<li><p>Terrain: Now a "Hole Edge Padding" option is added to terrain Detail Prototype that you can control how far details objects will be from the hole edge.</p></li>
<li><p>Terrain: Now an error message will show up on UI when you select an invalid detail prototype.</p></li>
<li><p>Terrain: Reduced Terrain per-frame CPU update cost.</p></li>
<li><p>UI Toolkit: Improved renderer batching.</p></li>
<li><p>Version Control: Smart Merge (UnityYamlMerge) now allows ignoring "tiny" float differences in some fields. For a configuration example, see mergerules.txt. (1211899)</p></li>
<li><p>WebGL: Added support for QualitySettings.vsyncCount.</p></li>
<li><p>WebGL: Added support for smooth rendering of decimated frame rates for 60/k fps  (30, 20, 15, 12, 10 and 5 fps).</p></li>
<li><p>WebGL: Added support for vsyncless rendering for development/profiling purposes. To enable this, set QualitySettings.vsyncCount = 0 and Application.targetFrameRate = 1000.</p></li>
<li><p>XR: Updated API docs on XRDisplaySubsystem.scaleOfAllViewports and XRDisplaySubsystem.scaleOfAllRenderTargets.</p></li>
<li><p>XR: Updated MagicLeap XR Plugin package to 6.2.2.</p></li>
<li><p>XR: Updated Oculus XR Plugin package to 1.8.1.</p></li>
<li><p>XR: Updated Windows Mixed Reality package to 4.1.1.</p></li>
<li><p>XR: Updated XR Plug-in Management package to 3.2.16 and Windows MR XR Plug-in package to 5.0.0.</p></li>
</ul>

### API Changes
<ul>
<li><p>2D: Added: Added Tilemap.GetUsedSpritesCount/NonAlloc to allow users to get information on the Sprites used in the Tilemap.</p></li>
<li><p>2D: Added: Added Tilemaps.TileFlags.KeepGameObjectRuntimeOnly flag to allow users to keep GameObjects from Tiles after removing the originating Tile.</p></li>
<li><p>2D: Added: SpriteAtlasAsset can be loaded/saved using SpriteAtlasAsset.Load and SpriteAtlasAsset.Save.</p></li>
<li><p>Android: Added: Added API level 30 to AndroidSdkVersions enum.</p></li>
<li><p>Animation: Added: Added a new parameter to the MatchTarget function for auto matching completion in case of interruption.</p></li>
<li><p>Animation: Added: Added UnbindAllStreamHandles and UnbindAllSceneHandles to manage Animation C# job handles. (<a href="https://issuetracker.unity3d.com/issues/animation-rigging-animator-dot-rebind-cant-resolve-bone-on-an-animator-that-featured-a-previously-active-rig-constraint">1238832</a>)</p></li>
<li><p>Asset Bundles: Added: Added AssetBundle.UnloadAsync for unloading assetbundles in the background. (1281619)</p></li>
<li><p>Asset Import: Added: Added <code>CanOpenAssetInEditor</code> method to check whether an asset would be opened in Editor.</p></li>
<li><p>Build Pipeline: Added: ContentBuildInterface.CalculatePlayerSerializationHashForType for providing precise per type dependency tracking for incremental rebuild of asset bundles.</p></li>
<li><p>Build Pipeline: Added: New API FilterToSubset on BuildReferenceMap &amp; BuildUsageTagSet providing more control over native build data, reducing unnecessary asset bundle rebuilds.</p></li>
<li><p>Burst: Added: Intrinsics: Neon - Added support for basic vld1 APIs.</p></li>
<li><p>Core: Added: Added new Screen, Application and SystemInfo classes in UnityEngine.Device namespace, that can mimic platform-specific behavior in the Unity Editor when used with Device Simulator.</p></li>
<li><p>Editor: Added: Added a callback when pivot mode, pivot rotation, view tool enable and grid snap enable are changed.</p></li>
<li><p>Editor: Added: Added EditorGUIUtility.SetMainWindowPosition.</p></li>
<li><p>Editor: Added: Added MeshPreview class for drawing an interactive Editor preview of a Mesh asset. (1184921)</p></li>
<li><p>Editor: Added: Added <code>attributeType</code> argument to OnOpenAssetAttribute to denote a function used to check if the asset would be opened in Editor.</p></li>
<li><p>Editor: Added: API method for setting custom diff tool. (<a href="https://issuetracker.unity3d.com/issues/extension-point-for-revision-control-diff-slash-merge-which-allows-to-add-custom-tool-rider-to-diff-tools-drop-down">1246952</a>)</p></li>
<li><p>Editor: Added: EditorGUI.LinkButton and EditorGUILayout.LinkButton are now public.<br> EditorUtility.OpenPropertyEditor  is now public.</p></li>
<li><p>Editor: Added: EditorUtility SetDefaultParentObject and ClearDefaultParentObject methods were added.</p></li>
<li><p>Editor: Added: Improved Search API documentation and added many examples.</p></li>
<li><p>Editor: Changed: HelpURLAttribute now supports derived classes in order to generate dynamic URLs.</p></li>
<li><p>Editor: Obsoleted: Remove Slave from MPE API and documentation.</p></li>
<li><p>Editor: Obsoleted: Renamed some SearchService API's classes to prevent name clashes.</p></li>
<li><p>GI: Added: Added two new callbacks: LightProbes.needsRetetrahedralization which is called whenever the current registered probes and tetrahedralization are out of sync, and LightProbes.tetrahedralizationCompleted which fires after (re-)tetrahedralization is done.</p></li>
<li><p>Graphics: Added: Added an option to flag renderers as static shadow casters in order to facilitate the implementation of cached shadow map in SRP.</p></li>
<li><p>Graphics: Added: Added methods to check if Material/MaterialPropertyBlock contains a property based on type (e.g. MaterialPropertyBlock.HasFloat, Material.HasColor, etc.).</p></li>
<li><p>Graphics: Added: Added new API Graphics.minOpenGLESVersion and built-in keyword SHADER_API_GLES30.</p></li>
<li><p>Graphics: Added: Added new API SystemInfo.GetRenderTextureSupportedMSAASampleCount(RenderTextureDescriptor desc) to query the correct MSAA samples count of a RenderTexture.</p></li>
<li><p>Graphics: Added: Added new SystemInfo.supportsStoreAndResolveAction API to check for StoreAndResolveAction store action support on a specific platform.</p></li>
<li><p>Graphics: Added: BatchRendererGroup: Added optional visibleIndicesY array. Data available in shader in Y channel. (Hybrid Renderer V2).</p></li>
<li><p>Graphics: Added: Exposed the API to set the renderDynamicObjects for Custom reflection probes.</p></li>
<li><p>Graphics: Added: Made GraphicsSettings.GetGraphicsSettings() public.</p></li>
<li><p>Graphics: Added: Support for the PlayStation 5 platform has been added.</p></li>
<li><p>Graphics: Added: Support for the XboxSeries platform has been added.</p></li>
<li><p>Graphics: Changed: Added callbacks to RenderPipelineManager that don't cause GC. (<a href="https://issuetracker.unity3d.com/issues/urp-scriptablerendercontext-dot-getcamera-array-dot-resize-creates-garbage-every-frame-when-more-than-one-camera-is-active">1259717</a>)</p></li>
<li><p>Graphics: Changed: RenderRequestMode now has enum values for PBR materials data.</p></li>
<li><p>HDRP: Added: Added a history rejection criterion based on if the pixel was moving in world space. (1302392)</p></li>
<li><p>HDRP: Added: Added a new function in GeometryTools.hlsl to calculate triangle edge and full triangle culling.</p></li>
<li><p>HDRP: Added: Added an additional check in the "check scene for ray tracing". (1314963)</p></li>
<li><p>HDRP: Added: Added color and intensity customization for Decals.</p></li>
<li><p>HDRP: Added: Added new API in CachedShadowManager.</p></li>
<li><p>HDRP: Added: Added pivot point manipulation for Decals (inspector and edit mode).</p></li>
<li><p>HDRP: Added: Added the default quality settings to the HDRP asset for RTAO, RTR and RTGI. (1304370)</p></li>
<li><p>HDRP: Added: Added UV manipulation for Decals (edit mode).</p></li>
<li><p>HDRP: Added: API to allow OnDemand shadows to not render upon placement in the Cached Shadow Atlas.</p></li>
<li><p>HDRP: Added: Exposed update upon light movement for directional light shadows in UI.</p></li>
<li><p>iOS: Added: Added <code>iOS.Device.iosAppOnMac</code> flag to check if app built for iOS is running on Mac equipped with Apple Silicon chip.</p></li>
<li><p>iOS: Obsoleted: The public accessor for the legacy Game Center player ID is now unavailable, and will be removed completely in the next major release of Unity.</p></li>
<li><p>Mobile: Added: Adaptive Performance: Updated the version defines for the device simulator to support it in 2021.1 without package.</p></li>
<li><p>Networking: Added: UnityWebRequest now supports sending/receiving data using NativeArray, avoiding managed allocations (UploadHandlerRaw and DownloadHandlerBuffer). (1138156)</p></li>
<li><p>Package: Added: Added ApplyAfter option to ImpulseListener, to add control over the ordering of extensions.</p></li>
<li><p>Package: Added: New feature: CinemachineConfiner2D - Improved 2D confiner.</p></li>
<li><p>Package Manager: Added: The <code>UnityEditor.PackageManager.PackageInfo</code> class has a new <code>GetAllRegisteredPackages</code> method which returns the list of packages currently registered.</p></li>
<li><p>Package Manager: Obsoleted: UnityEditor.PackageManager.PackageInfo.status' and 'UnityEditor.PackageManager.PackageStatus' are now obsolete.</p></li>
<li><p>Particles: Added: Added emitterVelocity property to InitialModule.</p></li>
<li><p>Physics: Added: Expose ArticulationBody.collisionDetectionMode property to set various collision detection modes, like Discrete, Continuous and etc.</p></li>
<li><p>Physics: Added: Expose ArticulationBody.computeParentAnchor option to control whether the parent anchor is matched to the other one automatically or not.</p></li>
<li><p>Physics: Added: Expose ArticulationBody.SnapAnchorToClosestContact function to place the anchor to a position where the risk of collider overlap is minimised.</p></li>
<li><p>Physics: Added: Make WheelCollider.sprungMass writable, to enable explicit mass distributions. In addition to that, expose WheelCollider.ResetSprungMasses() to reset the vehicle back to automatically calculated implicit sprung masses. It's the same usage pattern as with Rigidbody.inertiaTensor / Rigidbody.ResetInertiaTensor().</p></li>
<li><p>Player: Added: Added several object pool implementations including: ObjectPool, LinkedPool, GenericPool, UnsafeGenericPool and CollectionPool.</p></li>
<li><p>Profiler: Added: Added API for interacting with the Profiler Window and the selection in the CPU and GPU Usage Profiler modules.</p></li>
<li><p>Scripting: Added: Added a new AsyncReadManager FileInfo() API to check for a file's existence and (if present) the file size.</p></li>
<li><p>Scripting: Added: Added Vector3Int.forward and Vector3Int.back.</p></li>
<li><p>Scripting: Added: Introduced query for compute shader hardware support:<br> ComputeShader.IsSupported(int kernelIndex).</p></li>
<li><p>Scripting: Added: Time.timeAsDouble added<br> Scripting: Time.timeSinceLevelLoadAsDouble added<br>
Scripting: Time.fixedTimeAsDouble added<br>
Scripting: Time.unscaledTimeAsDouble added<br>
Scripting: Time.fixedUnscaledTimeAsDouble added<br>
Scripting: Time.realtimeSinceStartupAsDouble added.</p></li>
<li><p>Scripting: Changed: New Added Unity.IO.LowLevel.Unsafe.ReadStatus.Truncated result for completion of a truncated read. A truncated read occurs when an asynchronous file request attempts to read beyond the end of a file.<br> Added Unity.IO.LowLevel.Unsafe.ReadStatusExtension methods -Unity.IO.LowLevel.Unsafe.ReadStatusExtension.Complete() returns true on successful completetion regardless of truncated file reads.</p></li>
<li><p>Scripting: Deprecated: Deprecated IIl2CppProcessor.</p></li>
<li><p>Scripting: Deprecated: Deprecated IUnityLinkerProcessor.OnAfterRun.</p></li>
<li><p>Scripting: Deprecated: Deprecated IUnityLinkerProcessor.OnBeforeRun.</p></li>
<li><p>Scripting: Obsoleted: Removed UnityEditorInternal.ScriptEditor.</p></li>
<li><p>Scripting: Removed: Previously undocumented EditorUtility.CompileCSharp() is removed. Its functionality can be achieved through the supported AssemblyBuilder class.</p></li>
<li><p>Scripting: Removed: Removed UnityEditorInternal.GetExternalScriptEditorArgs as it was throwing not supported exception.</p></li>
<li><p>Services: Changed: Updating analytics dashboard to point to new location.</p></li>
<li><p>Shaders: Deprecated: Material, MaterialPropertyBlock and Shader API for working with "Int" properties is deprecated. Use "Integer" or "Float" properties and the corresponding API instead.</p></li>
<li><p>UI Toolkit: Added: Added a new dropdown menu made of VisualElements to enable popup fields in runtime.</p></li>
<li><p>UI Toolkit: Added: Added a new DropdownField control to UI Toolkit runtime.</p></li>
<li><p>UI Toolkit: Added: Added KeyboardNavigationManipulator to simplify the implementation for users.</p></li>
<li><p>UI Toolkit: Added: Added MeasureTextSize method for InputFields.</p></li>
<li><p>UI Toolkit: Added: Added RadioButton and RadioButtonGroup controls.</p></li>
<li><p>UI Toolkit: Added: UQuery: Enumerator support allows for foreach iteration with no or minimal gc allocations.</p></li>
<li><p>UI Toolkit: Changed: ProgressBar was moved to UnityEngine.UIElements to support runtime.</p></li>
<li><p>UI Toolkit: Obsoleted: ShowHorizontal is obsolete. Use horizontalScrollerVisibility instead.</p></li>
<li><p>UI Toolkit: Obsoleted: ShowVertical is obsolete. Use verticalScrollerVisibility instead.</p></li>
<li><p>Universal: Added: Removed Custom.meta which was causing warnings. (<a href="https://issuetracker.unity3d.com/issues/urp-warnings-about-missing-metadata-appear-after-installing">1314288</a>)</p></li>
<li><p>VFX Graph: Added: Added sample vertices of a transformed skinned mesh with Position (Skinned Mesh) and Sample Skinned Mesh operator.</p></li>
<li><p>VFX Graph: Added: Placement option (Vertex, Edge, Surface) in Sample Mesh &amp; Skinned Mesh, allows triangle sampling.</p></li>
<li><p>XR: Added: Updated XR Plug-in Management to 4.0.1.</p></li>
</ul>

### Changes
<ul>
<li><p>2D: Updated com.unity.2d.sprite package license.</p></li>
<li><p>2D: Updated com.unity.2d.tilemap package license.</p></li>
<li><p>Android: Removed use of QualitySettings.vSyncCount for Android.</p></li>
<li><p>Android: Vulkan is no longer preferred over OpenGL ES when using Android 7 and for all Mali Midgard GPUs.</p></li>
<li><p>Asset Import: When Meshes have no material defined in the imported file, the ModelImporter now assigns the default material to them rather than creating a 'No name' material sub-asset.</p></li>
<li><p>Burst: Burst enters RC phase.</p></li>
<li><p>Burst: Burst now uses platform-provided memory intrinsics for iOS, tvOS, WASM, and console platforms.</p></li>
<li><p>Burst: Bursted DOTS Runtime Jobs are now decorated with <code>[NativePInvokeCallback]</code> instead of <code>[MonoPInvokeCallback]</code>. This fixes the problem where <code>[MonoPInvokeCallback]</code> jobs could generate callback wrappers which could cause native code to inadvertently interop with the managed VM.</p></li>
<li><p>Burst: Changed how exceptions throw types and messages are stored in our Burst binaries to reduce binary size.</p></li>
<li><p>Burst: Changed the Burst menu-item <code>Safety Checks</code> to a modal choice of <code>Off</code>, <code>On</code>, or <code>Force On</code>. <code>Force On</code> will overwrite any user job or function-pointer with <code>DisableSafetyChecks = true</code>. To avoid users falling into the consistent trap of having <code>Safety Checks</code> set to <code>Off</code>, any reload of the Editor will issue a warning telling the user that <code>Safety Checks</code> have been reset to <code>On</code>.</p></li>
<li><p>Burst: Changed to inliner heuristics to improve build time and reduce executable size.</p></li>
<li><p>Burst: DOTS Runtime shares the logging code path with the general case.</p></li>
<li><p>Burst: Eager-compilation is now cancelled when script compilation starts, to prevent spurious errors related to recompiled assemblies.</p></li>
<li><p>Burst: Exception strings no longer contain the entry-point name of the job/function-pointer that caused the throw. This change was required because the Burst compiler has to produce deterministic results from any given compile, which is fundamentally opposed to per-entry-point function derivations.</p></li>
<li><p>Burst: Improved Burst initialization time.</p></li>
<li><p>Burst: Improved Burst Inspector loading time.</p></li>
<li><p>Burst: Improved eager-compilation performance.</p></li>
<li><p>Burst: Improved performance of "eager-compilation" (scheduling compilation immediately after assemblies are changed) by cancelling queued eager-compilation when entering play mode with Synchronous Compilation unchecked.</p></li>
<li><p>Burst: Improved performance of eager-compilation by not eager-compiling test assemblies.</p></li>
<li><p>Burst: In versions of Unity older than 2019.3, changing the following options in the Burst menu now requires the Editor to be restarted: Enable Compilation, Safety Checks, and Native Debug Mode Compilation. In versions of Unity older than 2019.3, previously-compiled methods were not recompiled after changing those options, which could lead to undefined behavior where methods might not be compiled with the correct options. This change removes that possibility.</p></li>
<li><p>Burst: Made the compiler better at constant-folding complex static readonly constructors.</p></li>
<li><p>Burst: Open-generic static methods are now hidden in the Burst Inspector. They are not supported by Burst, but they were previously visible.</p></li>
<li><p>Burst: Temporarily removed the Burst compiler warning about exception throws not in [Conditional("ENABLE_UNITY_COLLECTIONS_CHECKS")] methods, to let us address user feedback. The next minor version of Burst will reincorporate this in a more friendly manner.</p></li>
<li><p>Burst: The Burst Inspector no longer uses JIT compilation. The code it shows is now compiled the same way as for editor / player usage.</p></li>
<li><p>Burst: The command line option <code>--burst-disable-compilation</code> now entirely disables Burst, including the AppDomain.</p></li>
<li><p>Burst: Updated Cross Compilation Tooling To LLVM 10.</p></li>
<li><p>Burst: Upgraded Burst to use LLVM Version 11.0.1 by default, bringing the latest optimization improvements from the LLVM project.</p></li>
<li><p>Burst: Warnings are hidden in the inspector view.</p></li>
<li><p>Burst: When using "Executable Only" build type on Universal Windows Platform, Burst will now only generate code for a single CPU architecture that you're building for.</p></li>
<li><p>Editor: Deleting an object reference array entry in the Inspector now removes that array element. Previously first deletion set the element reference to none, and the second deletion deleted the element.</p></li>
<li><p>Editor: Deprecated Device Simulator package, feature moved to Core.</p></li>
<li><p>Editor: Quick Search is now part of the Unity Editor and no package needs to be installed.</p></li>
<li><p>Graphics: Changed so texture formats DXT1 and DXT5 in the UI labels are now named "DXT1|BC1" and "DXT5|BC3", indicating terminology used by modern graphics APIs.</p></li>
<li><p>Graphics: ComputeBuffer.IsValid now returns false when compute is not supported and ComputeBuffer.BeginWrite throws InvalidOperationException for invalid ComputeBuffers. (<a href="https://issuetracker.unity3d.com/issues/android-gles3-crash-on-samsung-galaxy-j5-after-launching-gfx-tests">1259525</a>)</p></li>
<li><p>Graphics: Removed postprocessing package from core packages list.</p></li>
<li><p>Graphics: Texture2D.Compress now compressed R8 textures to BC4 and R8G8 textures to BC5, on mobile platforms ETC/EAC are used.</p></li>
<li><p>Graphics: Updated postprocessing package to 3.1.0.</p></li>
<li><p>Graphics: VT-internal warnings no longer show up in the editor window, but still get printed into the editor log file.</p></li>
<li><p>HDRP: Avoids unnecessary RenderGraphBuilder.ReadTexture in the "Set Final Target" pass.</p></li>
<li><p>HDRP: Changed Path Tracing's maximum intensity from clamped (0 to 100) to positive value. (1310514)</p></li>
<li><p>HDRP: Changed some light unit slider value ranges to better reflect the lighting scenario.</p></li>
<li><p>HDRP: Changed the clamping approach for RTR and RTGI (in both perf and quality) to improve visual quality.</p></li>
<li><p>HDRP: Changed the convergence time of ssgi to 16 frames and the preset value.</p></li>
<li><p>HDRP: Changed the name from the Depth Buffer Thickness to Depth Tolerance for SSGI. (1301352)</p></li>
<li><p>HDRP: Changed the source value for the ray tracing frame index iterator from m_FrameCount to the camera frame count. (1301356)</p></li>
<li><p>HDRP: Changed the warning message for ray traced area shadows. (1303410)</p></li>
<li><p>HDRP: Disabled specular occlusion for what we consider medium and larger scale ao &gt; 1.25 with a 25cm falloff interval.</p></li>
<li><p>HDRP: Improved robustness of volumetric sampling in path tracing. (1295187)</p></li>
<li><p>HDRP: Removed backplate from rendering of lighting cubemap as it did not really work conceptually and caused artefacts.</p></li>
<li><p>HDRP: Removed the material pass probe volumes evaluation mode.</p></li>
<li><p>HDRP: The RTAO's history is now discarded if the occlusion caster was moving. (1303418)</p></li>
<li><p>HDRP: Tidy up of platform abstraction code for shader optimization.</p></li>
<li><p>HDRP: Transparent materials created by the Model Importer are set to not cast shadows.</p></li>
<li><p>HDRP: Unifying the history validation pass so that it is only done once for the whole frame and not per effect.</p></li>
<li><p>HDRP: Updated the tooltip for the Decal Angle Fade property (requires to enable Decal Layers in both HDRP asset and Frame settings). (1308048)</p></li>
<li><p>Mobile: Made session bugfixes for Adaptive Performance provider subsystem management.</p></li>
<li><p>Package: Added the Code Coverage package at version 1.0.0. This package helps you identify areas of your code that need more testing, even if you haven't written any automated tests.</p></li>
<li><p>Package: Storyboard Global Mute moved from Cinemachine menu to Cinemachine preferences.</p></li>
<li><p>Package: UI update - Moved Cinemachine menu to GameObject Create menu and Right Click context menu for Hierarchy.</p></li>
<li><p>Package: Updated com.unity.cinemachine to 2.7.2.</p></li>
<li><p>Package: Updated com.unity.purchasing version to 3.0.1.</p></li>
<li><p>Package: Updated FBX Exporter package to 4.0.1:<br> https://docs.unity3d.com/Packages/com.unity.formats.fbx@4.0/manual/index.html</p></li>
<li><p>Package Manager: The Package Manager no longer discards the existing package state in case of critical errors such as failure to parse the project manifest.</p></li>
<li><p>Scripting: AsyncReadManager.Read no longer writes the number of bytes read to the input ReadCommand array. The bytes read can now be accessed via the new ReadHandle.GetBytesRead method.</p></li>
<li><p>Scripting: Changed NativeArray limit of 2GiB in size, and now it can contain 2^31 items instead.</p></li>
<li><p>Scripting: Improved Roslyn analyzers that are inside assembly definition folders so that they apply to the asmdef assembly itself and to other assemblies that reference the asmdef assembly, but not to any other code in the project.</p></li>
<li><p>Scripting: Reintroduced a warning thrown when a script derived from MonoBehaviour has the same name as a built-in component (e.g. Transform).</p></li>
<li><p>Search: Removed the resource search provider (res:).</p></li>
<li><p>Shaders: Editor now skips warming up shaders from shader collections in the Preloaded shaders section of Graphics settings.</p></li>
<li><p>Shaders: Increased the global shader keyword limit to 384.</p></li>
<li><p>Shaders: Shader compiler logs are now generated in Logs folder instead of Library.</p></li>
<li><p>Timeline: Updated Timeline package to version 1.5.2</p></li>
<li><p>UI: Changed the license file based on legal requirements.</p></li>
<li><p>UI: Changed the Shader property for soft masking from _MaskSoftnessX / Y to _UIMaskSoftnessX / Y so we dont overlap with TMP's shader properties.</p></li>
<li><p>UI Toolkit: Allow :root pseudo selector to target the element receiving the style sheet.</p></li>
<li><p>UI Toolkit: Changed DynamicAtlas system to track texture references and support dynamic removals.</p></li>
<li><p>UI Toolkit: Changed the blending equation to allow blending of the resulting RenderTexture.</p></li>
<li><p>UI Toolkit: Improved renderer batching.</p></li>
<li><p>UI Toolkit: Mobile touch scrolling is now supported in scrollviews and listviews.</p></li>
<li><p>UI Toolkit: Text rendering is now handled by the textcore fontengine for both the editor and runtime.</p></li>
<li><p>UI Toolkit: Updated the menu item for Live Reload to be called "UI Toolkit Live Reload" to avoid user confusion.</p></li>
<li><p>VFX Graph: Tidy up of platform abstraction code for random number generation, requires a dependency on com.unity.render-pipelines.core for those abstractions.</p></li>
<li><p>XR: Updated com.unity.xr.legacyinputhelpers package to 2.1.6.</p></li>
<li><p>XR: Updated Oculus XR Plugin package to 1.7.0.</p></li>
<li><p>XR: Updated the ARCore, ARKit, ARKit Face Tracking, ARFoundation, ARSubsystems packages to 4.1.1.</p></li>
<li><p>XR: Updated the verified package versions for AR Foundation and related packages.</p></li>
<li><p>XR: Updated Windows XR Plugin package to 5.2.0.</p></li>
<li><p>XR: Updated XR Plug-in Management package to 3.2.17.</p></li>
</ul>

### Fixes
<ul>
<li><p>2D: Fixed dynamic batching of SpriteRenderers with TilemapRenderers in Individual Mode with the BaseMap shader property.</p></li>
<li><p>2D: Fixed exception when upgrading/downgrading packages used by Sprite Editor Window that is currently active. (<a href="https://issuetracker.unity3d.com/issues/2d-sprite-editor-window-to-turn-blank-along-with-exception-on-updating-2danimation-package-with-skinning-editor-selected">1242988</a>)</p></li>
<li><p>2D: Fixed Grid Selection outline when undoing a Grid Select action. (<a href="https://issuetracker.unity3d.com/issues/selection-area-in-the-tile-palette-window-stays-at-the-same-place-after-undoing">1275085</a>)</p></li>
<li><p>2D: Fixed IDE tooltip for Tilemap documentation. (<a href="https://issuetracker.unity3d.com/issues/tilemap-tilemap-dot-settile-method-documentation-in-the-ide-lacks-descriptive-information">1292596</a>)</p></li>
<li><p>2D: Fixed missing Sprite reference after loading scene from AssetBundles. (<a href="https://issuetracker.unity3d.com/issues/sprite-reference-missing-after-loading-scene-from-assetbundles">1274645</a>)</p></li>
<li><p>2D: Fixed null exception error when entering PlayMode with the Tile Palette window open and Inspector window open inspecting a GameObject. (<a href="https://issuetracker.unity3d.com/issues/error-is-thrown-when-entering-the-play-mode-while-inspector-and-tile-palette-are-opened-and-gameobject-with-grid-is-selected">1287664</a>)</p></li>
<li><p>2D: Fixed offset placement of Tile placed when dragging in a single Sprite or Tiles onto the Tile Palette window.</p></li>
<li><p>2D: Fixed Sprite Editor Window doesn't show the Sprite when the Inspector is locked and the Sprite is not selected in the Project window.</p></li>
<li><p>2D: Fixed Sprite is removed from Objects for Packing list of Sprite Atlas when using undo after replacing the Sprites. (<a href="https://issuetracker.unity3d.com/issues/sprite-is-removed-from-objects-for-packing-list-of-sprite-atlas-when-using-undo-after-swapping-the-sprites">1261537</a>)</p></li>
<li><p>2D: Fixed Sprite with no animation data is being processed during AssetPostProcessor.</p></li>
<li><p>2D: Made com.unity.2d.sprite and com.unity.2d.tilemap discoverable in Package Manager.</p></li>
<li><p>2D: Mark com.unity.2d.tilemap.extras as discoverable.</p></li>
<li><p>2D: Name Tiles based on Texture of Sprite when creating Tiles from nameless Sprites. (1281572)</p></li>
<li><p>2D: Order Tile Palette better when creating Tiles from a Sprite Texture when the size of Sprites are of multiples of each other. (<a href="https://issuetracker.unity3d.com/issues/tilepalette-tiles-are-not-ordered-in-the-palette-for-some-pre-sliced-textures">1281560</a>)</p></li>
<li><p>2D: Prevent Tile Palette Prefabs from showing as a Active Target for the Tile Palette window when selected.</p></li>
<li><p>2D: Store modified values of Grid Selection when asset/s are saved. (<a href="https://issuetracker.unity3d.com/issues/the-tile-palette-is-not-marked-as-dirty-and-changes-are-lost-after-editing-properties-of-a-tile-and-saving-the-scene">1287084</a>)</p></li>
<li><p>AI: Fixed editor crash when accessing null terrain tree meshes. (<a href="https://issuetracker.unity3d.com/issues/crash-on-calculatemeshbounds-when-baking-navmesh">1271682</a>)</p></li>
<li><p>Android: Added a warning if making a signed release Android build without Arm64 binaries. (1289652)</p></li>
<li><p>Android: Fixed a compilation error that occurred when using framebuffer fetch on single-channel texture formats. (<a href="https://issuetracker.unity3d.com/issues/urp-gles-shader-with-framebuffer-fetch-function-and-r8-unorm-color-format-rendertexture-fails-to-compile-on-android-build">1261534</a>)</p></li>
<li><p>Android: Fixed a crash that occurred when enabling/disabling camera access permission. (<a href="https://issuetracker.unity3d.com/issues/android-app-crashes-when-enabling-device-camera-permissions-for-the-app">1262468</a>)</p></li>
<li><p>Android: Fixed a mismatch between deltaTime and unscaledDeltaTime. (<a href="https://issuetracker.unity3d.com/issues/android-time-dot-unscaleddeltatime-does-not-match-time-dot-deltatime-when-timescale-is-1">1266965</a>)</p></li>
<li><p>Android: Fixed a problem with custom Aspect ratio value in manifest file. (<a href="https://issuetracker.unity3d.com/issues/android-build-fails-when-setting-a-custom-aspect-ratio-up-to-2-dot-1-in-player-settings">1284210</a>)</p></li>
<li><p>Android: Fixed an issue where the Build Settings window went black when SDK/build-tools were missing. (<a href="https://issuetracker.unity3d.com/issues/android-build-settings-window-goes-black-when-sdk-slash-build-tools-directory-is-empty">1230551</a>)</p></li>
<li><p>Android: Fixed crash when using UAV with Vulkan on older Mali devices. (<a href="https://issuetracker.unity3d.com/issues/android-crash-on-samsung-note8-while-running-gfx-tests">1256902</a>)</p></li>
<li><p>Android: Fixed issue where GL_EXT_shader_framebuffer_fetch wasn't added when fragment method is in an included file.</p></li>
<li><p>Android: Fixed wrong caret position inside InputField when quickly typing or deleting text. (<a href="https://issuetracker.unity3d.com/issues/android-input-field-caret-jumps-back-a-couple-of-characters-when-typing-fast">1252556</a>)</p></li>
<li><p>Android: Modified behavior to deselect ARM64 when switching to Mono, and restore when switching back to IL2CPP. (<a href="https://issuetracker.unity3d.com/issues/android-selecting-il2cpp-and-arm64-architecture-and-then-selecting-mono-leaves-the-arm64-architecture-checked-on">1281826</a>)</p></li>
<li><p>Android: Reduced the overhead of making the GetBigLittleConfiguration() call. (1285344)</p></li>
<li><p>Android: Removed gray banner that was displayed for projects built with -nographics enabled. (<a href="https://issuetracker.unity3d.com/issues/building-project-from-batchmode-with-nographics-flag-causes-icons-to-be-gray">1199310</a>)</p></li>
<li><p>Android: Updated Android Logcat package to version 1.2.1.</p></li>
<li><p>Android: Updated the Run Device tooltip on how to access the Preferences menu item. (<a href="https://issuetracker.unity3d.com/issues/android-macos-macos-tooltip-file-path-to-preferences-in-android-build-settings-is-incorrect">1213519</a>)</p></li>
<li><p>Android: When running Android SDK tool with elevated privileges use JDK bundled with Unity, previous behavior was the SDK tool would use java from PATH env variable, and would fail if there's no java installed and there's no java path set in PATH env variable. (<a href="https://issuetracker.unity3d.com/issues/android-windows-getting-unable-to-install-additional-sdk-when-java-is-not-installed-onto-windows-machine">1290206</a>)</p></li>
<li><p>Animation: Fixed an animation out of bounds issue. (1295247)</p></li>
<li><p>Animation: Fixed an issue where a humanoid mask did not correctly override during a transform. (<a href="https://issuetracker.unity3d.com/issues/avatar-mask-ignores-rm-when-both-humanoid-and-transform-masks-are-defined">1218558</a>)</p></li>
<li><p>Animation: Fixed an issue where an Animation clip with a length less than 0.05 seconds would not left align. (<a href="https://issuetracker.unity3d.com/issues/the-first-frame-in-the-animation-clips-timeline-is-not-aligned-to-the-left-when-clip-is-only-1-frame">1267304</a>)</p></li>
<li><p>Animation: Fixed an issue where Timeline window playback was disabled after unlinking the Animation window. (<a href="https://issuetracker.unity3d.com/issues/timeline-play-button-no-longer-works-after-leaving-aw-linked-state">1285659</a>)</p></li>
<li><p>Animation: Fixed an issue with culling mode when the renderer became visible. (1294699)</p></li>
<li><p>Animation: Fixed an issue with stepped animation evaluation. (1277195)</p></li>
<li><p>Animation: MeshFilter.mesh property is now animatable. (<a href="https://issuetracker.unity3d.com/issues/meshfilter-dot-mesh-property-should-be-animatable">1228956</a>)</p></li>
<li><p>Asset Bundles: Fixed main thread hitching when loading an AssetBundle asynchronously while loading other assets in the background.</p></li>
<li><p>Asset Import: Added Help box in the Model importer rig panel to inform about the state of QualitySettings.skinWeights when the Model importer skin weights value is higher. (<a href="https://issuetracker.unity3d.com/issues/warning-is-not-thrown-when-skin-weights-property-in-project-settings-overrides-skin-weights-property-in-import-settings">1194866</a>)</p></li>
<li><p>Asset Import: Fixed bug where renaming a script doesn't properly take effect on asset import workers.</p></li>
<li><p>Asset Import: Fixed corrupted PSD file could crash the Editor. (<a href="https://issuetracker.unity3d.com/issues/freeze-or-crash-with-various-stack-traces-when-importing-specific-psd-files">1284882</a>)</p></li>
<li><p>Asset Import: Fixed issue where embedded textures cannot be extracted from FBX files. (1307542)</p></li>
<li><p>Asset Import: Fixed issue where FBX and Sketchup files with paths longer than 260 characters cannot be imported on Windows.</p></li>
<li><p>Asset Import: Fixed issue where Reset does not apply to the 'Bake Axis conversion' setting in ModelImporter. (<a href="https://issuetracker.unity3d.com/issues/modelimport-reset-functionality-is-not-working-for-bake-axis-conversion-in-import-settings">1228920</a>)</p></li>
<li><p>Asset Import: Fixed OnOpenAsset callbacks ignoring callback order. (1297473)</p></li>
<li><p>Asset Import: Fixed such that Arguments are used as doubles rather than floats, allowing the FindGridCell method to have greater boundaries. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-gentangspace-when-importing-fbx-file">1280470</a>)</p></li>
<li><p>Asset Import: ModelImporter's remap Materials entries do not accept sub-assets materials anymore. (1243094)</p></li>
<li><p>Asset Import: Removed auto-alphabetization of items within a prefab. (<a href="https://issuetracker.unity3d.com/issues/the-object-hierarchy-is-not-preserved-when-objects-are-imported-using-scriptedimporter">1112123</a>)</p></li>
<li><p>Asset Pipeline: Added warning dialog before running out of disk space. Check is done on every refresh.</p></li>
<li><p>Asset Pipeline: Asset db file scanner will now error report files/folders that have a path or name that exceeded current limits. Path limit is 505/510 bytes (510 for meta file) and file name limit is 250/255 (255 for meta file). This fixes also an issue that would occur if a folder name was too long for getting a .meta counterpart. (<a href="https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-res-equals-equals-eagain-hasabortingerrors-when-importing-files-with-long-path">1280028</a>)</p></li>
<li><p>Asset Pipeline: Fixed for invalid artifact id assert that could get raised, when undo was restoring an object from a deleted asset. (<a href="https://issuetracker.unity3d.com/issues/tilemap-assertion-failed-exception-thrown-on-undo-action-after-removing-tilemap-and-tilemaprenderer-component">1254071</a>)</p></li>
<li><p>Asset Pipeline: Fixed issue when calling AssetDatabase.IsValidFolder() with a path that has a trailing slash at the end. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-isvalidfolder-returns-false-when-the-end-of-the-path-string-contains-a-directory-separator-slash">1153840</a>)</p></li>
<li><p>Asset Pipeline: Fixed shutdown discovered when reimporting all assets. (1274119)</p></li>
<li><p>Asset Pipeline: Fixed: changes made to Asset outside Unity are not applied during Play Mode when "Recompile After Finish Playing" is set in preferences. (<a href="https://issuetracker.unity3d.com/issues/changes-made-to-asset-outside-unity-are-not-applied-during-play-mode-when-recompile-after-finish-playing-is-set-in-preferences">1150790</a>)</p></li>
<li><p>Asset Pipeline: Logging in import worker will now always log to local import worker log file. (1286454)</p></li>
<li><p>Audio: Fixed an initialization issue on macOS that occurred when no audio input devices were available.</p></li>
<li><p>Audio: Fixed an issue in the Inspector window where the Wet slider did not immediately appear after selecting "Allow wet mixing" in the AudioGroup Strip View (1276039)</p></li>
<li><p>Audio: Fixed DSPGraph playback not being paused when the player was paused.</p></li>
<li><p>Bug Reporter: Bug Reporter throws an error if the project contains a shortcut to a path outside of the Assets folder. (<a href="https://issuetracker.unity3d.com/issues/bug-reporter-throws-an-error-if-the-project-contains-a-shortcut-to-a-path-outside-of-the-assets-folder">1160328</a>)</p></li>
<li><p>Bug Reporter: The Bug Reporter executable is now bundled with libssl 1.0.0 version. (<a href="https://issuetracker.unity3d.com/issues/bug-reporter-linux-2021-dot-1-bug-reporter-fails-to-open-when-using-ubuntu-20-dot-04">1293315</a>)</p></li>
<li><p>Build Pipeline: Fixed GlobalObjectIdGlobalObjectIdentifiersToObjectsSlow returning random objects when then GlobalObjectId references a non-existing object. (<a href="https://issuetracker.unity3d.com/issues/globalobjectidglobalobjectidentifierstoobjectsslow-sometimes-returns-a-random-existing-gameobject">1291291</a>)</p></li>
<li><p>Build Pipeline: StreamingAssets AssetBundle manifest is now provided by default to PlayerBuild, which will result in types being referred by AssetBundle being kept in the build even if Player.Optimization.Managed Stripping Level is set to Medium or High.</p></li>
<li><p>Build System: - Removed requirements over ILRepack when building Unity source code.<br></p> 
<ul>
<li>Removed requirements over ILRepack when building Unity source code.<br></li>
<li>Fixed ILRepack that was detected as Trojan:Win32/Wacatac.B!ml.<br></li>
<li>Removed ILRepack from external directory, now downloading ILRepack from our public stevedore repository.<br></li>
<li>You now have to explicitly call .\jam.pl BuildSystemProgramFiles to generate the solution for Unity Build System.</li>
</ul></li>
<li><p>Burst: ABI struct ret/by val for trivial aggregates for WASM is now respected.</p></li>
<li><p>Burst: Added PreserveAttribute to prevent the internal log from being stripped in il2cpp builds.</p></li>
<li><p>Burst: Allow to call <code>[BurstCompile]</code> functions from other <code>[BurstCompile]</code> functions.</p></li>
<li><p>Burst: Bitmask intrinsic was broken on non intel platforms.</p></li>
<li><p>Burst: Burst will now error if a <code>cpblk</code> was used to copy into a <code>[ReadOnly]</code> parameter or field.</p></li>
<li><p>Burst: Clang segmentation fault on iOS when member function debug information was emitted, it is disabled for this platform now.</p></li>
<li><p>Burst: Corrected 'Enable safety checks tooltip`.</p></li>
<li><p>Burst: Debug symbols are now output when using the native toolchain on mac.</p></li>
<li><p>Burst: Debug symbols for function names on some platforms are no longer hashes.</p></li>
<li><p>Burst: Dwarf symbols from multiple modules (e.g. multithreaded AOT compilation) now have correct compilation unit information.</p></li>
<li><p>Burst: Filter symbol warnings to prevent them reaching logs.</p></li>
<li><p>Burst: Fixed a bug that occurred when an explicitly laid out struct was used by a dup instruction, which caused an internal compiler error.</p></li>
<li><p>Burst: Fixed a bug where a <code>static readonly</code> variable that was a <code>System.Guid</code> would result in an internal compiler error.</p></li>
<li><p>Burst: Fixed a bug where a <code>stfld</code> into an element of a vector could deduce the wrong type for the underlying vector.</p></li>
<li><p>Burst: Fixed a bug where eager-compilation could pick up out-of-date global Burst menu options for compiling.</p></li>
<li><p>Burst: Fixed a bug where explicitly casting from an int to IntPtr would not sign extend the value.</p></li>
<li><p>Burst: Fixed a bug where if a user had defined multiple implicit or explicit casts, the compiler could resolve to the wrong cast.</p></li>
<li><p>Burst: Fixed a bug where if you used an enum argument to a function to index into a fixed array, a codegen error would occur.</p></li>
<li><p>Burst: Fixed a bug where loading from a vector within a struct, that was got from a NativeArray using an indexer, would cause the compiler to crash.</p></li>
<li><p>Burst: Fixed a bug where the Burst post-processing for direct call would cause duplicate function pointers to be compiled, wasting compile time in the editor and caused an Editor launch stall.</p></li>
<li><p>Burst: Fixed a bug where the mm256_cvtepi32_ps intrinsic would crash the compiler.</p></li>
<li><p>Burst: Fixed a bug where the progress bar would report double the amount of pending compile jobs if a user changed the Burst options while background compilation was going on.</p></li>
<li><p>Burst: Fixed a bug whereby for platforms that require us to write intermediate LLVM bitcode files, UTF paths would be incorrectly handled.</p></li>
<li><p>Burst: Fixed a bug with constant expressions that could cause a compile-time hang.</p></li>
<li><p>Burst: Fixed a bug with float/double vector constructors of <code>Unity.Mathematics</code> that take half or half vector parameters.</p></li>
<li><p>Burst: Fixed a poor error message when a generic unsupported type (like a class or an auto-layout struct) combined with an unsupported managed array (like (int, float)[]) wouldn't give the user any context on where the code went wrong.</p></li>
<li><p>Burst: Fixed a very obscure bug where if you had a function-pointer that was called from another function-pointer of job, and that function-pointer happened to be compiled in a player build in the same bucket as the caller, and the no-alias cloning analysis identified that it could clone the original function-pointer to enable more aliasing optimizations, it could create a duplicate symbol error.</p></li>
<li><p>Burst: Fixed alignment issues associated with xxHash3 on ArmV7 (case 1288992).</p></li>
<li><p>Burst: Fixed an internal compiler error when nested managed static readonly arrays were used (produces a proper Burst error instead now).</p></li>
<li><p>Burst: Fixed an issue that could prevent the Editor from shutting down.</p></li>
<li><p>Burst: Fixed an issue where Burst would erroneously error on BurstCompile.CompileFunctionPointer calls when building for the DOTS Runtime.</p></li>
<li><p>Burst: Fixed an issue where UNITY_DOTSPLAYER builds not building for NET_DOTS would be unable to compile do to references to UnityEngine.</p></li>
<li><p>Burst: Fixed compilation errors when targeting Arm CPUs and using some of the Intel intrinsics.</p></li>
<li><p>Burst: Fixed compilation errors when targeting Intel CPUs and using some of the Arm Neon intrinsics.</p></li>
<li><p>Burst: Fixed DOTS Runtime JobProducer Bursting code to support JobProducers with multiple generic arguments, complex job wrapper and generic jobs.</p></li>
<li><p>Burst: Fixed handling of conversion from signed integer to pointer which caused issues as discovered by Zuntatos on the forums.</p></li>
<li><p>Burst: Fixed incorrect struct layout for certain configurations of explicit-layout structs with overlapping fields.</p></li>
<li><p>Burst: Fixed Inspector slow down when scrolling/moving the window on large listings.</p></li>
<li><p>Burst: Fixed managed implementation of sub_ss intrinsic.</p></li>
<li><p>Burst: Fixed managed implementations of blend_epi32 and mm256_blend_epi32 intrinsics on Mono.</p></li>
<li><p>Burst: Fixed permissions error when running lipo tool to combine libraries.</p></li>
<li><p>Burst: Fixed potential error that could occur when unloading cached libraries.</p></li>
<li><p>Burst: Fixes a caching issue where stale cached libraries may have been used if a project was copied to a different folder, or Unity was upgraded to a newer version.</p></li>
<li><p>Burst: If targeting multiple iOS architectures, produce a combined burst library containing all architectures, this fixes "New Build System" on xcode version 12.</p></li>
<li><p>Burst: IL Function Pointer Invoke Transformation now uses correct runtime library for dots runtime.</p></li>
<li><p>Burst: IL Function Pointer Invoke Transformation updated to handle transforms that affect instructions that are the destination of a branch.</p></li>
<li><p>Burst: Intrinsics: Neon - fixed vget_low and vget_high producing suboptimal code.</p></li>
<li><p>Burst: Job Entry point symbols should now reflect the job name and type rather than a hash in callstacks/native profilers.</p></li>
<li><p>Burst: Job entry points without symbols now use the Execute location rather than pointing to unknown/unknown.</p></li>
<li><p>Burst: Multiple bugfixes (please look at https://docs.unity3d.com/Packages/com.unity.burst@1.5/changelog/CHANGELOG.html for a detailed list).</p></li>
<li><p>Burst: Private [BurstCompile] methods no longer throw MethodAccessException.</p></li>
<li><p>Burst: Sleef fallback to scalar float for WASM.</p></li>
<li><p>Burst: String interpolation issues when using Dots / Tiny runtime.</p></li>
<li><p>Burst: Strings can now be passed between methods.</p></li>
<li><p>Burst: We no longer attempt to replace the debug metadata multiple times for a given export.</p></li>
<li><p>Core: Fixed static analysis issue:<br> Non-static class member "isListening" is not initialized in this constructor nor in any functions that it calls.
(1291660)</p></li>
<li><p>Documentation: Updated the documentation to describe the design of OnApplicationFocus when using Play Mode in the Editor. (<a href="https://issuetracker.unity3d.com/issues/onapplicationfocus-sets-hasfocus-variable-to-true-and-instantly-to-false-when-focusing-on-the-editor-after-it-was-unfocused">1283510</a>)</p></li>
<li><p>DX12: Fixed a crash when executing a CommandBuffer that references a deleted RayTracingAccelerationStructure object.</p></li>
<li><p>DX12: Fixed a crash when RayTracingShader.Dispatch is called with an acceleration structure that was deleted in the meantime. (1281285)</p></li>
<li><p>DX12: Fixed potential crash in Debug builds when exiting Unity Editor when DX12 is used. (1309031)</p></li>
<li><p>Editor: Added a foolproof EditorGUIUtility.ResetGUIState(); when drawing Inspectors in the Override Preview panel. (<a href="https://issuetracker.unity3d.com/issues/vfx-visual-effect-text-overlaps-with-checkbox-in-prefab-override-window">1242693</a>)</p></li>
<li><p>Editor: Added a new flag called forceChildVisibiityfor the SerializedObject to control the visibility of hidden children. (<a href="https://issuetracker.unity3d.com/issues/drawing-serialized-properties-with-hideininspector-attribute-only-works-for-some-variable-types">1273848</a>)</p></li>
<li><p>Editor: Added padding to ReorderableList elements. (1281324)</p></li>
<li><p>Editor: Allow Hyphen character in Input Field when ContentType Property is set to Name. (<a href="https://issuetracker.unity3d.com/issues/hyphen-symbol-is-not-allowed-inside-the-inputfield-if-its-content-type-is-set-to-name">1270473</a>)</p></li>
<li><p>Editor: Checking and enabling VSync when Unmaximizing the Game view. (<a href="https://issuetracker.unity3d.com/issues/vsync-gets-disabled-in-the-game-view-when-maximizing-and-then-minimizing-the-game-view">1254640</a>)</p></li>
<li><p>Editor: Context menu shows in destination window in the Mac editor, regardless of whether the destination window is focused. (<a href="https://issuetracker.unity3d.com/issues/track-is-not-created-in-timeline-by-dragging-an-object-into-it-when-timeline-window-is-on-a-different-display-than-the-editor">1134774</a>)</p></li>
<li><p>Editor: Create Empty Parent' no longer relies on Scene View position.</p></li>
<li><p>Editor: Cursor is now locked to the center of the Game view in the Linux editor instead of the center of the screen when cursor lock is called in Play mode. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-cursor-placed-in-center-of-screen-after-unlock">1272190</a>)</p></li>
<li><p>Editor: Double-click on tab header maximizes/unmaximizes it. (1279177)</p></li>
<li><p>Editor: Dragging-and-dropping files across folders inside the Project Window will now prompt the user to choose what to do with a file when there are conflicting file names. (<a href="https://issuetracker.unity3d.com/issues/prompt-for-user-action-overwrite-rename-cancel-when-moving-files-in-project-view-and-destination-filename-already-exists">1210088</a>)</p></li>
<li><p>Editor: Fixed  issue where Terrain objects could still be selected despite picking being disabled. (<a href="https://issuetracker.unity3d.com/issues/terrain-objects-can-still-be-selected-when-their-selection-is-disabled">1251889</a>)</p></li>
<li><p>Editor: Fixed "Frame Selected" shortcut being invoked when Game View is focused and Play Mode is active, improving performance. (<a href="https://issuetracker.unity3d.com/issues/holding-the-f-key-shortcut-affects-the-performance-significantly-when-scene-view-is-hidden-and-the-game-view-is-opened">1252043</a>)</p></li>
<li><p>Editor: Fixed 'Toggle hidden packages visibility'  not affecting embedded/local packages. (<a href="https://issuetracker.unity3d.com/issues/embedded-slash-local-packages-that-are-set-to-always-hidden-are-still-shown-when-hidden-packages-visibility-is-toggled">1245277</a>)</p></li>
<li><p>Editor: Fixed -api-profile flag causing Editor to write to ProjectSettings/ProjectSettings.asset using binary serialization mode despite ForceText being configured in ProjectSettings/EditorSettings.asset.</p></li>
<li><p>Editor: Fixed a crash that could occur when Burst compilation was scheduled before Burst had been initialized.</p></li>
<li><p>Editor: Fixed a potential null reference exception in the Editor Tool Manager. (1251555)</p></li>
<li><p>Editor: Fixed a small issue with item position varying slightly in the Editor when display scaling is set to something other than 100%. (<a href="https://issuetracker.unity3d.com/issues/uir-certain-items-in-the-window-bounce-slash-flicker-when-resizing-the-window-and-the-display-scaling-is-set-to-125-percent-or-150-percent">1269754</a>)</p></li>
<li><p>Editor: Fixed a warning generated by undoing color change while picker is open. (<a href="https://issuetracker.unity3d.com/issues/hdrp-undo-color-change-while-picker-is-open-produces-a-warning">1262695</a>)</p></li>
<li><p>Editor: Fixed adding and removing components expanding collapsed components view in the Inspector window. (<a href="https://issuetracker.unity3d.com/issues/adding-slash-removing-components-expands-collapsed-components-view-in-the-inspector-window">1280892</a>)</p></li>
<li><p>Editor: Fixed an error where Slider1D was called with an invalid vector. (<a href="https://issuetracker.unity3d.com/issues/look-rotation-viewing-vector-is-zero-warnings-after-setting-spot-lights-range-to-0-in-srp">1284682</a>)</p></li>
<li><p>Editor: Fixed an issue causing incorrect display of redo operation when using GameObject.RegisterCreatedObjectUndo with a custom action name. (<a href="https://issuetracker.unity3d.com/issues/undoing-registercreatedobjectundo-always-changes-the-name-of-redo-to-create-object-instead-of-the-custom-name">1281435</a>)</p></li>
<li><p>Editor: Fixed an issue on Mac where open/save dialogs could not use copy/paste keyboard or menu shortcuts. (<a href="https://issuetracker.unity3d.com/issues/osx-cannot-paste-text-using-cmd-plus-v-when-naming-a-build">1252424</a>)</p></li>
<li><p>Editor: Fixed an issue to avoid "&lt;multi&gt;" string in the "Aniso Level" slider's value input field, in the Inspector, with multiple textures selected. (<a href="https://issuetracker.unity3d.com/issues/string-appears-in-the-aniso-level-sliders-value-input-field-in-the-inspector-with-multiple-textures-selected">1226069</a>)</p></li>
<li><p>Editor: Fixed an issue to avoid overlapping of Input fields and their labels in CustomRenderTextureEditor's Inspector if the Inspector is resized. (<a href="https://issuetracker.unity3d.com/issues/imgui-input-fields-of-properties-under-update-zones-are-overlapping-with-their-label-when-inspector-is-resized">1268481</a>)</p></li>
<li><p>Editor: Fixed an issue to avoid trimming of text in header, if header parameter contains line separator. (<a href="https://issuetracker.unity3d.com/issues/header-with-line-separator-symbol-parameter-is-cut-off-in-the-inspector">1269034</a>)</p></li>
<li><p>Editor: Fixed an issue to create Sorting Layers with the different names. (<a href="https://issuetracker.unity3d.com/issues/editor-sorting-layers-are-created-with-the-same-name-under-tag-and-layers-settings-from-project-settings-window">1268131</a>)</p></li>
<li><p>Editor: Fixed an issue to disable cut and copy in context when multiple objects are selected with different values. (<a href="https://issuetracker.unity3d.com/issues/context-menu-copying-and-cutting-is-allowed-for-different-value-fields-when-multi-selecting">1292164</a>)</p></li>
<li><p>Editor: Fixed an issue to set EnumFlagsField values properly while editing with multi-selected objects. (<a href="https://issuetracker.unity3d.com/issues/the-first-object-selected-dictates-what-flags-will-be-set-when-editing-multi-selected-objects-with-enumflagsfield-mixed-values">1282836</a>)</p></li>
<li><p>Editor: Fixed an issue to set static flag in inspector on 'Set to Value of X' in context menu . (<a href="https://issuetracker.unity3d.com/issues/inspectors-set-to-value-of-x-context-menu-fails-when-setting-bool-values">1221145</a>)</p></li>
<li><p>Editor: Fixed an issue where Account, Layer, and Layout buttons disappear when resizing the Editor beyond the width of the screen in MacOS. (<a href="https://issuetracker.unity3d.com/issues/imgui-account-layer-and-layout-buttons-get-disappears-when-resizing-the-editor">1254983</a>)</p></li>
<li><p>Editor: Fixed an issue where creating a Terrain material from a Terrain preset no longer causes a null reference access warning. (<a href="https://issuetracker.unity3d.com/issues/terrain-missingreferenceexception-thrown-on-creating-material-under-terrain-settings-in-preset-of-terrain">1240871</a>)</p></li>
<li><p>Editor: Fixed an issue where on Windows, when using the mouse in a Unity window, the wrong mouse position is used in other Unity windows. (<a href="https://issuetracker.unity3d.com/issues/2d-cell-selection-highlighter-appears-in-the-tilemap-on-editing-the-tile-palette">1275064</a>)</p></li>
<li><p>Editor: Fixed an issue where the default index doesn't filter prefabs using <code>t:prefab</code>. (1284865)</p></li>
<li><p>Editor: Fixed an issue where UnityEngine.Selection.objects should not return nulls. (1274421)</p></li>
<li><p>Editor: Fixed an issue where, after Play In Editor completed, settings were reset to default.</p></li>
<li><p>Editor: Fixed an issue with adding new tags and sorting layers in the Preset of 'Tags &amp; Layers'. (<a href="https://issuetracker.unity3d.com/issues/editor-new-tags-and-sorting-layers-are-not-created-and-added-in-the-list-of-preset-of-tags-and-layers">1268174</a>)</p></li>
<li><p>Editor: Fixed bad initial sync of search query. (<a href="https://issuetracker.unity3d.com/issues/search-sync-sends-wrong-initial-search-query">1296709</a>)</p></li>
<li><p>Editor: Fixed broken search for many types when attempting to assign assets to exposed property fields. (<a href="https://issuetracker.unity3d.com/issues/broken-search-for-many-types-mesh-texture-etc-dot-when-attempting-to-assigning-assets-to-exposed-property-fields">1307402</a>)</p></li>
<li><p>Editor: Fixed crash in GizmoUtilTests. (1274537)</p></li>
<li><p>Editor: Fixed CSharpCompiler.CompileAssemblyFromSource on Linux.</p></li>
<li><p>Editor: Fixed Custom font reset option not resetting all the values to their defaults. (<a href="https://issuetracker.unity3d.com/issues/imgui-reset-functionality-doesnt-work-for-custom-font-asset">1268319</a>)</p></li>
<li><p>Editor: Fixed doc and typo in Scene Template Pipeline. (<a href="https://issuetracker.unity3d.com/issues/fix-doc-and-typo-in-scene-templatepipeline">1286440</a>)</p></li>
<li><p>Editor: Fixed ETC Compression Legacy/Default that auto fills fast/normal settings. (<a href="https://issuetracker.unity3d.com/issues/etc-texture-compressor-editor-ui-does-not-work">1277170</a>)</p></li>
<li><p>Editor: Fixed expand/collapse icon settings when clicking on label. (<a href="https://issuetracker.unity3d.com/issues/mobile-notifications-mobile-notifications-settings-contents-are-not-responsive-to-resizing-of-right-and-bottom-borders">1195293</a>)</p></li>
<li><p>Editor: Fixed focused Inspector window tab is not updated when GameObject is renamed. (<a href="https://issuetracker.unity3d.com/issues/focused-inspector-window-tab-is-not-updated-when-gameobject-is-renamed">1285646</a>)</p></li>
<li><p>Editor: Fixed initial size of SafeMode when used for the first time. (1275799)</p></li>
<li><p>Editor: Fixed invisible asset created in the Project browser after renaming it with 260+ characters. (<a href="https://issuetracker.unity3d.com/issues/invisible-asset-is-created-in-ptoject-browser-when-create-a-material-with-260-plus-symbols-name">1281291</a>)</p></li>
<li><p>Editor: Fixed issue so preview Object names when selecting multiple assets are now displayed correctly. (<a href="https://issuetracker.unity3d.com/issues/inspector-preview-does-not-show-the-names-of-multiple-selected-files-when-they-are-in-the-same-format">1184882</a>)</p></li>
<li><p>Editor: Fixed issue so that correct prefab positioning in Hierarchy after undo and redo are called. (<a href="https://issuetracker.unity3d.com/issues/prefab-moves-one-position-down-in-hierarchy-window-when-pressing-redo">1268662</a>)</p></li>
<li><p>Editor: Fixed issue so that the camera inspector FOV slider now correctly adjusts its range when the FOV axis is horizontal. (<a href="https://issuetracker.unity3d.com/issues/imgui-slider-handle-of-field-of-view-disappears-on-selecting-horizontal-fov-axis-in-camera-properties">1219321</a>)</p></li>
<li><p>Editor: Fixed issue so that when app bundle identifier contains invalid chars (iOS/Android), they are removed with warning. (1183580)</p></li>
<li><p>Editor: Fixed issue so the green button on windows in MacOS now shows menu items correctly enabled when button is held. (<a href="https://issuetracker.unity3d.com/issues/tiling-menu-greyed-out-on-mac-editor-resize-button">1268232</a>)</p></li>
<li><p>Editor: Fixed issue to Handle Set/Clear As Active Parent Object action Undo correctly. (<a href="https://issuetracker.unity3d.com/issues/set-as-default-parent-is-not-considered-as-a-separate-action-when-undoing-slash-redoing">1275084</a>)</p></li>
<li><p>Editor: Fixed issue to restrict the access of CurrentViewWidth Property within OnGUI. (<a href="https://issuetracker.unity3d.com/issues/uielements-editorguiutility-dot-currentwidth-returns-0-when-using-it-in-a-visualelement">1289492</a>)</p></li>
<li><p>Editor: Fixed issue where changing Editor mode shows "Failed to load window layout". (1293093)</p></li>
<li><p>Editor: Fixed issue where custom cursor appears while hovering mouse on the Package Manager Window. (<a href="https://issuetracker.unity3d.com/issues/deployment-management-custom-cursor-appears-while-hovering-mouse-on-the-package-manager-window">1186485</a>)</p></li>
<li><p>Editor: Fixed issue where custom layout submenu item is showing when it should not (e.g. Window/Panels). (1265713)</p></li>
<li><p>Editor: Fixed issue where Handle null camera case in some of Handles functions, was producing a null reference exception when opening a ProBuilder UVEditor with a face selected. (<a href="https://issuetracker.unity3d.com/issues/probuilder-nullreferenceexception-and-argumentexception-errors-are-thrown-on-selecting-uv-editor-window">1242263</a>)</p></li>
<li><p>Editor: Fixed issue where Lightmap visualization tonemapping was not kept and used with Editor restarts. (<a href="https://issuetracker.unity3d.com/issues/lightmap-visualization-tonemapping-isnt-working-on-editor-start">1279800</a>)</p></li>
<li><p>Editor: Fixed issue where not all memory held by the Editor console was freed after it had been cleared. (<a href="https://issuetracker.unity3d.com/issues/logging-does-not-fully-clear-the-memory-used-once-the-console-is-cleared">1264725</a>)</p></li>
<li><p>Editor: Fixed issue where rectangle selection box sometimes did not select all vertices in the rectangle when editing a shape for Shadow Caster 2D. (<a href="https://issuetracker.unity3d.com/issues/rectangle-selection-box-sometimes-does-not-select-all-vertices-in-the-rectangle-when-editing-shape-for-shadow-caster-2d">1282153</a>)</p></li>
<li><p>Editor: Fixed LOD Group presets to not include references to renderers as these are related to Game Objects rather than project Assets. (<a href="https://issuetracker.unity3d.com/issues/assigning-a-preset-to-a-lodgroup-removes-reference-to-the-selected-renderer">1251159</a>)</p></li>
<li><p>Editor: Fixed modal window becoming non-interactable when creating a child modal window. (1215161)</p></li>
<li><p>Editor: Fixed not being able to delete array elements via keyboard 'Delete' key. (<a href="https://issuetracker.unity3d.com/issues/an-array-elements-content-is-not-deleted-when-selecting-the-element-in-the-inspector-window-and-pressing-del-key">1260899</a>)</p></li>
<li><p>Editor: Fixed organization refresh every tick. (1280142)</p></li>
<li><p>Editor: Fixed out of bounds errors when copying mesh renderer lists containing more renderers than the destination LOD Group in the Inspector. (<a href="https://issuetracker.unity3d.com/issues/inspector-breaks-when-copying-lodgroup-renderers-from-a-higher-renderer-count-group-to-a-smaller-one">1299768</a>)</p></li>
<li><p>Editor: Fixed ping highlight does not mark a folded child GameObject in the Hierarchy correctly when scrolling is required to reach the object. (<a href="https://issuetracker.unity3d.com/issues/ping-highlight-does-not-mark-a-folded-child-gameobject-in-the-hierarchy-correctly-when-scrolling-is-required-to-reach-the-object">1171103</a>)</p></li>
<li><p>Editor: Fixed Play and Pause button toggle icons not loading the correct "On" state when entering Play mode.</p></li>
<li><p>Editor: Fixed Player Settings Reset not clearing some icons for Android and iOS. (<a href="https://issuetracker.unity3d.com/issues/mobile-resetting-the-player-settings-does-not-reset-icons-to-default-empty-values">1263065</a>)</p></li>
<li><p>Editor: Fixed player settings visual glitch, "Metal API Validation" check box having an extra indentation level.</p></li>
<li><p>Editor: Fixed PropertyEditor callback issue which prevented PropertyEditor from being deallocated.</p></li>
<li><p>Editor: Fixed rare crash when several Editors are opened.</p></li>
<li><p>Editor: Fixed ReorderableList having wrong label/field width ratio.</p></li>
<li><p>Editor: Fixed ReorderableList incorrectly looping element selection when using arrow up or arrow down keys. (<a href="https://issuetracker.unity3d.com/issues/array-selection-cycling-using-the-arrow-key-shortcuts-is-inconsistent">1305527</a>)</p></li>
<li><p>Editor: Fixed ReorderableList sometimes reordering items when the user is multi-selecting elements. (<a href="https://issuetracker.unity3d.com/issues/clicking-on-array-elements-while-holding-the-control-key-shifts-the-array-order">1299784</a>)</p></li>
<li><p>Editor: Fixed restoration of static EditorGUI fields in case of exception during rendering of audio mixer effect inspector. (1232339)</p></li>
<li><p>Editor: Fixed Search index incremental update progress sometime never finishes. (1292594)</p></li>
<li><p>Editor: Fixed spacing in warning message when attempting to attach a debugger to the Editor. (1254306)</p></li>
<li><p>Editor: Fixed status bar's progress bar not refreshing correctly when progress finishes. (<a href="https://issuetracker.unity3d.com/issues/updating-assets-search-index-progress-bar-doesnt-disappear-when-assets-are-imported-and-process-is-finished">1310102</a>)</p></li>
<li><p>Editor: Fixed the issue where AddComponentMenu could have folders with no name. (<a href="https://issuetracker.unity3d.com/issues/probuilder-probuilder-meshfilter-list-headings-are-missing-on-clicking-add-component">1259764</a>)</p></li>
<li><p>Editor: Fixed the issue where Game Object name could be set to empty string when changed in Inspector window. (<a href="https://issuetracker.unity3d.com/issues/a-gameobject-with-no-name-is-created-when-its-name-is-deleted-in-the-inspector">1169191</a>)</p></li>
<li><p>Editor: Fixed the issue where Game View focus is lost when entering Play mode with maximized Game View. (<a href="https://issuetracker.unity3d.com/issues/game-view-focus-is-lost-when-entering-play-mode-with-maximized-game-view-either-by-shift-plus-space-or-options-maximize">1252097</a>)</p></li>
<li><p>Editor: Fixed the issue with Editor mode defaulting to Normal after restart. (<a href="https://issuetracker.unity3d.com/issues/inspector-mode-defaults-to-normal-after-editor-restart">1156788</a>)</p></li>
<li><p>Editor: Fixed the issue with Slider Component using an image for its Fill Rect field not marking the image's Fill Amount property as driven. (<a href="https://issuetracker.unity3d.com/issues/slider-component-using-an-image-for-its-fill-rect-field-does-not-properly-mark-the-images-fill-amount-property-as-driven">1264829</a>)</p></li>
<li><p>Editor: Fixed the issue with space between rectangles drawn using GUILayout. (<a href="https://issuetracker.unity3d.com/issues/rectangles-that-are-drawn-by-guilayout-dot-window-have-spacings-in-between-when-method-is-called-in-editor-window">1282874</a>)</p></li>
<li><p>Editor: Fixed the Package-related MenuItem issue. (<a href="https://issuetracker.unity3d.com/issues/2d-unable-to-use-ui-components-when-the-unity-ui-package-is-removed-and-added-again-in-the-package-manager">1233571</a>)</p></li>
<li><p>Editor: Fixed the title issue with a tooltip. Since the name of the texture you have selected is already there where you clicked, a tooltip is sufficient showing the full name if it is not being fully visible due to size constraint. (<a href="https://issuetracker.unity3d.com/issues/graphics-title-of-texture-preview-in-frame-debugger-overlaps-on-texture-property-data">1248621</a>)</p></li>
<li><p>Editor: Fixed the Unity crash handler on Windows to use the active project of the Editor from which it spawned when creating bug reports. (<a href="https://issuetracker.unity3d.com/issues/bug-reporter-includes-project-files-of-the-last-project-opened-instead-of-the-project-that-crashed">1246875</a>)</p></li>
<li><p>Editor: Fixed Tools.ViewTool returning ViewTool.Pan when not in GUI context. (<a href="https://issuetracker.unity3d.com/issues/tools-dot-viewtool-always-returns-viewtool-dot-pan">1165779</a>)</p></li>
<li><p>Editor: Fixed <code>Arrow Left</code> and <code>Arrow Right</code> keys not collapsing and expanding array elements. (<a href="https://issuetracker.unity3d.com/issues/the-items-of-reorderable-list-are-not-expanded-slash-collapsed-when-using-right-slash-left-arrow-keys">1281321</a>)</p></li>
<li><p>Editor: Improved default Hierarchy search engine's performance. (1313691)</p></li>
<li><p>Editor: Improved the performance of the model importer when dealing with degenerate triangles. (<a href="https://issuetracker.unity3d.com/issues/unity-editor-freezes-when-importing-a-specific-fbx-file">1232201</a>)</p></li>
<li><p>Editor: Last selected console log entry now stays active after search filter is removed. (1264776)</p></li>
<li><p>Editor: On Windows, LTS builds of the Editor will now each have their own entry in Add/Remove programs. (<a href="https://issuetracker.unity3d.com/issues/final-release-versions-are-not-listed-separately-in-programs-and-features-list-of-applications-in-the-system">1267038</a>)</p></li>
<li><p>Editor: Optimized rendering of TreeView when it has a large selection set.</p></li>
<li><p>Editor: Reduced unnecessary Game view repaint during LOD crossfade animations.</p></li>
<li><p>Editor: Resolve errors when opening Player Settings from Build Settings. (<a href="https://issuetracker.unity3d.com/issues/ubuntu-opening-player-settings-spams-console-with-error-messages">1291443</a>)</p></li>
<li><p>Editor: Reverted changes regarding DS-1131.</p></li>
<li><p>Editor: Roslyn analyzer rulesets are now correctly applied for script compilations that happen very early during Editor startup. (1273682)</p></li>
<li><p>Editor: Scene/Game view gizmo fadeout is less aggressive now, and can be user controlled via "Fade Gizmos" slider in Gizmos window. (<a href="https://issuetracker.unity3d.com/issues/wire-gizmos-not-visible-from-a-distance">1274317</a>)</p></li>
<li><p>Editor: String, Integer, Float, Character and BoundsInt type SerializedProperties now have Copy/Paste context menu options.</p></li>
<li><p>Editor: The input package now correctly calculates mouse deltas when the cursor is locked under Linux. (<a href="https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked">1248389</a>)</p></li>
<li><p>Editor: The Windows standalone uninstaller now correctly cleans up all files and removes the install directory. (<a href="https://issuetracker.unity3d.com/issues/installer-standalone-windows-editor-installer-does-not-clean-up-completely">1277752</a>)</p></li>
<li><p>Editor: Transform component inspector context menu is better organized now (Copy/Paste/Reset items under their own submenus). (1264870)</p></li>
<li><p>Editor: Update GUI.Color to reflect that it is not affected in personal addition. (<a href="https://issuetracker.unity3d.com/issues/gui-dot-color-not-applied-when-using-personal-theme">1273117</a>)</p></li>
<li><p>Editor: Updated sync icon. (1296453)</p></li>
<li><p>Editor: Updated the EULA for Mac installers. (1274616)</p></li>
<li><p>Editor: Use Search Default Search engine for new project. (1296465)</p></li>
<li><p>GI: Cookies on baked point lights now respect light rotation. (<a href="https://issuetracker.unity3d.com/issues/rotation-of-baked-point-light-with-a-cookie-ignored-when-baking-lightmap">1289490</a>)</p></li>
<li><p>GI: Fixed a bug so that the Clear Baked data control now resets the ambient probe and default reflection probe fields. (<a href="https://issuetracker.unity3d.com/issues/gi-clearing-bake-data-does-not-sync-to-game-view-or-scene-view-immediately">1200802</a>)</p></li>
<li><p>GI: Fixed a Static Analysis Defect 53772 in EnlightenJobHelpers.h which passed a tainted expression "sz" to "resize", which uses it as an allocation size. (1290400)</p></li>
<li><p>GI: Fixed HDR reflection probe baking when the Editor is in mobile platform mode with 11.11.10 HDR format active. (1280354)</p></li>
<li><p>GI: Scene objects the user deletes and restores now retain their lightmaps. (<a href="https://issuetracker.unity3d.com/issues/the-lightmaps-are-not-restored-after-removing-baked-gameobject-and-undoing">1225425</a>)</p></li>
<li><p>GI: The Auto Generate control is now accessible from every tab of the Lighting Window. (<a href="https://issuetracker.unity3d.com/issues/in-lighting-window-auto-generate-toggle-disappears-when-going-into-a-non-scene-tab">1266957</a>)</p></li>
<li><p>GI: The Editor now selects the correct GPU for eGPU baking. (1274223)</p></li>
<li><p>GI: The GPU Lightmapper is now compatible with the Apple Silicon DTK.</p></li>
<li><p>GI: The Radeon Pro denoiser now introduces fewer artifacts in HDR lightmaps. (<a href="https://issuetracker.unity3d.com/issues/plm-radeon-pro-denoiser-produces-artifacts">1272945</a>)</p></li>
<li><p>GI: The Unity Editor no longer returns erroneous error messages about GPU driver issues when the user's GPU does not have enough memory to support the GPU Lightmapper. (<a href="https://issuetracker.unity3d.com/issues/plm-opencl-errors-appear-in-the-console-when-attempting-to-generate-lighting-using-plm">1289660</a>)</p></li>
<li><p>GI: Users can now animate indirect bounce intensity. (<a href="https://issuetracker.unity3d.com/issues/some-light-properties-are-not-animatable">1278770</a>)</p></li>
<li><p>GI: While the Editor is rendering cubemaps, it now backs up and restores built in parameters. (<a href="https://issuetracker.unity3d.com/issues/shaders-that-use-lightcolor0-dot-rgb-flicker-to-black-in-game-view-when-reflection-probes-are-updated-in-realtime">1242415</a>)</p></li>
<li><p>Graphics: Added a space in the Tier list UI in Graphic Settings. (1259327)</p></li>
<li><p>Graphics: Added backbuffer MSAA support to OSX/Game View. (1289045)</p></li>
<li><p>Graphics: Added exposure slider to the inspector of HDR RenderTextures (excl 3D) &amp; 2D/2DArray textures. (1225327)</p></li>
<li><p>Graphics: Added missing script API taking GraphicsBuffer parameters, for SetBufferCounterValue and SetBufferData.</p></li>
<li><p>Graphics: Added support for CreateExternalTexture with the Vulkan API.</p></li>
<li><p>Graphics: Added SupportsRandomWriteOnRenderTextureFormat to query if a given RenderTextureFormat can be used when enabling the random write flag. (<a href="https://issuetracker.unity3d.com/issues/some-textures-are-not-created-when-their-formats-are-shown-as-supported-by-systeminfo-dot-supportsrendertextureformat">1266102</a>)</p></li>
<li><p>Graphics: Added the support of a custom shader editor per render pipeline with the CustomEditorForRenderPipeline ShaderLab keyword allowing to fix HDRP and URP material editor issues. (<a href="https://issuetracker.unity3d.com/issues/cant-edit-material-with-a-cross-pipeline-shader">1276432</a>)</p></li>
<li><p>Graphics: Adding Chinese pure dynamic font characters causes atlas memory leak of about 0.5mb each. (<a href="https://issuetracker.unity3d.com/issues/vulkan-tmpro-adding-chinese-pure-dynamic-font-characters-causes-atlas-memory-leak-of-about-0-dot-5mb-each">1273364</a>)</p></li>
<li><p>Graphics: Backporting fix for Metal bug where multiple render targets that share a blend state can have an incorrect write mask. (1296917)</p></li>
<li><p>Graphics: Clarifies and simplifies the texture resource views within the Xcode GPU frame debugger. (1281175)</p></li>
<li><p>Graphics: Corrected list of formats supported by Virtual Texturing.</p></li>
<li><p>Graphics: Correctly referenced the postprocessing package from the package manager. (<a href="https://issuetracker.unity3d.com/issues/post-processing-3-dot-0-3-package-cant-be-found-when-installing-from-package-manager">1317088</a>)</p></li>
<li><p>Graphics: CPU optimisation for graphics memory allocation/deallocations.</p></li>
<li><p>Graphics: Dirty prefab when dirtying a material used by that prefab. (1282291)</p></li>
<li><p>Graphics: Extended supported formats for GPU readback. (1123748)</p></li>
<li><p>Graphics: Fixed a casting issue when assigning an int to a bool with HLSLcc.</p></li>
<li><p>Graphics: Fixed a depth buffer size check when implicit backbuffer depth is used. Removed error message. (<a href="https://issuetracker.unity3d.com/issues/urp-an-error-is-spammed-in-a-build-when-using-2d-light-with-the-use-normal-map-option-enabled">1268201</a>)</p></li>
<li><p>Graphics: Fixed ALL/NONE to maintain the state on the Volume Component Editors.</p></li>
<li><p>Graphics: Fixed an issue where high numbers of materials would slow down unloading of Asset Bundles containing shaders. (<a href="https://issuetracker.unity3d.com/issues/unloading-an-assetbundle-that-contains-a-material-causes-a-call-to-findobjectsoftype">935529</a>)</p></li>
<li><p>Graphics: Fixed case 1086548 (RenderToCubemap offsets shadows when the material on the mesh has GPU Instancing enabled), by adding support for STEREO_CUBEMAP_RENDER_ON for instanced rendering. (<a href="https://issuetracker.unity3d.com/issues/rendertocubemap-offsets-shadows-when-the-material-on-the-mesh-has-gpu-instancing-enabled">1086548</a>)</p></li>
<li><p>Graphics: Fixed case 1266922.</p></li>
<li><p>Graphics: Fixed crash on VolumeComponentWithQualityEditor when the current Pipeline is not HDRP.</p></li>
<li><p>Graphics: Fixed custom shaders with no explicit Pass defined to respect the "receive shadows" flag. (<a href="https://issuetracker.unity3d.com/issues/shader-does-not-collect-proper-shadow-information-when-using-shadow-attenuation-macro">1050091</a>)</p></li>
<li><p>Graphics: Fixed drop of VisualEffectAsset within a prefab. (<a href="https://issuetracker.unity3d.com/issues/prefab-cannot-add-a-vfx-graph-inside-a-prefab">1285794</a>)</p></li>
<li><p>Graphics: Fixed erroneous assertion after calling Object.DestroyImmediate on a rendertarget that was just unbound. (<a href="https://issuetracker.unity3d.com/issues/gfxframebuffergles-an-active-rendertargetsetup-has-dangling-pointers-dot-is-thrown-when-entering-play-mode-in-opengl">1270401</a>)</p></li>
<li><p>Graphics: Fixed erroneous precision when deducing the precision of a sampler from a texture and using inline state. (<a href="https://issuetracker.unity3d.com/issues/using-an-inline-sampler-causes-metal-shader-to-have-extra-half-float-casts">1271276</a>)</p></li>
<li><p>Graphics: Fixed for setScissorRect crashing on metal when adjusting panels in editor. (<a href="https://issuetracker.unity3d.com/issues/setscissorrect-crashes-on-metal-when-adjusting-panels-in-editor">1256241</a>)</p></li>
<li><p>Graphics: Fixed FrameTimingManager produced incorrect frame time on Vulkan and DirectX12. (<a href="https://issuetracker.unity3d.com/issues/frametimingmanager-dot-getlatesttimings-returns-a-smaller-gpuframetime-than-it-actually-is">1274505</a>)</p></li>
<li><p>Graphics: Fixed gradient sampling in Fixed mode. (<a href="https://issuetracker.unity3d.com/issues/fixed-gradient-colors-are-blended-when-time-is-interpolated-using-random-number-node">1212002</a>)</p></li>
<li><p>Graphics: Fixed inconsistency issue where some meshes would be dynamically batched in editor but not in standalone player. (<a href="https://issuetracker.unity3d.com/issues/mobile-dynamic-batching-is-not-working-when-working-with-sub-mesh-on-a-mobile-device">1278480</a>)</p></li>
<li><p>Graphics: Fixed incorrect GeometryJob Fence initialisation causing graphical corruption in UI canvas rendering.</p></li>
<li><p>Graphics: Fixed issue on Metal-MacOS Standalone where HDR enabled Don't Clear and Depth Only cameras would clear the background (rendering the empty texture). (<a href="https://issuetracker.unity3d.com/issues/metal-player-rendering-breaks-when-a-second-non-fullscreen-camera-is-enabled">1184769</a>)</p></li>
<li><p>Graphics: Fixed issue where changing from fullscreen to windowed mode causes black screen on Linux when using OpenGL. (<a href="https://issuetracker.unity3d.com/issues/black-screen-after-switching-from-fullscreen-to-windowed-on-a-linux-build">1314460</a>)</p></li>
<li><p>Graphics: Fixed issue where passing a null value to GetBlendShapeIndex function on Mesh class would cause the editor to crash. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-getchannelindex-when-passing-null-to-mesh-dot-getblendshapeindex">1288012</a>)</p></li>
<li><p>Graphics: Fixed Metal error when creating pipeline state if number of shader components is less than render target pixel format. (1242218)</p></li>
<li><p>Graphics: Fixed missing support for coarse/fine derivatives in shader code.</p></li>
<li><p>Graphics: Fixed missing support for mip tails in sparse textures on Vulkan. (1265578)</p></li>
<li><p>Graphics: Fixed missing warning UI about Projector component being unsupported. (1300327)</p></li>
<li><p>Graphics: Fixed OpenGL bug where projection matrix was not correctly restored after calling Graphics.DrawMeshNow and GL.PopMatrix. (<a href="https://issuetracker.unity3d.com/issues/ios-projection-matrix-gets-corrupted">1262117</a>)</p></li>
<li><p>Graphics: Fixed potential divide by 0 when running graphics jobs on UWP Player.</p></li>
<li><p>Graphics: Fixed Prefab Inspector preview (Editor) adding Renderer components into existing RayTracingAccelerationStructures while the Inspector preview is visible. (<a href="https://issuetracker.unity3d.com/issues/dxr-a-raytracingaccelerationstructure-using-automatic-management-mode-will-also-include-the-mesh-in-prefab-inspector">1297799</a>)</p></li>
<li><p>Graphics: Fixed repaint of VFX Graph in play mode.</p></li>
<li><p>Graphics: Fixed sample mesh skinned (vfx) when GPUSkinning is disabled. (1275889)</p></li>
<li><p>Graphics: Fixed Shader.globalRenderPipeline tag is not being set correctly at runtime. (1141848)</p></li>
<li><p>Graphics: Fixed shadow maps in frame debugger. (<a href="https://issuetracker.unity3d.com/issues/game-view-is-black-when-using-frame-debugger-in-render-main-shadowmap">1278463</a>)</p></li>
<li><p>Graphics: Fixed shadowmask behavior for terrain trees that have LODs. (1285466)</p></li>
<li><p>Graphics: Fixed situation where Hybrid Renderer could throw errors because of invalid reflection data.</p></li>
<li><p>Graphics: Fixed spacing between property fields on the Volume Component Editors.</p></li>
<li><p>Graphics: Fixed stateful case where ComputeShader could be put in a bad state internally if user forgot to bind out buffer. Required Editor restart to get rid of previously.</p></li>
<li><p>Graphics: Fixed terrain material being reset to builtin terrain material after reopening an SRP project.</p></li>
<li><p>Graphics: Fixed the default background color for previews to use the original color.</p></li>
<li><p>Graphics: Fixed the default background color for previews to use the original color.</p></li>
<li><p>Graphics: Fixed the display name of a Volume Parameter when is defined the attribute InspectorName.</p></li>
<li><p>Graphics: Fixed the selection of the Additional properties from ALL/NONE when the option "Show additional properties" is disabled.</p></li>
<li><p>Graphics: Fixed Validation error from creating 0 size frame buffers on Vulkan. (1278091)</p></li>
<li><p>Graphics: Fixed Vulkan validation error Shader requires vertexPipelineStoresAndAtomics but is not enabled on the device. (1288889)</p></li>
<li><p>Graphics: Fixed Vulkan Validation warnings when fragment shader input is not produced for render pass attachment. (1278088)</p></li>
<li><p>Graphics: Fixed [VFX] HUP regressions introduced by editor repaint optimizations. (<a href="https://issuetracker.unity3d.com/issues/camera-command-list-issues-leading-to-broken-gpu-sorting-and-mesh-lods">1293323</a>)</p></li>
<li><p>Graphics: Fixes NullReferenceException on Terrain Shaders when project is opened after deleting Library folder. (<a href="https://issuetracker.unity3d.com/issues/urp-nullreferenceexception-on-terrain-shaders-when-project-is-opened-after-deleting-library-folder">1240491</a>)</p></li>
<li><p>Graphics: Fixes reflections in baked reflection probes not being rendered when rendering path is set to deferred. (<a href="https://issuetracker.unity3d.com/issues/reflection-probe-bounces-dont-work-when-rendering-path-is-set-to-deferred">1260144</a>)</p></li>
<li><p>Graphics: Fixes vulkan validation error VUID-VkFramebufferCreateInfo-pAttachments-00882. (1278684)</p></li>
<li><p>Graphics: Frame Debugger does not show formats of MRT (multiple render targets) correctly. (1261622)</p></li>
<li><p>Graphics: Handle depthSlice -1 for backbuffer when using OpenGL ES. (1281747)</p></li>
<li><p>Graphics: Keep it possible to create textures using deprecated ASTC enums. (<a href="https://issuetracker.unity3d.com/issues/ios-unable-to-create-texture2ds-with-astc-rgba-4x4-texture-format-at-runtime">1277203</a>)</p></li>
<li><p>Graphics: Made accessing buffer dimensions an error when compiling for metal. (1274166)</p></li>
<li><p>Graphics: Make it clear that some Line Renderer Inspector options are for Scene View editing, and do not belong to the Line Renderer instance. (<a href="https://issuetracker.unity3d.com/issues/improved-prefabs-blue-highlight-is-missing-for-simplify-preview-and-tolerance-fields-in-line-renderer-prefab">1199217</a>)</p></li>
<li><p>Graphics: Nodes using camera buffers (depth or color) from the main camera will use the buffers from the scene camera when the main camera is not rendered. (1256861)</p></li>
<li><p>Graphics: Prevent ability for users to incorrectly pick a scene object when picking a detail mesh prefab. (1270627)</p></li>
<li><p>Graphics: Prevent drag and drop of Material, Shader, Texture on a GameObject with VFXRenderer. (<a href="https://issuetracker.unity3d.com/issues/vfx-graph-material-can-be-dragged-and-dropped-onto-vfx-graph-asset-in-scene-with-lit-mesh-output">1251051</a>)</p></li>
<li><p>Graphics: Removed parent hiearchy keeping world transform in sceneView for VisualEffect. (<a href="https://issuetracker.unity3d.com/issues/when-a-vfx-asset-is-dragged-and-dropped-on-a-gameobject-it-is-parented-to-it-instead-of-being-created-as-a-new-gameobject">1288444</a>)</p></li>
<li><p>Graphics: Restore all settings on LODGroup to defaults when Reset. (1254015)</p></li>
<li><p>Graphics: Sample Mesh - Color store as float. (1229974)</p></li>
<li><p>Graphics: Small bugfixes in the texture mipmap streamer.</p></li>
<li><p>Graphics: Standalone Server Build forces Gfx Threading Mode Direct.</p></li>
<li><p>Graphics: Terrain asset presets no longer include instance data. This corrects the intended behavior, and significantly improves performance. (<a href="https://issuetracker.unity3d.com/issues/application-dot-processwindowsmessage-loading-window-is-displayed-when-closing-select-preset-window-of-a-terrain">1244214</a>)</p></li>
<li><p>Graphics: Terrain no longer has artifacts on some iOS devices when using Anisotropic Textures and Instancing. (<a href="https://issuetracker.unity3d.com/issues/ios-metal-opengles3-terrain-is-rendered-with-artifacts-on-ios-devices-when-using-anisotropic-textures">1103084</a>)</p></li>
<li><p>Graphics: The Post-processing package has been updated to version 3.0.1.</p></li>
<li><p>Graphics: Updated SRP packages to 10.2.0.</p></li>
<li><p>Graphics: Updated terrain warning against using shaders that rely on tangents to recommend the correct shaders for SRPs. (<a href="https://issuetracker.unity3d.com/issues/terrain-inspector-is-proposing-a-shader-which-isnt-there">1281595</a>)</p></li>
<li><p>Graphics: Warn user for rendering artifacts when importing texture with cubemap sequence/cross layout with non-optimal size. (<a href="https://issuetracker.unity3d.com/issues/in-the-cubemap-preview-incorrect-dimensions-are-shown-when-the-cubemap-texture-has-wrong-resolution">1163002</a>)</p></li>
<li><p>Graphics: When blitting textures with multiple slices, all slices are now blit across the source and destination. (<a href="https://issuetracker.unity3d.com/issues/texture2darrays-blit-source-destination-is-not-copying-the-entire-texture-source-to-destination">1211291</a>)</p></li>
<li><p>GraphView: Added capability support to stacks, stack children, and groups to help better avoid unsupported behaviors. Specifically with grouping and heterogeneous selections.</p></li>
<li><p>HDRP: Fixed a locale issue with the diffusion profile property values in ShaderGraph on PC where comma is the decimal separator.</p></li>
<li><p>HDRP: Fixed a reload bug when using objects from the scene in the lookdev. (1300916)</p></li>
<li><p>HDRP: Fixed ability to override AlphaToMask FrameSetting while camera in deferred lit shader mode.</p></li>
<li><p>HDRP: Fixed after post process custom pass scale issue when dynamic resolution is enabled. (<a href="https://issuetracker.unity3d.com/issues/viewport-is-incorrect-in-a-custom-pass-running-in-afterpostprocess-when-using-dynamic-resolution">1299194</a>)</p></li>
<li><p>HDRP: Fixed alpha output in debug view and AOVs when using shadow matte. (<a href="https://issuetracker.unity3d.com/issues/unrecognized-identifier-error-is-thrown-when-hdrp-slash-unlit-shadow-matte-is-enabled-and-common-material-properties-is-set-to-alpha">1311830</a>)</p></li>
<li><p>HDRP: Fixed an exception when opening the color picker in the material UI. (<a href="https://issuetracker.unity3d.com/issues/hdrp-unityengine-dot-exitguiexception-error-is-thrown-on-opening-color-palette-window-in-the-material-inspector">1307143</a>)</p></li>
<li><p>HDRP: Fixed an issue in shadergraph when switch from a RenderingPass. (<a href="https://issuetracker.unity3d.com/issues/shader-graph-graph-settings-window-gets-blank-with-argumentexception-on-changing-the-material-value-to-lit-in-hdrp-settings">1307653</a>)</p></li>
<li><p>HDRP: Fixed an issue in the planar reflection probe convolution.</p></li>
<li><p>HDRP: Fixed an issue where first frame of SSAO could exhibit ghosting artefacts.</p></li>
<li><p>HDRP: Fixed an issue where selection in a debug panel would reset when cycling through enum items.</p></li>
<li><p>HDRP: Fixed an issue with half res ssgi upscale.</p></li>
<li><p>HDRP: Fixed an issue with light intensity prefab override application not visible in the inspector. (<a href="https://issuetracker.unity3d.com/issues/hdrp-apply-to-prefab-option-is-missing-when-pressing-on-the-light-component-intensity-propertys-label-on-a-prefab">1299563</a>)</p></li>
<li><p>HDRP: Fixed an issue with material using distortion from ShaderGraph init after Material creation. (<a href="https://issuetracker.unity3d.com/issues/shader-has-different-effects-depending-on-whether-the-material-was-created-by-selecting-the-shader-or-applying-it-afterwards">1294026</a>)</p></li>
<li><p>HDRP: Fixed an issue with the capture callback (now includes post processing results).</p></li>
<li><p>HDRP: Fixed an issue with the frame count management for the volumetric fog. (1299251)</p></li>
<li><p>HDRP: Fixed an issue with the mipmap generation internal format after rendering format change.</p></li>
<li><p>HDRP: Fixed an issue with transparent meshes writing their depths and recursive rendering. (1314409)</p></li>
<li><p>HDRP: Fixed box light attenuation.</p></li>
<li><p>HDRP: Fixed Clearcoat on Stacklit or Lit breaks when URP is imported into the project. (1297806)</p></li>
<li><p>HDRP: Fixed decal draw order for ShaderGraph decal materials.</p></li>
<li><p>HDRP: Fixed decal normal for double sided materials. (1312065)</p></li>
<li><p>HDRP: Fixed decals in material debug display.</p></li>
<li><p>HDRP: Fixed Emissive color property from Autodesk Interactive materials not editable in Inspector. (<a href="https://issuetracker.unity3d.com/issues/materials-emissive-color-cannot-be-changed-when-the-material-is-using-hdrp-autodesk-interactive-shaders">1307234</a>)</p></li>
<li><p>HDRP: Fixed error in Depth Of Field near radius blur calculation. (1306228)</p></li>
<li><p>HDRP: Fixed error in the RTHandle scale of Depth Of Field when TAA is enabled.</p></li>
<li><p>HDRP: Fixed error when opening the default composition graph in the Graphics Compositor. (1318933)</p></li>
<li><p>HDRP: Fixed GC allocations from XR occlusion mesh when using multipass.</p></li>
<li><p>HDRP: Fixed incorrect debug wireframe overlay on tessellated geometry (using littessellation), caused by the picking pass using an incorrect camera matrix.</p></li>
<li><p>HDRP: Fixed issue of accessing default frame setting stored in current HDRPAsset instead fo the default HDRPAsset.</p></li>
<li><p>HDRP: Fixed issue when debug full screen 'Transparent Screen Space Reflection' do not take in consideration debug exposure.</p></li>
<li><p>HDRP: Fixed issue with automatic exposure settings not updating scene view.</p></li>
<li><p>HDRP: Fixed issue with compositor custom pass hooks added/removed repeatedly. (1315971)</p></li>
<li><p>HDRP: Fixed issue with compositor related custom passes still active after disabling the compositor. (1305330)</p></li>
<li><p>HDRP: Fixed issue with Depth of Field CoC debug view.</p></li>
<li><p>HDRP: Fixed issue with physically-based DoF computation and transparent materials with depth-writes ON.</p></li>
<li><p>HDRP: Fixed issue with shadow mask and area lights.</p></li>
<li><p>HDRP: Fixed issue with velocity rejection in post-DoF TAA. Fixing this reduces ghosting. (1304381)</p></li>
<li><p>HDRP: Fixed issues with compositor's undo. (<a href="https://issuetracker.unity3d.com/issues/hdrp-graphics-compositor-editor-crashes-on-doing-undo-operation-after-adding-image-sublayer-in-render-schedule">1305633</a>)</p></li>
<li><p>HDRP: Fixed issues with path-traced volumetric scattering. (1295222, 1295234)</p></li>
<li><p>HDRP: Fixed label style in pbr sky editor.</p></li>
<li><p>HDRP: Fixed LayerMask editor for volume parameters.</p></li>
<li><p>HDRP: Fixed light gizmo showing shadow near plane when shadows are disabled.</p></li>
<li><p>HDRP: Fixed light layer issue when performing editing on multiple lights.</p></li>
<li><p>HDRP: Fixed lights shadow frustum near and far planes.</p></li>
<li><p>HDRP: Fixed LookDev environment library assignement after leaving playmode.</p></li>
<li><p>HDRP: Fixed loss of persistency of ratio between pivot position and size when sliding by 0 in DecalProjector inspector. (1308338)</p></li>
<li><p>HDRP: Fixed material keywords with fbx importer.</p></li>
<li><p>HDRP: Fixed missing BeginCameraRendering call for custom render mode of a Camera.</p></li>
<li><p>HDRP: Fixed missing option to use POM on emissive for tessellated shaders.</p></li>
<li><p>HDRP: Fixed model import by adding additional data if needed.</p></li>
<li><p>HDRP: Fixed multiple HDRP Frame Settings panel issues: missing "Refraction" Frame Setting. Fixing ordering of Rough Distortion, it should now be under the Distortion setting.</p></li>
<li><p>HDRP: Fixed nullref in layered lit shader editor.</p></li>
<li><p>HDRP: Fixed nullref when adding a volume component in a Volume profile asset. (<a href="https://issuetracker.unity3d.com/issues/hdrp-nullreference-error-when-adding-any-override-to-a-volume">1317156</a>)</p></li>
<li><p>HDRP: Fixed path tracing alpha channel support. (1304187)</p></li>
<li><p>HDRP: Fixed PCSS filtering issues with cached shadow maps.</p></li>
<li><p>HDRP: Fixed performance issue with ShaderGraph and Alpha Test.</p></li>
<li><p>HDRP: Fixed register spilling on  FXC in light list shaders.</p></li>
<li><p>HDRP: Fixed resize IES when already baked in the Atlas. (<a href="https://issuetracker.unity3d.com/issues/hdrp-ies-profile-breaks-point-light-after-increasing-resolution-past-1024">1299233</a>)</p></li>
<li><p>HDRP: Fixed Rough Distortion frame setting not greyed out when Distortion is disabled in HDRP Asset.</p></li>
<li><p>HDRP: Fixed screen being over-exposed when changing very different skies.</p></li>
<li><p>HDRP: Fixed shadow matte not working with ambient occlusion when MSAA is enabled.</p></li>
<li><p>HDRP: Fixed side effect on styles during compositor rendering.</p></li>
<li><p>HDRP: Fixed size and spacing of compositor info boxes. (<a href="https://issuetracker.unity3d.com/issues/imgui-hdrp-base-layer-aovs-property-warning-text-is-clipped-in-graphics-compositor-window">1305652</a>)</p></li>
<li><p>HDRP: Fixed skybox for ortho cameras.</p></li>
<li><p>HDRP: Fixed some render texture leaks.</p></li>
<li><p>HDRP: Fixed spacing of UI widgets in the Graphics Compositor. (<a href="https://issuetracker.unity3d.com/issues/hdrp-graphics-compositor-color-palette-alpha-line-changes-its-position-on-changing-the-chroma-keying-index-in-input-filters">1305638</a>)</p></li>
<li><p>HDRP: Fixed SSGI frame setting not greyed out while SSGI is disabled in HDRP Asset.</p></li>
<li><p>HDRP: Fixed StackLit ShaderGraph surface option property block to only display energy conserving specular color option for the specular parametrization. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-hdrp-transmission-and-energy-conserving-specular-color-should-appear-only-in-their-respective-modes">1257050</a>)</p></li>
<li><p>HDRP: Fixed sub-shadow rendering for cached shadow maps.</p></li>
<li><p>HDRP: Fixed the condition on temporal accumulation in the reflection denoiser. (1303504)</p></li>
<li><p>HDRP: Fixed the default background color for previews to use the original color.</p></li>
<li><p>HDRP: Fixed timing issues with accumulation motion blur.</p></li>
<li><p>HDRP: Fixed undo-redo on layered lit editor.</p></li>
<li><p>HDRP: Fixed Undo/Redo instability of light temperature.</p></li>
<li><p>HDRP: Fixed update upon light movement for directional light rotation.</p></li>
<li><p>HDRP: Fixed various issues with non-temporal SSAO and rendergraph.</p></li>
<li><p>HDRP: Fixed Warnings about "SceneIdMap" missing script in eye material sample scene.</p></li>
<li><p>HDRP: Fixed white flashes on camera cuts on volumetric fog.</p></li>
<li><p>HDRP: Fixed wizard checking FrameSettings not in HDRP Default Settings.</p></li>
<li><p>HDRP: Fixed wrong shader / properties assignement to materials created from 3DsMax 2021 Physical Material. (<a href="https://issuetracker.unity3d.com/issues/hdrp-importing-a-model-with-a-3ds-max-physical-material-assign-an-incorrect-shader-and-does-not-apply-its-textures">1293576</a>)</p></li>
<li><p>HDRP: Fixed XR depth copy when using MSAA.</p></li>
<li><p>HDRP: Fixed: SSR with transparent. (<a href="https://issuetracker.unity3d.com/issues/hdrp-prb-accumulation-does-not-work-when-ssr-for-transparents-is-enabled">1311088</a>)</p></li>
<li><p>IL2CPP: Correctly report the public key for assemblies where is exists.</p></li>
<li><p>IL2CPP: Fixed issue with generated Visual Studio Solution project files that caused IntelliSense and other code analysis tools to fail when scanning source files. (1285102)</p></li>
<li><p>IMGUI: Https://jira.unity3d.com/browse/UIT-191: The rect transform rectangle visual is too light.</p></li>
<li><p>IMGUI: Updated Layers drop down icon positions and images. (1184677)</p></li>
<li><p>iOS: Fixed a crash when going to background from portrait upside down on some devices. (<a href="https://issuetracker.unity3d.com/issues/ios-app-is-crashing-when-it-is-switched-out-of-focus-and-focused-again-while-it-is-in-reverse-portrait">1285042</a>)</p></li>
<li><p>iOS: Fixed application not rendering when using a very high Application.targetFrameRate.</p></li>
<li><p>iOS: Fixed xcode12 picking "generic" target by default, resulting in "build and run" not running app. (<a href="https://issuetracker.unity3d.com/issues/ios-xcode12-build-and-run-generates-an-xcodeproj-project-but-does-not-build-or-run-it-when-using-xcode-12">1279315</a>)</p></li>
<li><p>iOS: Generated Xcode project does not use MapFileParser. (<a href="https://issuetracker.unity3d.com/issues/ios-mapfileparser-dot-sh-permission-denied-when-building-xcode-project-built-from-windows-directly-to-a-macos-shared-folder">1071993</a>)</p></li>
<li><p>iOS: Removed prohibited API usage.</p></li>
<li><p>Kernel: Fixed enter playmode regression when there are many outstanding Burst jobs to compile.</p></li>
<li><p>License: Fixed broken login during batchmode license activation. (1294709)</p></li>
<li><p>License: Fixed serverDirectory in license server configuration file.</p></li>
<li><p>Linux: Added check for return value of write to avoid failure (1228164)</p></li>
<li><p>Linux: Fixed a bug where unplugging/plugging in controllers would lead to a bad input device tracking state. (1279308)</p></li>
<li><p>Linux: Fixed an incorrect assert message on disconnecting a game controller. (1279323)</p></li>
<li><p>Linux: Fixed an issue where the Linux Downloader would not properly extract files.</p></li>
<li><p>Linux: Fixed the Bug Reporter suggestion box. (<a href="https://issuetracker.unity3d.com/issues/linux-bugreporter-suggestion-box-never-updates">1156930</a>)</p></li>
<li><p>Linux: Fixed tooltips are not resized correctly when shown consecutively one after another. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-tooltips-appear-in-the-same-loaction-and-of-the-same-size-as-the-first-one-if-shown-consecutively-one-after-another">1279878</a>)</p></li>
<li><p>Linux: Fixed Unity Bug Reporter taskbar icon on Ubuntu LTS showing "unknown". (<a href="https://issuetracker.unity3d.com/issues/linux-unity-bug-reporter-taskbar-icon-description-says-unknown">1188799</a>)</p></li>
<li><p>Linux: Re-enable CanAllocateALotOfMemory test. (1111793)</p></li>
<li><p>Linux: Show error if Linux Mono support is not installed. (<a href="https://issuetracker.unity3d.com/issues/linux-player-builds-with-mono-scripting-backend-fails-with-a-confusing-error-message-if-only-il2cpp-players-are-installed">1276232</a>)</p></li>
<li><p>Linux: Updated from SDL 2.0.7 to 2.0.12.</p></li>
<li><p>macOS: Added a semaphore to break out of the editor's idle loop when a tick is signaled. (1281419)</p></li>
<li><p>macOS: Added logging to Thread shutdown to help determine possible broken threads, as well as potential fix for HID thread not properly shutting down when exiting.</p></li>
<li><p>macOS: Application is correctly focussed and unfocussed when the GameCenter UI is used.</p></li>
<li><p>macOS: Eyedropper now works on multiple screens. (<a href="https://issuetracker.unity3d.com/issues/color-is-not-sourced-with-the-color-picker-tool-when-choosing-it-from-an-editor-window-on-another-monitor">1278129</a>)</p></li>
<li><p>macOS: Fixed a hang between Burst's usage of the background task UI reporting and the Editor. (1308530)</p></li>
<li><p>macOS: Fixed an issue where a unitypackage created on another filesystem might fail to import. (<a href="https://issuetracker.unity3d.com/issues/macos-failed-to-import-package-with-error-couldnt-decompress-package-is-thrown-when-importing-a-specific-unitypackage">1266321</a>)</p></li>
<li><p>macOS: Fixed aux window remains active when a tab is moved. (<a href="https://issuetracker.unity3d.com/issues/scene-view-scene-draw-mode-menu-remains-active-even-if-the-scene-window-moved-aside">1265583</a>)</p></li>
<li><p>macOS: Fixed crash when trying to access Movies, Music, or Photos folders on Catalina. (<a href="https://issuetracker.unity3d.com/issues/macos-crash-on-abort-with-payload-when-trying-to-import-an-asset-from-photos-movies-or-music">1280375</a>)</p></li>
<li><p>macOS: Fixed improper layout of the Inspector when making the Editor full screen. (<a href="https://issuetracker.unity3d.com/issues/macos-bottom-part-of-the-inspector-is-hidden-when-entering-fullscreen-mode-in-the-editor">1283862</a>)</p></li>
<li><p>macOS: Fixed improper layout of the Package Manager Window when making the Editor full screen. (<a href="https://issuetracker.unity3d.com/issues/package-manager-package-manager-window-does-not-become-fullscreen-when-maximized">1278245</a>)</p></li>
<li><p>macOS: Report shader compiler error when invalid texture samplers are used in Metal shaders. (<a href="https://issuetracker.unity3d.com/issues/macos-no-error-is-thrown-on-metal-graphics-api-when-shader-texture-slash-sampler-is-mismatched">1214014</a>)</p></li>
<li><p>macOS: Target directory has to be selected instead of target .xcodeproj when building MacOS Xcode Project.</p></li>
<li><p>Mobile: Fixed iOS plugin compile flags not updating on build append. (<a href="https://issuetracker.unity3d.com/issues/ios-plugin-compile-flags-do-not-update-on-append-build">1254117</a>)</p></li>
<li><p>Mobile: Ignore touch events in DeviceSimulator in notches and cutouts. (<a href="https://issuetracker.unity3d.com/issues/devicesimulator-the-input-is-detected-when-clicking-on-notch">1295407</a>)</p></li>
<li><p>Mobile: Updated the provider icon and info text to be displayed correctly.</p></li>
<li><p>Multiplayer: Fixed out of bounds access error when doing connection checks in unet.</p></li>
<li><p>Multiplayer: Resolved an issue where you can now set the threadpool size for LL API.</p></li>
<li><p>Package: Error message when loading new scene with DontDestroyOnLoad. (<a href="https://issuetracker.unity3d.com/issues/cinemachine-throws-an-argumentoutofrange-exception-when-destroying-a-camera-with-dontdestroyonload">1283984</a>)</p></li>
<li><p>Package: Fixed bug that causes searcher window to be offset too far when accounting for host window boundaries.</p></li>
<li><p>Package: Fixed edge-case exception when vcam is deleted. (1284701)</p></li>
<li><p>Package: Lens inspector sometimes displayed ortho vs perspective incorrectly for a brief time. (<a href="https://issuetracker.unity3d.com/issues/cinemachine-camera-randomly-changes-lens-parameter-from-orthographic-size-to-field-of-view-when-duplicated">1060230</a>)</p></li>
<li><p>Package: Removed unnecessary allocations and garbage collections during runtime.</p></li>
<li><p>Package: Visual Scripting: Dropdown icon is not clipped with TextField under "Get Variable".</p></li>
<li><p>Package: Visual Scripting: Fixed "Restore to Defaults" buttons in the Project Settings window.</p></li>
<li><p>Package: Visual Scripting: Fixed an error when executing "Fix Missing Scripts" in a HDRP project.</p></li>
<li><p>Package: Visual Scripting: Fixed console errors when deleting a Prefab with a Visual Script.</p></li>
<li><p>Package: Visual Scripting: Fixed console errors when editing nested graphs during Play Mode.</p></li>
<li><p>Package: Visual Scripting: Fixed error message when custom inspectors are generated.</p></li>
<li><p>Package: Visual Scripting: Fixed Graph getting corrupted when adding "Get Action Map" unit.</p></li>
<li><p>Package: Visual Scripting: Fixed Node description being sometimes clipped.</p></li>
<li><p>Package: Visual Scripting: Fixed the object Variables tabs not being updated when creating a Prefab.</p></li>
<li><p>Package: Visual Scripting: Fixed ThreadAbortException when entering Play Mode while searching in the Fuzzy Finder.</p></li>
<li><p>Package: Visual Scripting: Fixed warnings overflow in the console when deleting and adding a boolean variable in the blackboard.</p></li>
<li><p>Package: Visual Scripting: Fixed warnings when entering play mode when the "Script Changes While Playing" is set to Recompile And Continue Playing.</p></li>
<li><p>Package: Visual Scripting: FlowMachine type is now back in usable types.</p></li>
<li><p>Package: Visual Scripting: Fuzzy finder no longer blinks when trying to add a node [BOLT-1157](https://issuetracker.unity3d.com/product/unity/issues/guid/BOLT-1157),.</p></li>
<li><p>Package: Visual Scripting: Fuzzy finder search window no longer remains above all other windows [BOLT-1197](https://issuetracker.unity3d.com/product/unity/issues/guid/BOLT-1197)";;;;;;;;;.</p></li>
<li><p>Package: Visual Scripting: Fuzzy search no longer drops keyboard inputs and respond slowly [BOLT-1214](https://issuetracker.unity3d.com/product/unity/issues/guid/BOLT-1214),.</p></li>
<li><p>Package: Visual Scripting: GraphPointerException occurs when nesting graph within itself [BOLT-1257](https://issuetracker.unity3d.com/issues/visual-scripting-graphpointerexception-occurs-when-nesting-<br> graph-within-itself).</p></li>
<li><p>Package: Visual Scripting: Help button in the visual scripting Assets and Behaviours inspector now links to the package documentation.</p></li>
<li><p>Package: Visual Scripting: Missing succession for Cooldown. Output of Cooldown completed is treated as unentered.  [BOLT-725](https://issuetracker.unity3d.com/issues/bolt-1-output-of-cooldown-completed-<br> is-treated-as-unentered).</p></li>
<li><p>Package: Visual Scripting: Opening the graph window no longer causes Unity UI stop processing mouse click [BOLT-1159](https://issuetracker.unity3d.com/product/unity/issues/guid/BOLT-1159),.</p></li>
<li><p>Package: Visual Scripting: RenamedFrom attribute does not function correctly on array references to a renamed type [BOLT-1149](https://issuetracker.unity3d.com/product/unity/issues/guid/BOLT-1149).</p></li>
<li><p>Package: Visual Scripting: Rendering of inactive ObjectFields.</p></li>
<li><p>Package: Visual Scripting: Resize cursor rect on group when graph window is zoomed.</p></li>
<li><p>Package: Visual Scripting: ScalarAdd unit migration from 1.4.13 to 1.4.14 and above.</p></li>
<li><p>Package: Visual Scripting: Scale groups when zoom is not at 1x.</p></li>
<li><p>Package: Visual Scripting: Sidebar (graph inspector/blackboard) resize when a vertical scrollbar is needed.</p></li>
<li><p>Package: Visual Scripting: Variable type reset to Enum when changing from Enum to GameObject when both Blackbaord and Variables inspector are displayed.</p></li>
<li><p>Package: Visual Scripting: Visual Scripting Preferences being searchable [BOLT-1218](https://issuetracker.unity3d.com/issues/visual-scripting-preferences-are-not-searchable-when-using-search-in-the-preferences-window).</p></li>
<li><p>Package: Visual Scripting: Visual Scripting Preferences spacing has been adjusted to avoid overlaps.</p></li>
<li><p>Package: Visual Scripting: VisualScripting.Generated folder is removed when removing the VisualScripting package.</p></li>
<li><p>Package Manager: Changed the Package Manager window to open to the first package with an entitlement error after displaying a warning where the user selects <em>Continue</em>.</p></li>
<li><p>Package Manager: Fixed an issue in the Package Manager window where a package's status icon was being offset and wasn't aligning with other icons when its name was too long. (1287317)</p></li>
<li><p>Package Manager: Fixed an issue in the Package Manager window where the Packages view tab shrinks even though there is plenty of space to display the complete text.</p></li>
<li><p>Package Manager: Fixed an issue on the Package Manager window where the package items weren't aligning properly. (1307752)</p></li>
<li><p>Package Manager: Fixed an issue where <em>See All Versions</em> from the project settings was affecting package discovery in the <em>My Registries</em> context. (1284861)</p></li>
<li><p>Package Manager: Fixed an issue where removing packages with read-only files was throwing an <code>UnauthorizedAccessException</code> if the package was in the Packages directory (Git clone). (<a href="https://issuetracker.unity3d.com/issues/package-manager-removing-package-with-a-read-only-file-throws-unauthorizedaccessexception-if-package-is-in-packages-directory">1237777</a>)</p></li>
<li><p>Package Manager: Fixed an issue where the Package Manager was not recognizing new package names from the Asset Store.</p></li>
<li><p>Package Manager: Fixed an issue where the Package Manager wasn't applying changes in the project manifest when <code>autorefresh</code> was disabled. (1292471)</p></li>
<li><p>Package Manager: Fixed an issue where the Package Manager wasn't performing the search query using the specified text whenever the user would manually refresh a list.</p></li>
<li><p>Package Manager: Fixed an issue which was preventing the Unity Package Manager from starting on Linux under specific circumstances.</p></li>
<li><p>Package Manager: Fixed an issue which was preventing the Unity Package Manager from starting on Windows 7. (<a href="https://issuetracker.unity3d.com/issues/package-manager-doesnt-start-anymore-on-windows-7">1298330</a>)</p></li>
<li><p>Package Manager: Fixed issues with Samples display when switching between low width and regular width view.</p></li>
<li><p>Package Manager: Fixed the issue where new versions of a package weren't appearing after a refresh in the <em>In Project</em> tab. (1281125)</p></li>
<li><p>Package Manager: Fixed the issue where the <em>Add from git URL</em> textbox was not shrinking properly in the Package Manager window.</p></li>
<li><p>Package Manager: Fixed the issue where the advanced settings were not persisting in the project.</p></li>
<li><p>Package Manager: Fixed the issue where the package names in dependencies weren't matching either the display name or the name of the package.</p></li>
<li><p>Package Manager: Fixed the null ref exception that was occurring when a user would switch accounts and the Package Manager would try to display any new assets in the package list.</p></li>
<li><p>Package Manager: Fixed the sample display name error messages when the package was not in development and the Package Manager window was set to the lowest width.</p></li>
<li><p>Package Manager: Improved the performance of accessing <code>HiddenPackagesCount</code> in <code>PackageManagerUtilityInternal</code>. (1275248)</p></li>
<li><p>Package Manager: Release Candidate packages are no longer tagged as 'Release Candidate (RC)'. Alpha and beta versions no longer display packages appear with the "Pre-release" tag unless the <em>Enable Pre-release</em> setting is enabled.</p></li>
<li><p>Package Manager: Removed the Package Manager error messages that were getting logged twice. (1283355)</p></li>
<li><p>Package Manager: The <em>Preview Packages in Use</em> behavior now conforms to Lifecycle V2. (1284843)</p></li>
<li><p>Package Manager: The Package Manager now adds an ellipsis when the package name, version or tag is truncated. (1284866)</p></li>
<li><p>Package Manager: The Package Manager now automatically selects the first added scoped registry when opening project settings from the popup.</p></li>
<li><p>Package Manager: The Package Manager now tags scoped registry packages in the details pane according to the version tag.</p></li>
<li><p>Particles: Added shortcuts for Resimulate, Show Bounds and Show only Selected. (1268064)</p></li>
<li><p>Particles: Ensure smooth size updates when doing slow-mo scrubbing of the particle playback time. (<a href="https://issuetracker.unity3d.com/issues/mesh-particle-system-update-frequency-is-too-low-and-causes-visible-stutters-when-adjusting-with-playback-time-slider">1224857</a>)</p></li>
<li><p>Particles: Fixed crash when using BakeTrails with <code>Attach Ribbons to Transform</code>.</p></li>
<li><p>Particles: Fixed emit from script bug when emitting particles from LateUpdate during Edit Mode. (<a href="https://issuetracker.unity3d.com/issues/shuriken-emitparams-getting-overwritten-with-empty-values-when-using-emit-in-editmode">1283939</a>)</p></li>
<li><p>Particles: Fixed ParticleSystem Window throwing an error when Undo was performed after creating a sub-system. (<a href="https://issuetracker.unity3d.com/issues/shuriken-errors-on-undo-operation-after-creating-partcle-effect-from-particle-editor-window">1280126</a>)</p></li>
<li><p>Particles: Remove the warning about mis-matched vertex streams when creating a default Particle System. (1259366)</p></li>
<li><p>Physics: CCD type is restored to specified Collision Detection type in Rigidbody Inspector when isKinematic is toggled from true to false. Inspector does not show speculative CCD in use during kinematic override. There are no warnings that this is occurring. (<a href="https://issuetracker.unity3d.com/issues/rigidbody-collision-detection-mode-cannot-be-updated-after-setting-the-iskinematic-field-to-true-then-false-during-runtime">1177698</a>)</p></li>
<li><p>Physics: Display Linear and Angular damping in the root of the ArticulationBody.</p></li>
<li><p>Physics: Fixed crashes/instabilities of physics simulation for ArticulationBody component hierarchy modifications during the runtime.</p></li>
<li><p>Physics: Fixed internal issues happening when a joint connected a rigidbody to an inactive articulation body. (<a href="https://issuetracker.unity3d.com/issues/error-message-is-thrown-when-referencing-an-inactive-articulationbody-from-a-joint">1293798</a>)</p></li>
<li><p>Physics: Fixed Physics Debug window section titles to be clickable for dropdown. (<a href="https://issuetracker.unity3d.com/issues/physics-dropdown-doesnt-expand-on-clicking-its-title-under-physics-debugger-window">1261353</a>)</p></li>
<li><p>Physics: Fixed the kinematic flag not being not being applied correctly when off and when there were concave meshes attached. (<a href="https://issuetracker.unity3d.com/issues/errors-on-enabling-slash-disabling-is-kinematic-if-convex-is-unchecked-on-a-mesh">1299855</a>)</p></li>
<li><p>Physics: Physics Collider Tooltips were revised. (<a href="https://issuetracker.unity3d.com/issues/physics-tooltips-are-missing-for-the-properties-under-collider-component">1261350</a>)</p></li>
<li><p>Physics: When using the Physics Debugger, GameView and SceneView gizmo highlights are now synced. (1285340)</p></li>
<li><p>Playables: Fixed an issue where an Assertion would occur if you evaluated a PlayableDirector in OnEnable for a MonoBehaviour with the ExecuteInEditMode Attribute. (<a href="https://issuetracker.unity3d.com/issues/assembly-cache-should-be-empty-appears-in-the-console-when-evaluating-a-timeline-during-onenable">1246997</a>)</p></li>
<li><p>Plugins: Removed console exceptions for Magic Leap. (1252217)</p></li>
<li><p>Prefabs: Added missing tooltips for Revert and Apply buttons in Prefab overrides comparison view. (<a href="https://issuetracker.unity3d.com/issues/improved-prefab-tooltips-are-missing-for-apply-and-revert-buttons-in-the-override-window">1261334</a>)</p></li>
<li><p>Prefabs: Fixed crash when exiting Prefab mode in some circumstances. (1269978)</p></li>
<li><p>Prefabs: Fixed Prefab preview in Inspector doesn't update until reselected. (<a href="https://issuetracker.unity3d.com/issues/improved-prefabs-prefab-preview-in-inspector-doesnt-update-until-reselected">1056071</a>)</p></li>
<li><p>Prefabs: Fixed so deleting the context parent in Prefab Mode in Context is prevented from the UI. (<a href="https://issuetracker.unity3d.com/issues/deleting-the-dummy-parent-in-prefab-mode-in-context-should-be-prevented-from-the-ui">1291699</a>)</p></li>
<li><p>Prefabs: Fixed that there is no information provided about the Prefab when a Prefab's child has broken references after using ForceReserializeAssets. (<a href="https://issuetracker.unity3d.com/issues/there-is-no-information-provided-about-the-parent-when-prefabs-child-has-broken-references-after-using-forcereserializeassets">1262196</a>)</p></li>
<li><p>Prefabs: The apply menu in the Prefab overrides comparison view no longer lists apply targets where all overrides are default overrides compared to that apply target. This brings the apply menu items in the comparison view in line with the apply menu items in component context menus and ensures there's no apply menu items that don't have any effect. (<a href="https://issuetracker.unity3d.com/issues/exception-is-not-thrown-when-nested-prefabs-name-cant-be-overridden">1190143</a>)</p></li>
<li><p>Prefabs: When opening a UI Prefab in Prefab Mode in Context and then opening a child UI Prefab in a nested Prefab Mode in Context, the UI of the child would sometimes get hidden below the UI of the context. (1268329)</p></li>
<li><p>Profiler: Fixed a bug when UnityEditor.UnityStats returned invalid number of active animations. (1252764)</p></li>
<li><p>Profiler: Fixed a crash while using Profiler ProfilerProperty and ProfilerFrameDataIterator API. (1289580)</p></li>
<li><p>Profiler: Fixed an issue which caused RegisterNewMarkerCallback to be called multiple times with the same marker. (1158554)</p></li>
<li><p>Profiler: Fixed an issue with wrong chart scale after profiler capture load. (<a href="https://issuetracker.unity3d.com/issues/profiler-the-cpu-frame-chart-doesnt-scale-with-the-data-when-the-data-is-loaded-in">1283344</a>)</p></li>
<li><p>Profiler: Fixed crash when -profiler-enable arg is used. (<a href="https://issuetracker.unity3d.com/issues/deployment-management-project-fails-to-open-with-the-command-line-argument-profiler-enable-and-crash-logo-appears">1295637</a>)</p></li>
<li><p>Profiler: Fixed errors after switching from Main Thread to another in Editor profiling. (<a href="https://issuetracker.unity3d.com/issues/profiler-errors-and-crash-after-switching-from-main-thread-to-another-in-editor-profiling">1293246</a>)</p></li>
<li><p>Profiler: Fixed exit gui state when clearing to prevent errors when clearing profiler. (1305901)</p></li>
<li><p>Profiler: Fixed HDRP/URP GPU statistics in Editor showing zeroes. (1299569)</p></li>
<li><p>Profiler: Fixed issue when threads could have empty name in Profiler. (<a href="https://issuetracker.unity3d.com/issues/profiler-deserializer-thread-is-shown-at-top-of-timeline-view-with-no-thread-name-while-generating-test-data">1278270</a>)</p></li>
<li><p>Profiler: Fixed large amount of tris and verts are being reported in an empty scene by the Game View statistics when refocusing the Editor. (<a href="https://issuetracker.unity3d.com/issues/large-amount-of-tris-and-verts-are-being-reported-in-an-empty-scene-by-the-game-view-statistics-when-refocusing-the-editor">1275827</a>)</p></li>
<li><p>Profiler: Fixed performance overhead in Asset Importer process due to profiler capture always enabled. (1298257)</p></li>
<li><p>Profiler: Fixed potential array outbound access on non-paired GPU marker begin/end. (1295390)</p></li>
<li><p>Profiler: Fixed Profiler settings option to clarify what it does. (<a href="https://issuetracker.unity3d.com/issues/profiler-switching-profiler-target-mode-from-editmode-to-playmode-under-preferences-does-not-work">1240432</a>)</p></li>
<li><p>Profiler: Fixed Profiler window breaking after switching treads. (<a href="https://issuetracker.unity3d.com/issues/profiler-window-breaks-after-switching-treads">1293257</a>)</p></li>
<li><p>Profiler: Fixed recursive call in ProfilerUnsafeUtility.CreateMarker causing il2cpp builds to fail.</p></li>
<li><p>Profiler: Fixed situation when Audio Profiler view can show information from an invalid frame. (<a href="https://issuetracker.unity3d.com/issues/profiler-audio-detailed-information-retains-data-after-recording-it-when-loading-in-data">1240903</a>)</p></li>
<li><p>Profiler: Fixed Standalone Profiler recording without clearing previously recorded data when Clear on Play is selected. (<a href="https://issuetracker.unity3d.com/issues/profiler-standalone-process-continues-recording-without-clearing-previously-recorded-data-when-clear-on-play-is-selected">1249920</a>)</p></li>
<li><p>Profiler: Fixed statistics window showing 0 or flickering when in the Play Mode. (<a href="https://issuetracker.unity3d.com/issues/macos-statistics-windows-statistics-show-0-when-in-the-play-mode">1301835</a>)</p></li>
<li><p>Profiler: Fixed the sorting order of the Show Related Objects panel to be numerical instead of alphabetical. (<a href="https://issuetracker.unity3d.com/issues/wrong-sorting-for-gc-alloc-column-in-show-related-objects-panel-of-profiler-window">1198266</a>)</p></li>
<li><p>Profiler: Fixed the Thread Selection Dropdown in Hierarchy view showing multiple threads as selected if they all share the same name.</p></li>
<li><p>Profiler: Fixed to generate unique names for new Profiler Modules to avoid confusion. (1256273)</p></li>
<li><p>Profiler: Fixed UnityEngine.Profiling.Recorder.gpuElapsedNanoseconds produced invalid results on Vulkan. (1273246)</p></li>
<li><p>Profiler: Hierarchy Views randomly collapsing (i.e. hiding their children) parts of the sample tree when Editor Only samples are present in a frame and the "Collapse EditorOnly Samples" option is turned on (default setting is on).</p></li>
<li><p>Profiler: Removing the Loading.IDRemapping profiler tag which was causing excessive profiling overhead when loading AssetBundles.</p></li>
<li><p>Profiler: Selecting the Modules dropdown on Mac now closes the dropdown window if it's open. (<a href="https://issuetracker.unity3d.com/issues/profiler-profiler-modules-dropdown-window-doesnt-close-on-clicking-its-header">1317447</a>)</p></li>
<li><p>Profiler: Selections CPU or GPU samples made in the CPU Usage and GPU Usage Profiler Modules now carry over correctly and persistently to all views (Timeline, Hierarchy, Raw Hierarchy) as well as to all frames that contain them. In frames other than the one the selection was originally made in, the selection will point to the first sample that provides the best match to the stack of sample names that lead up to that original sample. So if there are e.g. multiple Components of the same type "MyComponent", and you select the "MyComponent.Update()" sample of one of them, there is no way for the Profiler to identify the "MyComponent.Update()" sample of exactly that sample Component in the next frame. It will therefore just select the very first "MyComponent.Update()" sample it can find. If a part of the Sample Stack is missing in a frame, the selection Tooltip in Timeline or an extra line at the bottom of the Hierarchy views will alert you of the fact, that the selection that was carried over to this frame is just an approximation. An option was added to show the difference in this approximated Sample Stack, and the originally selected Sample Stack. If not even one of the sample names from the original selection fits the samples in a particular frame and thread, no selection will be displayed. If a selection was made on a thread other than the Main Thread, switching to the Hierarchy Views will automatically switch them to the right thread this selection was made in. (<a href="https://issuetracker.unity3d.com/issues/ux-selection-of-sample-does-not-distribute-on-all-views-timeline-hierarchy-raw-hierarchy">1066309</a>)</p></li>
<li><p>Profiler: Stops UI System Preview Window from being maximised and throwing an exception. (<a href="https://issuetracker.unity3d.com/issues/profiler-null-reference-exception-thrown-on-maximizing-ui-system-preview-window">1287275</a>)</p></li>
<li><p>Scene Manager: Enforce required full path for LoadSceneInPlayMode. (<a href="https://issuetracker.unity3d.com/issues/scenes-are-loaded-without-any-gameobjects-present-when-valid-scene-name-is-passed-to-loadscene-async-inplaymode">1220015</a>)</p></li>
<li><p>Scene Manager: Make GetSceneByPath no longer case sensitive. (<a href="https://issuetracker.unity3d.com/issues/scenemanager-getscenebypath-returns-an-invalid-scene-when-lower-case-slash-not-case-sensitive-path-is-provided">1214583</a>)</p></li>
<li><p>Scene Manager: Prevent loading scene where multiple objects have same identifier. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-transformchangedispatch-queuetransformchangeifhaschanged-when-opening-a-scene">1138553</a>)</p></li>
<li><p>Scene Manager: Scene is set dirty when child dragged upon own parent. (<a href="https://issuetracker.unity3d.com/issues/drag-and-drop-a-child-on-the-parent-operation-doesnt-dirty-the-scene">1278128</a>)</p></li>
<li><p>Scene/Game View: Exposed a property to make grid snapping usable from custom EditorTools.</p></li>
<li><p>Scene/Game View: Fixed "Width &amp; Height" field in the new Game View aspect ratio menu not allowing mouse drag input. (<a href="https://issuetracker.unity3d.com/issues/gameview-input-value-for-the-width-and-height-is-not-changing-when-a-mouse-is-dragged-over-it-under-the-free-aspect-ratio">1284724</a>)</p></li>
<li><p>Scene/Game View: Fixed crash in GizmoManager when trying to build gizmos for a GameObject with a null transform component. (<a href="https://issuetracker.unity3d.com/issues/clicking-on-game-objects-in-the-scene-crashes-the-editor">1260013</a>)</p></li>
<li><p>Scene/Game View: Fixed Line Renderer editor not repainting the Scene View when selecting points. (<a href="https://issuetracker.unity3d.com/issues/line-renderer-edit-points-scene-view-gizmo-is-not-updated-when-a-point-is-selected-in-the-inspector-window">1276045</a>)</p></li>
<li><p>Scene/Game View: Fixed picking in Scene view for materials with non-2D _MainTex textures. (<a href="https://issuetracker.unity3d.com/issues/error-assigning-3d-texture-to-2d-texture-property-maintex-when-using-a-texture3d-and-a-shader-from-the-unity-manual">1288999</a>)</p></li>
<li><p>Scene/Game View: Fixed Scene View Invert Selection not taking into account scene picking/visibility state. (<a href="https://issuetracker.unity3d.com/issues/sceneviz-ctrl-plus-i-inverse-selection-will-ignore-objects-that-arent-pickable">1277187</a>)</p></li>
<li><p>Scene/Game View: Fixed Scene View Overlays preventing other IMGUI windows in the Scene View from receiving input. (<a href="https://issuetracker.unity3d.com/issues/editortools-editor-tools-doesnt-work-when-component-editor-tools-panel-is-toggled-on">1282859</a>)</p></li>
<li><p>Scripting: C# scripts containing invalid characters in disabled conditional sections are now correctly imported. (<a href="https://issuetracker.unity3d.com/issues/unity-doesnt-recognise-the-script-as-monobehaviour-script-when-theres-a-grave-accent-in-an-number-if-false-block-inside-a-namespace">1279339</a>)</p></li>
<li><p>Scripting: Common math and geometry structs such as Vector3 no longer depend on CultureInfo.CurrentCulture to implement ToString method overloads. (<a href="https://issuetracker.unity3d.com/issues/string-dot-format-returns-string-containing-decimal-commas-instead-of-dots-for-vector-types-depending-on-set-cultureinfo">1275065</a>)</p></li>
<li><p>Scripting: Favor .pdb files over .mdb files when symbols are loaded for managed assemblies if both files exist. (1278282)</p></li>
<li><p>Scripting: Fixed debugger crashes caused due to incorrect marshalling for pinvoke byte array return type. (<a href="https://issuetracker.unity3d.com/issues/crash-while-inspecting-byteslist-values-of-a-dictionary-in-vs-debugger-when-using-arucounity-plugin">1274470</a>)</p></li>
<li><p>Scripting: Fixed minor documentation issue in Player Settings for Get/SetAdditionalCompilerArgumentsForGroup.</p></li>
<li><p>Scripting: Fixed potential AsseblyUpdater assembly corruption when applying Camera.GetScreenHeight() / GetScreenWidth() -&gt; Screen.height/width updates.</p></li>
<li><p>Scripting: Fixed potential AsseblyUpdater assembly corruption when field name and type needs updating.</p></li>
<li><p>Scripting: Fixed potential error due to ApiUpdater not handling extension methods correctly.</p></li>
<li><p>Scripting: Fixes usage of comment in rsp file. (1216598)</p></li>
<li><p>Scripting: Fixes usage of whitespace in rsp command arguments. (<a href="https://issuetracker.unity3d.com/issues/visual-c-number-compiler-fails-to-locate-assembly-if-response-file-compiler-argument-path-contains-spaces">1223381</a>)</p></li>
<li><p>Scripting: Quaternion.Angle: Apply the same epsilon tolerance value when comparing q &amp; -q as we do when comparing q &amp; q, both of which should always result in an angle of 0. (<a href="https://issuetracker.unity3d.com/issues/quaternion-dot-angle-is-non-null-when-comparing-a-quaternion-with-its-inverted-arguments">1246947</a>)</p></li>
<li><p>Scripting: Sign bee_backend.exe so it does not trip up user virus protection.</p></li>
<li><p>Search: Do not show empty explicit search provider tabs. (<a href="https://issuetracker.unity3d.com/issues/search-empty-special-search-provider-are-shown-even-if-they-cannot-have-any-result">1296463</a>)</p></li>
<li><p>Search: Fixed mesh filtering in Project window (t:Mesh) doesn't show any Meshes. (<a href="https://issuetracker.unity3d.com/issues/editor-mesh-filtering-in-project-window-t-mesh-doesnt-show-any-meshes">1305383</a>)</p></li>
<li><p>Search: Fixed selecting a saved query from the saved searches list doesn't update the providers. (<a href="https://issuetracker.unity3d.com/issues/search-selecting-a-saved-query-from-the-saved-searches-list-doesnt-update-the-providers">1296559</a>)</p></li>
<li><p>Search: Improved search index artifact asynchronous resolution performance for very large projects (i.e. 900k files). (1296452)</p></li>
<li><p>Search: Slightly improved Scene indexing performance. (1310424)</p></li>
<li><p>Serialization: Fields of type UnityEngine.Hash128 are now correctly serialized in ScriptableObjects and MonoBehaviours. (<a href="https://issuetracker.unity3d.com/issues/unityengine-dot-hash128-and-unityeditor-dot-guid-are-not-serialized-in-user-components">1271062</a>)</p></li>
<li><p>Serialization: Fixed SerializedProperty.arraySize and add SerializedProperty.minArraySize. (<a href="https://issuetracker.unity3d.com/issues/type-is-not-a-supported-string-value-error-appears-in-the-console-window-when-selecting-multiple-fbx-models">1279753</a>)</p></li>
<li><p>Serialization: HDRP/TerrainLit shader no longer produce build errors when in Always included Shaders list. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-building-the-project-if-hdrp-slash-terrainlit-shader-is-in-always-included-shaders-list">1237876</a>)</p></li>
<li><p>Services: Fixed the parameter supplied to the request to enable analytics.</p></li>
<li><p>Shadergraph: Fixed a broken link in the TOC to Main Preview.</p></li>
<li><p>Shadergraph: Fixed an issue where deleting a property node while your mouse is over it leaves the property highlighted in the blackboard. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-deleting-a-property-node-while-your-mouse-is-over-it-leaves-the-property-highlighted-in-the-blackboard">1238635</a>)</p></li>
<li><p>Shadergraph: Fixed an issue where dragging Blackboard properties and using the  Escape key left the drag indicator visible.</p></li>
<li><p>Shadergraph: Fixed an issue where dragging Blackboard properties wouldn't scroll the list. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-dragging-an-individual-property-in-the-blackboard-doesnt-automatically-scroll-the-list">1293632</a>)</p></li>
<li><p>Shadergraph: Fixed an issue where Float/Vector1 properties were not editable in the Inspector, unlike other Vector types.</p></li>
<li><p>Shadergraph: Fixed an issue where renaming blackboard properties through the Blackboard wouldn't actually change the underlying property name.</p></li>
<li><p>Shadergraph: Fixed an issue where SampleRawCubemapNode were requiring the Normal in Object space instead of World space. (1307962)</p></li>
<li><p>Shadergraph: Fixed an issue where the Blackboard wasn't resizable from all directions, unlike the Inspector and Main Preview.</p></li>
<li><p>Shadergraph: Fixed an issue with the Gradient color picker displaying different values than the selected color.</p></li>
<li><p>Shadergraph: Fixed issue with Hybrid renderer compatibility. (1296776)</p></li>
<li><p>Shadergraph: Fixed issue with SRP Batcher compatibility. (1310624)</p></li>
<li><p>Shadergraph: Fixed the Custom Editor GUI field in the Graph settings that was ignored.</p></li>
<li><p>Shadergraph: Fixed the ViewDirection Node in Tangent space's calculation to match how the transform node works.</p></li>
<li><p>Shadergraph: Newly created properties and keywords no longer use obfuscated GUID-based reference names in the shader code. (1300484)</p></li>
<li><p>Shadergraph: The Material Inspector now displays Boolean keywords without requiring them to have reference names that end in _ON. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-boolean-keywords-disappear-from-the-inspector-after-changing-the-reference-name">1306820</a>)</p></li>
<li><p>Shaders: Added a new keyword to handle the custom editors per render pipeline in ShaderLab to ensure a smooth material workflow between render pipelines.</p></li>
<li><p>Shaders: Added Material.SetInteger, Material.GetInteger, MaterialPropertyBlock.SetInteger, MaterialPropertyBlock.GetInteger, Shader.SetGlobalInteger and Shader.GetGlobalInteger that use integers internally; added Integer property type to ShaderLab. (<a href="https://issuetracker.unity3d.com/issues/material-setint-and-getint-methods-are-not-precise-when-large-values-are-used">1277994</a>)</p></li>
<li><p>Shaders: Fixed Integer property type not affecting uniform state and fixed function state in shaders. (<a href="https://issuetracker.unity3d.com/issues/integer-property-type-in-shaderlab-has-no-effect-on-uniforms-and-fixed-function-state">1294048</a>)</p></li>
<li><p>Shaders: Fixed iOS Tesselation shader compilation issue when using appdata_full. (<a href="https://issuetracker.unity3d.com/issues/ios-metal-shaders-with-tessellation-are-not-compiled-when-displacement-feature-is-removed-from-number-pragma">1281129</a>)</p></li>
<li><p>Shaders: Fixed the "end of shader compiler log" printing to the editor log at compiler crashes if the compiler log is very small.</p></li>
<li><p>Shaders: Frame debugger now shows Integer properties in the draw call description. (<a href="https://issuetracker.unity3d.com/issues/integer-properties-do-not-show-up-in-frame-debugger">1294069</a>)</p></li>
<li><p>Shaders: Prevent editor crash on unlucky timing when a shader compiler process is being killed.</p></li>
<li><p>Shaders: Removed redundant shader upgrader pass on editor startup. (1274174)</p></li>
<li><p>Shaders: Reset m_LightmapFlags in Material::ResetWithShader(). (<a href="https://issuetracker.unity3d.com/issues/bug-materials-reset-functionality-doesnt-work-on-emission-in-material">1283694</a>)</p></li>
<li><p>Shaders: ShaderUtil.ClearShaderMessages() now actually clears all the current shader errors. Any previously encountered errors will come back when trying to compile the shader again either for build or rendering, or when reimporting. (1283645)</p></li>
<li><p>Shaders: Support Texture.CalculateLevelOfDetail function in Metal shaders. (1237836)</p></li>
<li><p>Terrain: Fixed a connection cleared when AutoConnect is not used in first frame. (<a href="https://issuetracker.unity3d.com/issues/terrain-normals-produce-artifacts-when-connecting-neighboring-terrain-using-terrain-dot-setneighbors">1241302</a>)</p></li>
<li><p>Terrain: Fixed being unable to rotate branch group. (1283095)</p></li>
<li><p>Terrain: Fixed new Tree GameObjects instantiating with the name "OptimizedTree" instead of "Tree.". (1283097)</p></li>
<li><p>Terrain: Fixed Terrain paint tool selection persistence when loading or removing paint tools. (1283242)</p></li>
<li><p>Terrain: Fixed: terrain in draw instanced mode now cast shadows when illuminated by spotlights. (<a href="https://issuetracker.unity3d.com/issues/terrain-does-not-cast-shadows-when-draw-instanced-option-is-enabled-in-the-terrain-settings">1192100</a>)</p></li>
<li><p>Terrain: Fixes confusing behavior for Lock Width To Height feature when painting trees on Terrain where width is randomized within the specified height range instead of using the randomized height value. (1265350)</p></li>
<li><p>Terrain: Fixes crash that occurs when deleting terrain component during OnTerrainChanged callback. (1281737)</p></li>
<li><p>Terrain: Internal: fixed crash when copying terrain during callback with debug allocator active. (1286747)</p></li>
<li><p>Terrain: Re-use of the leaf icon for the tree component as the component icon was missing. (<a href="https://issuetracker.unity3d.com/issues/tree-component-icon-is-missing-in-the-inspector">1260457</a>)</p></li>
<li><p>Terrain: The reset functionality from the component burger menu was not working for trees, the PR fixes this. (<a href="https://issuetracker.unity3d.com/issues/tree-reset-functionality-does-not-work-in-the-tree-component">1252536</a>)</p></li>
<li><p>Terrain: When reparenting a element of the tree, all modification made by hand are reset to avoid strange behaviors. (1272795)</p></li>
<li><p>Text: Fixed a crash in the Text system. (1288809)</p></li>
<li><p>Timeline: Fixed an alignment issue with property reference fields in Timeline. (<a href="https://issuetracker.unity3d.com/issues/timeline-source-game-object-input-field-is-misaligned-under-contol-playable-asset-for-contol-track">1222744</a>)</p></li>
<li><p>Timeline: Fixed an issue with Timeline audio playing at the wrong time when Time.timeScale was not set to 1. (<a href="https://issuetracker.unity3d.com/issues/timeline-audio-clips-are-played-early-when-time-scale-is-less-than-1">981046</a>)</p></li>
<li><p>UI: Added OnSubmit functionality which will be called when the input field should be sumitted. (1262424)</p></li>
<li><p>UI: Fixed an issue where canvas takes the Display size for RenderTexture. (1294869)</p></li>
<li><p>UI: Fixed issue where PixelPerfect wouldn't update right away when toggled on the Canvas. (<a href="https://issuetracker.unity3d.com/issues/pixel-perfect-setting-not-applied-immediately">1261788</a>)</p></li>
<li><p>UI: Fixed issue with layout property preview not having contrast in light skin. (<a href="https://issuetracker.unity3d.com/issues/low-color-contrast-between-text-and-its-background-in-the-layout-properties-section-when-the-editor-theme-is-set-to-light">1293782</a>)</p></li>
<li><p>UI: Fixed issue with UI profiler showing wrong batch count for canvas's that shrink. (1290246)</p></li>
<li><p>UI: Fixed uGUI description to not mention UI Toolkit to avoid confusion.</p></li>
<li><p>UI: Fixed Unity Events that were set as Runtime only to initialize properly upon entering playmode with the FastEnterPlay mode enabled. (<a href="https://issuetracker.unity3d.com/issues/onvaluechanged-callback-is-not-executed-in-play-mode-when-domain-reload-is-disabled">1206410</a>)</p></li>
<li><p>UI: Fixing issue with vertex attributes not getting pass through to the profile rerendering leaving the view empty. (<a href="https://issuetracker.unity3d.com/issues/profiler-ui-objects-are-not-displayed-in-the-preview-of-profilers-ui-section">1276001</a>)</p></li>
<li><p>UI: Fixing uGUI doc population.</p></li>
<li><p>UI: Make use to first materials texture ID and texel size if no texture has been provided. (<a href="https://issuetracker.unity3d.com/issues/textmeshpro-text-ui-does-not-display-outline-effect-when-used-with-a-custom-shader">1257149</a>)</p></li>
<li><p>UI Toolkit: Added the possibility to put an event on mouse down before showing a contextual menu. (1268159)</p></li>
<li><p>UI Toolkit: Added tooltip in StyleSheets pane when hovering a class selector that is trimmed (UI Builder). (1313198)</p></li>
<li><p>UI Toolkit: Backport - Added new controls (RadioButton, RadioButtonGroup, DropdownField) to the UITK Samples and UI Builder Standard Library pane. (1310158)</p></li>
<li><p>UI Toolkit: Backport - Fixed RadioButtonGroup and DropdownField choice attribute parsing in the UI Builder.</p></li>
<li><p>UI Toolkit: Backport - GenericDropdownMenu no longer needs to be reinstanced on every use. (1308433)</p></li>
<li><p>UI Toolkit: Changed EnumField+derivatives &amp; BasePopupField-based classes to properly handle pointer down events. (<a href="https://issuetracker.unity3d.com/issues/quick-search-error-thrown-on-selecting-extension-folder-file-option-under-excludes-from-search-index-manager-window">1248669</a>)</p></li>
<li><p>UI Toolkit: Changed TextField to match IMGUI behavior of select-all-on-mouse-up. (1179932)</p></li>
<li><p>UI Toolkit: Double-clicking a uxml file will always open the UI Builder. (1313423)</p></li>
<li><p>UI Toolkit: Drag and drop of class pills in stylesheet pane now support selector reordering. (UI Builder). (1313148)</p></li>
<li><p>UI Toolkit: Enabled dynamic atlassing of sprites. Fixed tight sprite scale modes.</p></li>
<li><p>UI Toolkit: Fixed "unsaved changes will be lost" popup when changing an uxml file using an external editor. (UI Builder). (1316730)</p></li>
<li><p>UI Toolkit: Fixed a bug where users could drag the slider knob behind the its text field when enabled. (1294691)</p></li>
<li><p>UI Toolkit: Fixed an issue where changing the size of a TwoPaneSplitView would not resize its content. (<a href="https://issuetracker.unity3d.com/issues/editor-window-does-not-preserve-the-minimum-height-and-width-of-ui-elements-when-resizing-it">1313077</a>)</p></li>
<li><p>UI Toolkit: Fixed being able to drag elements onto existing elements outside the currently active sub-document.</p></li>
<li><p>UI Toolkit: Fixed being able to drag or create elements onto empty space in the Canvas while editing a child sub-document in-place, leading to elements being added to the wrong document.</p></li>
<li><p>UI Toolkit: Fixed being able to paste USS Selectors from the Hierarchy pane and elements from the StyleSheets pane. Paste now works based on which pane is currently active. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed button text on the circular dependency dialog box. (UI Builder). (1313150)</p></li>
<li><p>UI Toolkit: Fixed clicking in empty space in Hierarchy pane not deselecting a USS Selector and vice-versa for the StyleSheets pane. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed closing of no UI Toolkit installed warning disabling Viewport zoom.</p></li>
<li><p>UI Toolkit: Fixed document settings (like Canvas background and zoom) being reset when editing a sub-document in-place. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed editor freeze when adding circular dependencies through the UI Builder and a external editor. (1315612)</p></li>
<li><p>UI Toolkit: Fixed element highlight overlay not being reset after deleting the element. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed Element not visisle after being hiden/shown in specific sequence. (<a href="https://issuetracker.unity3d.com/issues/ui-builder-button-elements-sometimes-not-visible-after-being-pressed-multiple-times">1269414</a>)</p></li>
<li><p>UI Toolkit: Fixed error with UI Elements Samples window after Minimizing/Maximizing another window. (<a href="https://issuetracker.unity3d.com/issues/uielements-maximizing-ui-toolkit-sample-window-throws-invalid-editor-window-unityeditor-dot-fallbackeditorwindow-errors">1244800</a>)</p></li>
<li><p>UI Toolkit: Fixed exception thrown when selecting the currently open UXML asset in the Project Window. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed float and double attributes not being stored correctly in UXML as CultureInvariant. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed handling of a deleted StyleSheet that is being used by the currently open UXML UI Document. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed KeyboardNavigationManipulator does not trigger the callback if operation is None. (1314063)</p></li>
<li><p>UI Toolkit: Fixed layout being affected by the state of RenderTexture.active. (<a href="https://issuetracker.unity3d.com/issues/uir-ui-toolkit-runtime-resize-bug-with-graphics-dot-blit">1268095</a>)</p></li>
<li><p>UI Toolkit: Fixed ListView Horizontal Scrolling attribute value not being reflected properly in the Inspector.</p></li>
<li><p>UI Toolkit: Fixed ListView range selection when initial selection is set programmatically.</p></li>
<li><p>UI Toolkit: Fixed non-whole pixel size and position values resulting from resizing or moving elements in the Viewport with the zoom set to 75%. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed not being able to create a single-character selector. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed not being able to rename USS Selectors directly inside the StyleSheets pane via double-click or the right-click menu.</p></li>
<li><p>UI Toolkit: Fixed null reference exception when using the Align style properties on a USS Selector. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed panel color that was not being premultiplied before clearing the target texture background. (<a href="https://issuetracker.unity3d.com/issues/uir-clear-color-isnt-premultiplied-before-being-applied">1277149</a>)</p></li>
<li><p>UI Toolkit: Fixed possible instability inside in-place sub-document editing mode after selecting elements belonging to a parent document.</p></li>
<li><p>UI Toolkit: Fixed potentially losing assigned StyleSheets in parent document when discarding changes before going inside a sub-document.</p></li>
<li><p>UI Toolkit: Fixed PropertyField created from UXML missing its default label. (1309780)</p></li>
<li><p>UI Toolkit: Fixed PropertyField now able to have no label displayed if an empty string is passed as the label argument. Note that if a null value is passed, the label will still be displayed using the localized display name, like before. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-propertyfield-can-not-have-no-label">1293580</a>)</p></li>
<li><p>UI Toolkit: Fixed re-importing of a child UXML asset that is instanced by a parent UXML asset causing the parent to be unusable via the Library pane.</p></li>
<li><p>UI Toolkit: Fixed ScrollView's scroll bars not showing when children are using position:absolute. (1247583)</p></li>
<li><p>UI Toolkit: Fixed scrollView's showHorizontal and showVertical limitations. They are converted to a tristate enum, horizontalScrollerVisibility and verticalScrollerVisibility, to support a new Hidden state, along with AlwaysVisible and Auto. (1278466)</p></li>
<li><p>UI Toolkit: Fixed settings search not working for UI Builder settings in the Project Settings window. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed the InvalidCastException thrown when assigning a built-in image asset to a Texture2D in the UI Builder inspector. (UI Builder).</p></li>
<li><p>UI Toolkit: Fixed unsaved changes * indicator not being reset when going inside a child sub-document while discarding changes in the parent.</p></li>
<li><p>UI Toolkit: Only use mapped buffers when the graphics device support it. (1281641)</p></li>
<li><p>UI Toolkit: Prevent NullRefException when providing textureless sprites as background.</p></li>
<li><p>UI Toolkit: PropertyField will now use a custom label(if provided) when drawing a property with an IMGUI PropertyDrawer.</p></li>
<li><p>UI Toolkit: PropertyFields on array fields would not refresh properly when array size changed in some use cases. (1290774)</p></li>
<li><p>UI Toolkit: Selecting the UI Builder selector creation field no longer selects the dot character, but instead places the curser right after it, to avoid erasing it by mistake. (UI Builder). (1310160)</p></li>
<li><p>UI Toolkit: Throw a proper argument null exception when using UQuery.</p></li>
<li><p>UI Toolkit: Trying to move/rename nested uxml/uss files of an opened document will prompt the invalid action dialog as it should. (UI Builder). (1315594)</p></li>
<li><p>Universal: Fixed an issue such that it is now posible to enqueue render passes at runtime.</p></li>
<li><p>Universal: Fixed an issue where bokeh dof is applied incorrectly when there is an overlay camera in the camera stack. (<a href="https://issuetracker.unity3d.com/issues/urp-bokeh-depth-of-field-is-applied-incorrectly-when-the-main-camera-has-an-overlay-camera-in-the-camera-stack">1303572</a>)</p></li>
<li><p>Universal: Fixed an issue where objects in motion might jitter when the Pixel Perfect Camera is used. (<a href="https://issuetracker.unity3d.com/issues/urp-characters-sprite-repeats-in-the-build-when-using-pixel-perfect-camera-and-2d-renderer">1300474</a>)</p></li>
<li><p>Universal: Fixed an issue where the inspector of Renderer Data would break after adding RenderObjects renderer feature and then adding another renderer feature.</p></li>
<li><p>Universal: Fixed GC allocations from XR occlusion mesh when using multipass.</p></li>
<li><p>Universal: Fixed shadow cascade blend culling factor.</p></li>
<li><p>Universal: Fixed the default background color for previews to use the original color.</p></li>
<li><p>Universal: Fixed wrong shader / properties assignement to materials created from 3DsMax 2021 Physical Material.</p></li>
<li><p>Universal Windows Platform: Fixed input on IMGUI elements when using the new input system. (<a href="https://issuetracker.unity3d.com/issues/uwp-unitys-ui-and-imgui-cannot-be-interacted-while-new-input-system-is-on">1201666</a>)</p></li>
<li><p>Universal Windows Platform: Fixed Tab key on the TouchScreenKeyboard not inserting a tab character. (<a href="https://issuetracker.unity3d.com/issues/uwp-tab-key-on-hololens2-keyboard-doesnt-insert-tabs-into-inputfield-slash-tmp">1314405</a>)</p></li>
<li><p>Version Control: Fixed '-vcsMode' command-line argument being applied after API Updater. (1266509)</p></li>
<li><p>Version Control: Status overlay icons are no longer "washed out colors" in Linear color space. (<a href="https://issuetracker.unity3d.com/issues/vcs-linear-color-space-affects-version-control-icons">1218701</a>)</p></li>
<li><p>VFX Graph: Fixed unexpected compilation warning in VFXMouseBinder. (<a href="https://issuetracker.unity3d.com/issues/unexpected-compilation-warning-in-vfxmouseeventbinder">1313003</a>)</p></li>
<li><p>VFX Graph: Fixed VFXEventBinderBase throwing a null reference exception in runtime.</p></li>
<li><p>VFX Graph: Removed some useless compilation triggers (modifying not connected or disabled nodes for instance).</p></li>
<li><p>Video: Fixed video preview in editor.</p></li>
<li><p>Video: Uncommented the EndReached callback in VideoPlayback playmode tests and updated the tests since the original fix for the callback issue had landed. (1062515)</p></li>
<li><p>Virtual Texturing: Fixed a crash during tile extraction of invalid virtual texture stacks.</p></li>
<li><p>WebGL: Added more detailed information when a page load fails due to misconfiguration in server hosting settings. Note that Firefox does not currently support Brotli compression for local development (https://bugzilla.mozilla.org/show_bug.cgi?id=1670675). (<a href="https://issuetracker.unity3d.com/issues/brotli-compressed-build-fails-to-run-in-firefox">1283658</a>)</p></li>
<li><p>WebGL: Applied a workaround to Chrome specific Web Audio performance issue https://bugs.chromium.org/p/chromium/issues/detail?id=1133233. (<a href="https://issuetracker.unity3d.com/issues/webgl-audiosource-dot-update-cpu-usage-increases-overtime-when-playing-audiosources-on-chromium-browsers">1270768</a>)</p></li>
<li><p>WebGL: Attempting to open a dynamic library will now throw a DllNotFoundException rather than aborting execution as a runtime error. (<a href="https://issuetracker.unity3d.com/issues/p-slash-invoking-into-non-existent-library-crashes-player-on-webgl-instead-of-throwing-a-managed-exception">1227393</a>)</p></li>
<li><p>WebGL: Consistently refer to WebGL APIs by names "WebGL 1" and "WebGL 2". (<a href="https://issuetracker.unity3d.com/issues/project-settings-graphics-apis-naming-is-inconsistent-when-using-webgl-player">1260548</a>)</p></li>
<li><p>WebGL: Fixed a bug where keyboard up events would be missed if WebGLInput.captureAllKeyboardInput was set to false while a key was being held down. (<a href="https://issuetracker.unity3d.com/issues/input-system-key-input-get-stuck-on-pressed-state-when-captureallkeyboardinput-is-set-on-true-in-webgl">1195047</a>)</p></li>
<li><p>WebGL: Fixed a crash with Unity web loader on new macOS Big Sur.</p></li>
<li><p>WebGL: Fixed a GUI blit issue in WebGL builds with linear color space enabled, that caused washed out UI images on web browsers compared to other platforms. (<a href="https://issuetracker.unity3d.com/issues/imgui-on-webgl-builds-appears-washed-out-when-comparing-to-same-imgui-in-the-editor">1187401</a>)</p></li>
<li><p>WebGL: Fixed a hang in Caching.ClearCache() when building against multithreaded WebGL. (<a href="https://issuetracker.unity3d.com/issues/webgl-build-with-threading-stalls-when-invoking-caching-dot-clearcache">1146530</a>)</p></li>
<li><p>WebGL: Fixed an issue when a failing cross-domain revalidation request prevents a file from being downloaded. (1266091)</p></li>
<li><p>WebGL: Fixed default page template to properly scale the canvas size at startup on mobile. Removed by-default low DPI scaling on mobile pages (use a custom template .html to do half-res or quarter-res rendering if desired). (<a href="https://issuetracker.unity3d.com/issues/webgl-android-webgl-fullscreen-ignores-dpi-on-android-chrome">1274295</a>)</p></li>
<li><p>WebGL: Fixed for TAB keys being ignored by UI input fields. (1281765)</p></li>
<li><p>WebGL: Fixed inverted y axis for game controllers with the Input System on WebGL. (<a href="https://issuetracker.unity3d.com/issues/webgl-input-system-vertical-axis-input-is-inverted-slash-reversed-when-using-an-xbox-one-controller">1273623</a>)</p></li>
<li><p>WebGL: Fixed issue with paused audio clicking in Firefox. (<a href="https://issuetracker.unity3d.com/issues/webgl-pausing-audio-source-causes-continuous-tapping-sounds-in-firefox-browser">1238052</a>)</p></li>
<li><p>WebGL: Fixed Keyboard.current and Mouse.current to be immediately available in MonoBehaviour.Start() functions, instead of returning null. (<a href="https://issuetracker.unity3d.com/issues/new-input-system-cannot-retrieve-devices-in-start-method-when-used-in-webgl-build">1239007</a>)</p></li>
<li><p>WebGL: Fixed mouse wheel scrolling with the new input system on WebGL. (<a href="https://issuetracker.unity3d.com/issues/webgl-input-system-scrolling-with-mouse-wheel-is-much-slower-on-webgl-builds-when-using-new-input-system-package">1264545</a>)</p></li>
<li><p>WebGL: Fixed occasional large values with Input.GetAxis. (<a href="https://issuetracker.unity3d.com/issues/webgl-input-dot-getaxis-slash-input-dot-getaxisraw-sometimes-returns-significantly-larger-value-in-webgl-when-cursor-is-locked">1208971</a>)</p></li>
<li><p>WebGL: Fixed Preset incompatibilities in Player Settings. (1232138)</p></li>
<li><p>WebGL: Fixed Screen.orientation API to work on Android and iOS. On desktop browsers Screen.orientation is simulated by checking whether browser window width &lt; height. (<a href="https://issuetracker.unity3d.com/issues/webgl-android-screen-dot-orientation-doesnt-update-on-android-webgl">1283211</a>)</p></li>
<li><p>WebGL: Fixed UnityWebRequest with relative URLs on WebGL platform when built with no exception support (Enable Exceptions = None). (<a href="https://issuetracker.unity3d.com/issues/unitywebrequest-throws-an-error-when-exceptions-set-to-none">1283652</a>)</p></li>
<li><p>WebGL: Fixed video playback in Firefox to loop seamlessly. For more information, see https://bugzilla.mozilla.org/show_bug.cgi?id=1668591. (<a href="https://issuetracker.unity3d.com/issues/theres-a-black-frame-in-a-video-on-firefox-browser-when-the-video-loops">1267333</a>)</p></li>
<li><p>WebGL: Overlay cameras will no longer cause full screen renders to be incorrect. (<a href="https://issuetracker.unity3d.com/issues/webgl-multiple-camera-viewports-in-fullscreen-mode-are-rendered-differently-in-webgl-builds-than-in-the-editor">1184385</a>)</p></li>
<li><p>WebGL: Reduced memory usage on dual Intel integrated + NVidia GPU Windows laptops when using URP in a large scene with many individual objects. (<a href="https://issuetracker.unity3d.com/issues/webgl-urp-large-memory-allocations-on-builds-when-many-objects-are-visible-in-the-viewport-while-using-integrated-gpu">1225254</a>)</p></li>
<li><p>WebGL: Removed support for Wasm arithmetic exceptions in preparation for updating to LLVM Wasm backend. (<a href="https://issuetracker.unity3d.com/issues/webgl-ui-toolkit-player-crashes-when-using-textfield">1286167</a>)</p></li>
<li><p>Windows: Batchmode now allows settings resolution and window mode. (<a href="https://issuetracker.unity3d.com/issues/standalone-player-resolution-is-not-correct-when-build-is-ran-in-batchmode-with-custom-screen-width-and-height-arguments">1266308</a>)</p></li>
<li><p>Windows: Fixed Time.deltaTime calculations on D3D11 and D3D12 when VSync is force disabled from the driver software (like Nvidia Control Panel, Radeon Settings or Intel Graphics Command Center).</p></li>
<li><p>Windows: Fixed Unity Editor Icon at the top left is blurry. (<a href="https://issuetracker.unity3d.com/issues/unity-editor-icon-at-the-top-left-is-blurry">1264422</a>)</p></li>
<li><p>Windows: Fixed Windows player infrequently deadlocking when changing fullscreen modes on D3D11 and D3D12 graphics APIs.</p></li>
<li><p>Windows: Popover window in Frame debugger now closes when pressing up or down on the keyboard in the tree view.</p></li>
<li><p>Windows: Provide informational message in developer console when Open Log File operation fails. (<a href="https://issuetracker.unity3d.com/issues/open-log-file-button-doesnt-create-slash-open-log-file-in-developer-console">1276710</a>)</p></li>
<li><p>Windows: Removed UWP "USB Device" Build and Run option. (<a href="https://issuetracker.unity3d.com/issues/build-and-run-usb-device-option-is-broken">1292590</a>)</p></li>
<li><p>XR: Added XR Interaction Toolkit as a pre-release package.</p></li>
<li><p>XR: Corrected document link underlining.</p></li>
<li><p>XR: Fixed a deadlock that occurred when the Windows player was hidden and VR was enabled.</p></li>
<li><p>XR: Fixed an issue with Graphics.Blit when using VRTextureUsage.TwoEyes. (<a href="https://issuetracker.unity3d.com/issues/graphics-dot-blit-0-index-texture-will-not-be-drawn-when-vrtextureusage-is-set-to-twoeyes">1258990</a>)</p></li>
<li><p>XR: Removed error-reporting for XR Devices if no tracking features found on device.</p></li>
<li><p>XR: Updated the subsystem instance map to clear on deinitialize so that stale instances aren't retrieved on restarts.</p></li>
</ul>
