# Unity 2020.2.0
https://unity3d.com/unity/whats-new/2020.2.0

## Final 2020.2.0f1 Release Notes


### Features
<ul>
<li><p>2D: Added C# job tessellation support for the Sprite Shape's <em>Fill Area</em>.</p></li>
<li><p>Android: Improved support for playing video in addressables and AssetBundles. Compressed and in-memory bundles are now supported on Android 9 and newer devices.</p></li>
<li><p>Animation: Verified <a href="https://docs.unity3d.com/Packages/com.unity.animation.rigging@latest">Animation Rigging</a> package version 1.0.3.</p></li>
<li><p>Asset Pipeline: Added Safe Mode for startup, which gives you the option to avoid asset importing when there are script compilation errors.<br></p> 
<div class="inline-frame rel clear mb20">
           <img src="/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif" class="blank bg-dg">
           <iframe src="https://www.youtube.com/embed/BBs30DoCkQ0?HD=1&amp;rel=0&amp;showinfo=0&amp;controls=1&amp;theme=dark&amp;color=white&amp;" frameborder="0" border="0" scrolling="no" allowfullscreen="1" mozallowfullscreen="1" webkitallowfullscreen="1"></iframe>
         </div></li>
<li><p>Asset Pipeline: Added two new properties to the <em>Asset Pipeline</em>:<br></p> 
<ul>
<li><code>AssetDatabase.GlobalArtifactDependencyVersion</code><br></li>
<li><code>AssetDatabase.GlobalArtifactProcessedVersion</code>.</li>
</ul></li>
<li><p>Asset Pipeline: Enabled consistency checking of assets using <code>-consistencyCheck</code> on the command-line and when force reimporting through the Project window.</p></li>
<li><p>Editor: Added a <code>-version</code> argument to command-line inputs that prints the current version of Unity to the console.</p></li>
<li><p>Editor: Added an <code>EditorToolContext</code> class to allow custom tools to override built-in transform tools. See <a href="https://docs.unity3d.com/2020.2/Documentation/ScriptReference/EditorTools.EditorToolContext.html">EditorToolContext</a>.</p></li>
<li><p>Editor: Added button <em>Enable debugging to all projects</em> to the dialog box <em>C# Debugger Attached</em>, and made text more descriptive.</p></li>
<li><p>Editor: Added support for a Root Namespace field in Assembly Definition files. New scripts created inside Unity have a namespace in the default template if it is set in the corresponding Assembly Definition file (or for non-Assembly Definition file scripts, the <em>Project Settings</em> &gt; <em>Editor</em> &gt; <em>Project Root</em> namespace).<br></p> 
<div class="inline-frame rel clear mb20">
           <img src="/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif" class="blank bg-dg">
           <iframe src="https://www.youtube.com/embed/XTsy45o1OnE?HD=1&amp;rel=0&amp;showinfo=0&amp;controls=1&amp;theme=dark&amp;color=white&amp;" frameborder="0" border="0" scrolling="no" allowfullscreen="1" mozallowfullscreen="1" webkitallowfullscreen="1"></iframe>
         </div></li>
<li><p>Editor: Added support for importing texture arrays (<code>Texture2DArray</code>) and volume textures (<code>Texture3D</code>) from "flipbook" image layouts. To use this, open the Texture Importer and see the <em>Shape</em> setting.<br></p></li>
<li><p>Editor: Added support for Roslyn reference assemblies. Unity skips compilation of assembly references if the metadata for the modified assembly does not change when compiling scripts for the editor. Reference assemblies are enabled by default; to disable them, open the Player settings and disable <em>Use Reference Assemblies</em>.</p></li>
<li><p>Editor: Added the ability to optionally drag all the edges from one port to another at the same time.</p></li>
<li><p>Editor: Added the ability to toggle <code>GraphView</code> snap lines on or off in <em>Preferences</em>. If enabled, <code>GraphElements</code> in <code>GraphViews</code> align with one another when moved. If disabled, <code>GraphElements</code> move freely.</p></li>
<li><p>Editor: Modified the built-in Visual Studio C# solution generator to include Root Namespace from Assembly Definition Files in generated C# project files.</p></li>
<li><p>Editor: Renamed <code>auto_quitter</code> to <code>UnityAutoQuitterauto_quitter</code> on all platforms and made it a native program on MacOS and Linux.</p></li>
<li><p>Editor: Updated ProBuilder version to 4.3.1.</p></li>
<li><p>Editor: Updated <a href="https://docs.unity3d.com/Packages/com.unity.probuilder@4.2/manual/index.html">ProBuilder</a> to version 4.2.3.</p></li>
<li><p>Editor: Verified <a href="https://docs.unity3d.com/Packages/com.unity.editorcoroutines@latest">Editor Coroutines</a> package version 1.0.0.</p></li>
<li><p>Editor: Verified <a href="https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@latest">Profile Analyzer(com.unity.performance.profile-analyzer)</a> package.</p></li>
<li><p>GI: Added support for blue noise sampling (as described in Eric Heitz and Laurent Belcour's <a href="https://eheitzresearch.wordpress.com/762-2/">SIGGRAPH 2019 talk</a>).</p></li>
<li><p>Graphics: Added an experimental <code>ExternalGPUProfiler</code> capture API that allows users to programmatically take GPU frame captures using supported GPU debugging tools. See <a href="https://docs.unity3d.com/2020.2/Documentation/ScriptReference/Experimental.Rendering.ExternalGPUProfiler.html">ExternalGPUProfiler</a>.</p></li>
<li><p>Graphics: Added an option to evict data in a region. The original invalidate now keeps the original "stale" data on your graphics hardware until refreshed.</p></li>
<li><p>Graphics: Added an <code>ExtensibleCamera</code> class that inherits properties from the <code>Camera</code> class.</p></li>
<li><p>Graphics: Added Custom Render Texture API, so you can write your own update loop in C#.</p></li>
<li><p>Graphics: Added support for importing 16-bit per-channel integer formats without quantization. This also exposed new <code>TextureFormats</code> R16G16, R16G16B16 &amp; R16G16B16A16.</p></li>
<li><p>Graphics: Added support for Virtual Texturing for Linux Standalone player.</p></li>
<li><p>Graphics: Added the ability to output a CPU event and get it back to the component level.</p></li>
<li><p>Graphics: Added the Virtual Texturing Profiler module to the Unity Profiler, which you can use to get performance information about the Virtual Texturing system.</p></li>
<li><p>Graphics: Added trilinear filtering support for procedural VT.</p></li>
<li><p>Graphics: Added Virtual Texturing support on the Universal Windows Platform.</p></li>
<li><p>IL2CPP: Added <code>Il2CppEagerStaticClassConstructionAttribute</code>, which can help to avoid performance impact associated with static constructors.</p></li>
<li><p>Linux: Added VTune integration support for Linux.</p></li>
<li><p>macOS: Added support for native Apple Silicon and macOS Universal 2 builds.<br></p></li>
<li><p>Mobile: Added Adaptive Performance settings.</p></li>
<li><p>Mobile: Verified <a href="https://docs.unity3d.com/Packages/com.unity.mobile.adaptiveperformance@latest">Adaptive Performance</a> package version 2.0.0.</p></li>
<li><p>Package Manager: Added a UI for users to manage their Scoped Registries from inside the Editor. Also added a popup alert for when Scoped Registries are added to their project from outside that Scoped Registries management UI. The Scoped Registries management UI automatically opens when the popup appears.<br></p> 
<div class="inline-frame rel clear mb20">
           <img src="/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif" class="blank bg-dg">
           <iframe src="https://www.youtube.com/embed/8atK0oOxutk?HD=1&amp;rel=0&amp;showinfo=0&amp;controls=1&amp;theme=dark&amp;color=white&amp;" frameborder="0" border="0" scrolling="no" allowfullscreen="1" mozallowfullscreen="1" webkitallowfullscreen="1"></iframe>
         </div></li>
<li><p>Package Manager: Added advanced Project Settings for the Package Manager.</p></li>
<li><p>Package Manager: Added an option on the Asset Store Has Moved window to skip it in future. If enabled, this setting opens the Asset Store directly in the browser when clicking on <em>Window &gt; Asset Store</em>, and the user will not see the Asset Store Has Moved window again once they close it.</p></li>
<li><p>Package Manager: Added support for distinguishing between operation and state errors.</p></li>
<li><p>Package Manager: Added the <strong>Pause</strong> and <strong>Resume</strong> buttons when downloading Asset Store packages in the <strong>My Assets</strong> context in the Package Manager.</p></li>
<li><p>Package Manager: Added the ability to extract any hyperlinks and display them as text in an Asset Store package description (when in <strong>My Assets</strong> list context). This allows the user to copy them so they can still visit the page (until hyperlinks are supported in descriptions).</p></li>
<li><p>Package Manager: Added the Preview Packages in Use dropdown menu.</p></li>
<li><p>Package Manager: Added <code>changelogUrl</code> and <code>licensesUrl</code> as optional properties that can be specified in the <code>package.json</code> of a custom package. If specified, the auto-generated changelog and license links will be replaced with custom URLs.</p></li>
<li><p>Package Manager: Introduced two new environment variables to override the user and global configuration file path. <code>UPM_GLOBAL_CONFIG_FILE</code> overrides the default path to the global configuration file, and <code>UPM_USER_CONFIG_FILE</code> overrides the default path to the user configuration file.</p></li>
<li><p>Package Manager: Made console log errors from Package Manager UI clearly specify that they are from [Package Manager Window]. Also modified error messages in the UI so that they do not prompt the user to 'see console for more details' if no details are logged in the console.</p></li>
<li><p>Package Manager: Modified the appearance of the Package Manager window to highlight preview packages.</p></li>
<li><p>Package Manager: Modified the package details interface to display the full version of a package, including tags. Removed the '(Current)' note from the release details view of UPM packages.</p></li>
<li><p>Package Manager: Modified the package details interface to display the installation path for locally installed packages.</p></li>
<li><p>Package Manager: Modified the refresh button in the Package Manager window to a drop-down that selects the type of refresh to perform.</p></li>
<li><p>Package Manager: Moved the <em>Enable Preview Packages</em> option in the Package Manager Project Settings window.</p></li>
<li><p>Package Manager: Split the Package Name into Name and Organization.</p></li>
<li><p>Particles: Added Local and Shape Scaling Mode support when using Mesh Renderer and Skinned Mesh Renderer in the Shape module.</p></li>
<li><p>Particles: Modified the Triggers module to query which colliders a particle is interacting with.</p></li>
<li><p>Physics: Expose <code>Joint.connectedArticulationBody</code> to be able to link <code>ArticulationBody</code> and <code>Rigidbody</code> hierarchies together with regular joints.</p></li>
<li><p>Player: Added the ability to pull Unity Player logs after test runs.</p></li>
<li><p>Prefabs: Added support for a Prefab post-processor.</p></li>
<li><p>Profiler: Added the Module Editor, which supports the creation of custom Profiler modules the ability to add charts to the Profiler for either existing or user generated Profiler statistics.</p></li>
<li><p>Scripting: Added support for Roslyn analyzers in Unity projects.<br></p> 
<div class="inline-frame rel clear mb20">
           <img src="/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif" class="blank bg-dg">
           <iframe src="https://www.youtube.com/embed/hbHyArijG3M?HD=1&amp;rel=0&amp;showinfo=0&amp;controls=1&amp;theme=dark&amp;color=white&amp;" frameborder="0" border="0" scrolling="no" allowfullscreen="1" mozallowfullscreen="1" webkitallowfullscreen="1"></iframe>
         </div></li>
<li><p>Scripting: Added support for script compilation with C# 8.</p></li>
<li><p>Services: Added Services Window support for the Unity Distribution Portal.<br></p> 
<div class="inline-frame rel clear mb20">
           <img src="/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif" class="blank bg-dg">
           <iframe src="https://www.youtube.com/embed/m_s9BdNZg1k?HD=1&amp;rel=0&amp;showinfo=0&amp;controls=1&amp;theme=dark&amp;color=white&amp;" frameborder="0" border="0" scrolling="no" allowfullscreen="1" mozallowfullscreen="1" webkitallowfullscreen="1"></iframe>
         </div></li>
<li><p>Shaders: Added scriptable stripping support for compute shaders.</p></li>
<li><p>Shaders: Implemented Shader Live-Link support.</p></li>
<li><p>Shaders: Modified shader preprocessors so that they can be overriden on a per-shader basis.</p></li>
<li><p>UI Toolkit: Added the asset type <code>ThemeStyleSheet</code>.</p></li>
<li><p>UI Toolkit: Added <code>TwoPaneSplitView</code> control.</p></li>
</ul>

### Improvements
<ul>
<li><p>2D: Added a <strong>Detect Contiguous Tiles</strong> toggle to GridBrush when you do a FloodFill. The toggle only changes contiguous Tiles when enabled, and all Tiles of the same type when disabled.</p></li>
<li><p>2D: Added a Copy, Paste and Paste All functionality to the Outline and Physics Shape modules for the Sprite Editor.</p></li>
<li><p>2D: Added ability to delete a selection of Tiles with the Delete/Backspace key when you select Tiles with the Select tool.</p></li>
<li><p>2D: Added ability to specify Corners properties.</p></li>
<li><p>2D: Added custom axis sort to the Tile Palette asset to allow users to show Tiles in the Tile Palette that the custom axis sorts.</p></li>
<li><p>2D: Added message to inform user about dependent packages when they view certain sample Scenes in the Animation package.</p></li>
<li><p>2D: Added support for SpriteShape meshes to be precomputed.</p></li>
<li><p>2D: Added Transform Gizmos for making Transform changes to a Grid Selection for a Scene view.</p></li>
<li><p>2D: Adjusted the length of the popup and value fields for the Skinning Module's <em>Weight Slider</em> window.</p></li>
<li><p>2D: Implemented repainting of the Tile Palette when you make changes to a Grid Selection for a Tile Palette.</p></li>
<li><p>2D: Improved deformation performance when Collection and Burst package is installed.</p></li>
<li><p>2D: Improved Memory Allocations.</p></li>
<li><p>2D: Improved performance in SceneView for SceneViewOpenTilePaletteHelper.</p></li>
<li><p>2D: Improved performance of TilemapRenderer Individual mode.</p></li>
<li><p>2D: Improved the memory and speed of <code>Animation.SpritePostProcess</code> when used for a large sprite count.</p></li>
<li><p>2D: Improved the organization of the 2D Menus to allow for easier creation of default assets and GameObjects. This will improve user experience in level white boxing and prototyping.</p></li>
<li><p>2D: Improved the Sprite Skin Editor UI.</p></li>
<li><p>2D: Improved user experience of FloodFill tool from the Tile Palette when previewing the results of FloodFill.</p></li>
<li><p>2D: Updated 2D template to use current verified version of 2D packages.</p></li>
<li><p>2D: Updated Bone Influence window to allow you to rearrange the order of bones in the Sprite Skin Inspector.</p></li>
<li><p>AI: Added tooltips to Navigation window and related components. (<a href="https://issuetracker.unity3d.com/issues/navmesh-tool-tips-are-missing-for-navmesh-agent">970778</a>)</p></li>
<li><p>Android: Added anti-piracy measures which print your Company Name and Product Name in the log during application start. This can be used to prove that the game is yours if someone pirates it.</p></li>
<li><p>Android: Added support for compressed 3D textures with OpenGL ES 3.1.</p></li>
<li><p>Android: Added support for Vulkan backbuffer pre-rotation.</p></li>
<li><p>Android: Added target display support for Android.</p></li>
<li><p>Android: Added update so that frame rate is decided automatically when optimized frame pacing is enabled and Vsync is disabled.</p></li>
<li><p>Android: Enabled support for Light Probe proxy volumes when using OpenGL ES 3.</p></li>
<li><p>Android: Improved documentation for Application.targetFrameRate behavior on mobile devices.</p></li>
<li><p>Android: Improved logging when you try to find a plugin that is missing. (<a href="https://issuetracker.unity3d.com/issues/android-unable-to-find-lib-burst-0-0-and-burst-0-0-message-logged-when-burst-is-enabled">1268172</a>)</p></li>
<li><p>Android: Improved <code>Application.genuine implementation</code>, so it checks that the package name set in Player Settings matches with the one acquired at runtime.</p></li>
<li><p>Android: Improved <code>Screen.currentResolution.refreshRate</code> to correct itself if the display refresh rate changes.</p></li>
<li><p>Android: Improved <code>Screen.resolutions</code> to include supported display resolutions for 4K detection. (<a href="https://issuetracker.unity3d.com/issues/mobile-systemwidth-isnt-set-to-renderingwidth-or-currentresolution-dot-width">1178233</a>)</p></li>
<li><p>Android: Moved <code>noCompress</code> settings from launcher project to <code>unitylibrary</code>. (1239760)</p></li>
<li><p>Android: Optimized async texture readback and CopyTexture when using Vulkan on Mali GPUs.</p></li>
<li><p>Android: Updated <a href="https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.2/manual/index.html">Android Logcat</a> package to version 1.1.1.</p></li>
<li><p>Animation: Improved warnings for animated property curve names by minimizing false-positives and lessening repeated logs.</p></li>
<li><p>Animation: Localized some terms in the Animation window.</p></li>
<li><p>Asset Import: Added support for 3DsMax's Simplified Physical Material from FBX files in the Model Importer.</p></li>
<li><p>Asset Import: Asset previews are generated as a separate step after importing an asset.</p></li>
<li><p>Asset Import: Improved search speed when using glob syntax to search project assets.</p></li>
<li><p>Asset Import: Improved UV unwrapper performance.</p></li>
<li><p>Asset Import: Made <code>AssetDatabaseExperimental.SetImporterOverride</code> accessible from the Inspector. You can now access it in any Asset Importer header by selecting an available Importer Override to apply.</p></li>
<li><p>Asset Pipeline: Improved the adb Profiler output in the Editor log so it only gives necessary information.</p></li>
<li><p>Asset Pipeline: Removed unnecessary additional domain reloads associated with asset import workers.</p></li>
<li><p>Asset Pipeline: Unity no longer needs to reimport all textures, audio, and video when switching between Standalone platforms (for example, Win32 to Win64, or Mac to Linux).</p></li>
<li><p>Asset Pipeline: Updated progress dialog to display more precise information when asset postprocess callbacks take a long time to finish. (1228418)</p></li>
<li><p>Asset Pipeline: Updated source asset dependencies to use both file hash and timestamp to decide when to reload an asset.</p></li>
<li><p>Audio: Updated audio previews so that they stop when Unity loses focus and <em>Run in Background</em> is disabled.</p></li>
<li><p>Bug Reporter: Updated <code>services-config.json</code> to add ability to set Bug Reporter defaults for <em>Publicity</em> and <em>CustomerEmail</em>, and to set whether to exclude project files.</p></li>
<li><p>Build Pipeline: Added support to obtain GameCore redist DLLS from locally installed MSVC instances.</p></li>
<li><p>Burst: Added support for External symbols on a platform that required it.</p></li>
<li><p>Core: Improved Time.deltaTime consistency for the Metal graphics API on iOS and macOS.</p></li>
<li><p>DX12: Added support for constant buffers set with the <code>CommandBuffer.SetGlobalConstantBuffer</code> and <code>Shader.SetGlobalConstantBuffer</code> methods in Ray Tracing Shaders. Fixed and improved all the Ray Tracing-related Scripting API documentation.</p></li>
<li><p>DX12: Added support for GraphicsBuffer constant buffers that can be set using <code>ComputeShader.SetConstantBuffer</code> and <code>CommandBuffer.SetComputeConstantBufferParam</code>.</p></li>
<li><p>DX12: Added support for GraphicsBuffer constant buffers that can be set using <code>RayTracingShader.SetConstantBuffer</code> and <code>CommandBuffer.SetRayTracingConstantBufferParam</code>.</p></li>
<li><p>DX12: Ensured that values are only filled in for available channels when reading vertex attributes from vertex buffers (closest hit / any hit shaders). Unavailable channel values do not default to 0.</p></li>
<li><p>DX12: Improved CPU performance when binding raytracing shaders.</p></li>
<li><p>DX12: Improved CPU performance when building Ray Tracing Acceleration Structures.</p></li>
<li><p>DX12: Improved CPU performance when dispatching Ray Tracing Shaders.</p></li>
<li><p>DX12: Updated skin pose buffer to use scratch buffer memory, so that updates do not trigger an upload operation.</p></li>
<li><p>Editor: Added "Set as Default" option to Hierarchy objects so that users can set a custom parent GameObject for GameObjects they drag into the Scene/Hierarchy windows, and GameObjects they create via the GameObject menu.</p></li>
<li><p>Editor: Added a label displaying how many Game Objects are currently selected in the Inspector. (1208698)</p></li>
<li><p>Editor: Added a new naming scheme option to Editor Settings. This is set to <em>Prefab (1)</em> by default, or you can choose <em>Prefab.1</em> or <em>Prefab_1</em>.</p></li>
<li><p>Editor: Added ability to copy and paste arrays and user-written serializable classes and structs in the Inspector.</p></li>
<li><p>Editor: Added ability to create keyboard shortcuts to copy and paste camera positions. In the shortcut settings, these are <em>Scene View/Copy Camera Placement</em>, <em>Scene View/Paste Camera Placement</em> and <em>Game View/Copy Camera Placement</em>. No default keys are assigned.</p></li>
<li><p>Editor: Added optional "thickness" parameter functions for <code>Handle</code>: <code>DrawLine</code>, <code>DrawWireDisc</code> and <code>DrawWireArc</code>, for drawing thick handles.</p></li>
<li><p>Editor: Added Recent Scenes to the File menu in the Toolbar.</p></li>
<li><p>Editor: Added shift + select functionality to various tree view windows (e.g. Hierarchy, Project) to enable you to select multiple items without deselecting previously selected items.</p></li>
<li><p>Editor: Added support for Ray Tracing Shader (DX12) which sends information to the Frame Debugger.</p></li>
<li><p>Editor: Added support for the Scene view's <em>Shaded Wireframe</em> mode to work with SRPs, via <code>ScriptableRenderContext.DrawWireOverlay</code>.</p></li>
<li><p>Editor: Added support for Undo and Redo for moving and renaming assets in the Project view.</p></li>
<li><p>Editor: Added support for <code>GradientFields</code> and Gradient editor to have their color interpreted as linear.</p></li>
<li><p>Editor: Added the ability to use Ctrl+C on a focused progress dialog in Windows Editor to copy the progress text to clipboard.</p></li>
<li><p>Editor: Added the command line argument "vcsModeSession", which sets VCS mode for the current Editor session only. (<a href="https://issuetracker.unity3d.com/issues/vcsmode-cli-argument-writes-to-projectsettings-slash-editorsettings-dot-asset">1226304</a>)</p></li>
<li><p>Editor: Added tooltips to Editor status bar icons.</p></li>
<li><p>Editor: Enhanced the <strong>Open</strong> context menu so that it expands the folders in One Column Layout in the Project Browser. (<a href="https://issuetracker.unity3d.com/issues/folders-are-opening-when-trying-to-open-them-from-editor">1243843</a>)</p></li>
<li><p>Editor: Improved how assert user messages are displayed in the Console view, so the user message for an assert can be read in the Console without needing to look at expanded details.</p></li>
<li><p>Editor: Improved inspector performance for large text asset files. (<a href="https://issuetracker.unity3d.com/issues/editor-keeps-repainting-continuously-when-selecting-a-txt-file-that-contains-binary">1241212</a>)</p></li>
<li><p>Editor: Improved Move/Rotate/Scale handles: thicker lines, brighter colors, increased movement accuracy, better visibility, and other UI improvements.</p></li>
<li><p>Editor: Improved performance of Scene hierarchy when you select GameObjects in the Project view. (1252528)</p></li>
<li><p>Editor: Improved progress bar details for texture importing, including details on crunch compression and cubemap convolution.</p></li>
<li><p>Editor: Improved Project Browser window to show asset file path whilst in One Column mode. (<a href="https://issuetracker.unity3d.com/issues/assets-path-is-not-shown-when-using-one-column-layout-in-the-project-window">1200880</a>)</p></li>
<li><p>Editor: Improved ray direction calculations so they are relative to the camera instead of a direction in world space. This should significantly improve precision when interacting with handles far away from the origin. (1178966)</p></li>
<li><p>Editor: Improved script creation so that Unity no longer writes a UTF8 BOM to new scripts it creates. This removes problems that BOM's can cause with tools such as source control.</p></li>
<li><p>Editor: Improved scripting defines list cut/copy/paste functionality. (1287729)</p></li>
<li><p>Editor: Improved scroll smoothness in Editor in macOS.</p></li>
<li><p>Editor: Improved the Layouts menu and dialogs. Layout deletion is now under a submenu and has a confirmation dialog. Save layout now has a confirmation dialog when overwriting an existing layout. The menu item "Revert Factory Settings"  has been renamed to "Reset All Layouts". The Layouts dropdown in main toolbar is wider. Save Layout to File now shows the file in file explorer.</p></li>
<li><p>Editor: Improved the time taken for mobile ETC/ETC2/EAC texture compression.</p></li>
<li><p>Editor: Improved <code>JobsDebugger</code> performance.</p></li>
<li><p>Editor: Minimized allocations when calculating bounds for the <em>Rect Tool</em>.</p></li>
<li><p>Editor: Modified prefabs in the Hierarchy window so that certain Version Control state icons (Out of Sync, Conflicted, Remote Locked, Remote Delete, Remote Checkout) will be displayed (if enabled in the Project Settings window).</p></li>
<li><p>Editor: Optimized Gizmo rendering; now is ~5x faster when many gizmos are visible.</p></li>
<li><p>Editor: Optimized style catalog asset post-processing. (1222761)</p></li>
<li><p>Editor: Released <a href="https://docs.unity3d.com/Packages/com.unity.quicksearch@1.1/manual/index.html">Quick Search</a> package version 1.5.3 with minor fixes, and improved test stability regarding Asset Store.</p></li>
<li><p>Editor: Removed redundant preview packages message from the title bar.</p></li>
<li><p>Editor: Replaced the text field for Scripting Define Symbols in Project Settings with a foldout string array.</p></li>
<li><p>Editor: Updated Frame Selected so that pressing it a second time focuses on the GameObject's handle/gizmo.</p></li>
<li><p>Editor: Updated Inspector so that you can re-order arrays and lists. To enable this, use the <code>[Reorderable]</code> attribute on your script variables.</p></li>
<li><p>Editor: Updated Mesh Inspector to add <em>Pan</em>, <em>Zoom</em> and <em>Blendshape Preview</em>.</p></li>
<li><p>Editor: Updated Polybrush to 1.0.2.</p></li>
<li><p>Editor: Updated Quick Search to 2.0.<br></p> 
<div class="inline-frame rel clear mb20">
           <img src="/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif" class="blank bg-dg">
           <iframe src="https://www.youtube.com/embed/5xGLXxsm7QM?HD=1&amp;rel=0&amp;showinfo=0&amp;controls=1&amp;theme=dark&amp;color=white&amp;" frameborder="0" border="0" scrolling="no" allowfullscreen="1" mozallowfullscreen="1" webkitallowfullscreen="1"></iframe>
         </div></li>
<li><p>Editor: Updated Scene View to accept multiple objects when dragging and dropping.</p></li>
<li><p>Editor: Updated Settings Provider example and doc.</p></li>
<li><p>Editor: Updated the Game View resolution dropdown for Standalone platform with a more comprehensive list of default aspect ratios (16:9, 16:10) and resolutions (1920x1080, 1366x768, 2560x1440, 3840x2160).</p></li>
<li><p>Editor: Updated the material preview in the Inspector to remember the last used preview mesh.</p></li>
<li><p>Editor: Updated the Quick Search window to version 1.5.2, including minor fixes and improved performance.</p></li>
<li><p>Editor: Updated the UI for background tasks and main toolbar.</p></li>
<li><p>Editor: Updated to ProBuilder 4.4.0.</p></li>
<li><p>Editor: Updated UI so that Scene view deselect-click (Ctrl/Cmd) works more intuitively with prefabs that contain child GameObjects.</p></li>
<li><p>Editor: Updated Unity so it no longer treats layers 3, 6 and 7 as reserved. (1264751)</p></li>
<li><p>GI: Added API to get or set the Lighting Setting Asset for loaded scenes.</p></li>
<li><p>GI: Added support for half float texture format for Light Probe Proxy Volume (LPPV) component. You can now choose the format of the 3D LPPV texture from the LPPV inspector.</p></li>
<li><p>GI: Ensured that correct, official AMD graphics card names are displayed in the Lighting window GPU device dropdown.</p></li>
<li><p>GI: Improved Lighting Settings such as preset support, updated related docs and exposed default settings.</p></li>
<li><p>GI: Improved scheduling of lightmaps, light probes and additional probe bakes with the GPU lightmapper.</p></li>
<li><p>GI: Improved speed of GI main thread initialization on Editor startup. (<a href="https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup">1162775</a>)</p></li>
<li><p>GI: Improved the com.unity.rendering.hybrid package by forcing all lightmaps to max atlas size so that they can be stored in texture arrays.</p></li>
<li><p>GI: Reduced GPU memory usage when you bake large lightmaps with the GPU lightmapper. Achieved by baking in smaller tiles in non progressive mode.</p></li>
<li><p>GI: Removed custom Lighting Settings from 3D template.</p></li>
<li><p>GI: Updated Light Probe Proxy Volumes components so that they only update once per frame, rather than once per camera render, because these components are not camera relative.</p></li>
<li><p>GI: Upgraded Radeon denoiser to use RIF 1.5.1.2. This will only attempt to run on GPUs with at least 4GB of memory, becuase this is required by the AI model.</p></li>
<li><p>Graphics: A warning message appears when a users sets a UV out of range in the RecalculateUVDistributionMetric C# function.</p></li>
<li><p>Graphics: Added <strong>Shader Precision Model</strong> to the Player Settings, which allows you to change between current platform defaults and the new Unified Model. The Unified Model defaults to full sampler precision on all platforms, but allows explicit declarations of lower precision and using FP16 ops on targets where this is available. (1280157)</p></li>
<li><p>Graphics: Added debug names for resources on DX12.</p></li>
<li><p>Graphics: Added generated warnings when you use an unsupported CommandBuffer API inside a Render Pass.</p></li>
<li><p>Graphics: Added support for ASTC decode mode RGB9E5 for ASTC HDR textures. This only works when there is no alpha channel in use.</p></li>
<li><p>Graphics: Added support for DXT5nm normal maps on Android, iOS, tvOS. (1235914)</p></li>
<li><p>Graphics: Added the option to delay acquiring the swapchain buffer until it is actually used when rendering in Vulkan.</p></li>
<li><p>Graphics: Copy spawn count because we can process several time Init/Update per frame. (<a href="https://issuetracker.unity3d.com/issues/vfx-thread-group-size-must-be-above-zero-error-is-thrown-continuously-when-exact-fixed-time-update-mode-is-enabled">1268360</a>)</p></li>
<li><p>Graphics: Disabled rendering to color channels during a Scriptable Render Pipeline shadow pass, to improve performance.</p></li>
<li><p>Graphics: Enabled threaded texture creation on Xbox DX11 to remove frame spikes. Added support for direct upload of offline processed data on DX12 when threaded texture creation is disabled.</p></li>
<li><p>Graphics: Enhanced colorspace switching to only recreate textures with colorspace sensitive formats (for example DXT1_sRGB/UNorm).</p></li>
<li><p>Graphics: Ensured that ComputeBuffer counters are put into separate physical buffers to impove data access/alignment for the Metal API.</p></li>
<li><p>Graphics: Extended supported types/formats for RWTexture2D when using Vulkan and OpenGL ES.</p></li>
<li><p>Graphics: Improved ComputeBuffer data alignment for Metal.</p></li>
<li><p>Graphics: Improved DX12 async texture loading so that when out of GPU memory, it returns a failure state, reports an error and cleans up memory.</p></li>
<li><p>Graphics: Improved DX12 performance when Unity creates a lot of resources per frame.</p></li>
<li><p>Graphics: Improved DX12 performance with the hybrid renderer.</p></li>
<li><p>Graphics: Improved error reporting in the Ray Tracing shaders interface.</p></li>
<li><p>Graphics: Improved input validation of RenderPass API.</p></li>
<li><p>Graphics: Improved performance by initializing the intermediate tree renderer with AABB::zero instead of NaN.</p></li>
<li><p>Graphics: Improved shader property error messages.</p></li>
<li><p>Graphics: Improved texture creation performance for cube maps on Metal.</p></li>
<li><p>Graphics: Improved texture creation performance for cube maps on Vulkan.</p></li>
<li><p>Graphics: Improved texture creation performance for CubeMaps on PC and Xbox on DX11 and DX12, and PS4.</p></li>
<li><p>Graphics: Improved the error messaging interface which appears when texture stacks are set up incorrectly.</p></li>
<li><p>Graphics: Improved validation of <code>RenderTexture</code> with bindTextureMS for unsupported formats.</p></li>
<li><p>Graphics: Increased draw calls per command list to improve URP Shadow Pass performance when rendering cascaded shadow maps.</p></li>
<li><p>Graphics: Metal: Add changes required for Apple GPU support on a Mac.</p></li>
<li><p>Graphics: Optimized D3D12 Constant Buffers for per-Pass binding.</p></li>
<li><p>Graphics: Reduced shader compilation times and application build sizes for GLSL/Metal platforms.</p></li>
<li><p>Graphics: Updated the D3D12 internal command buffer to allow access from a D3D12 native plugin.</p></li>
<li><p>GraphView: Added capability support to stacks, child stacks, and groups to better avoid unsupported behaviors, specifically with grouping and heterogeneous selections.</p></li>
<li><p>IL2CPP: Added attribute to avoid runtime performance impact of static constructors.</p></li>
<li><p>IL2CPP: Fixed a GC performance regression on Android and Linux.</p></li>
<li><p>IL2CPP: Improved error message when required Visual Studio components are not installed when building for Windows.</p></li>
<li><p>IL2CPP: Parallel IL2CPP Conversion is now default to improve IL2CPP build performance.</p></li>
<li><p>IL2CPP: Reduced the number of error messages produced by an IL2CPP failure from two to one.</p></li>
<li><p>iOS: Added support for custom storyboards on iOS.</p></li>
<li><p>iOS: Changed built-in .xib launch screens to storyboard.</p></li>
<li><p>iOS: Improved how version defines in Trampoline are generated so all versions are supported and they can be compared numerically. (<a href="https://issuetracker.unity3d.com/issues/ios-unity-version-in-unitytrampolineconfigure-dot-h-is-higher-in-earlier-unity-versions-compared-to-newer-versions">1244796</a>)</p></li>
<li><p>iOS: Modified <code>Camera.targetDisplay</code> to work with iOS Metal. (<a href="https://issuetracker.unity3d.com/issues/mobile-multi-display-doesnt-work-on-secondary-displays-using-lwrp">1171951</a>)</p></li>
<li><p>iOS: Under some circumstances, interim AA resolve no longer results in an extra texture copy.</p></li>
<li><p>Kernel: Fixed issue where Unity would crash when passing an empty filename to <code>AsyncReadManager.Read</code>.</p></li>
<li><p>Kernel: Optimized the low-level atomic queue container used by the <code>JobQueue</code>.</p></li>
<li><p>Kernel: Reduced job system overhead on macOS.</p></li>
<li><p>Kernel: Reduced main thread overhead of creating job reflection data.</p></li>
<li><p>Kernel: Reduced the time it takes to enter Play mode with many IJobChunk-style Burst compiled jobs.</p></li>
<li><p>Kernel: Refactored memory label code, for a lower generated code size.</p></li>
<li><p>Kernel: Removed the unneccesary parallel for access restrictions for <code>IJobFor.Schedule</code></p></li>
<li><p>macOS: Removed project name in the window title bar.</p></li>
<li><p>Mobile: Added VRR support.</p></li>
<li><p>Mobile: Improved Provider Stats reporting.</p></li>
<li><p>Mobile: Updated com.unity.mobile.notifications to 1.3.2.</p></li>
<li><p>Mobile: Updated verified package Adaptive Performance and Samsung provider to 1.1.6.</p></li>
<li><p>Mobile: Updated <a href="https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@2.1/manual/index.html">Adaptive Performance Samsung Android</a> package to version 1.1.1.</p></li>
<li><p>Package: Updated input system package to 1.0.1. (<a href="https://issuetracker.unity3d.com/issues/input-system-after-package-install-the-update-slash-switch-and-restart-prompt-does-not-appear">1292513</a>)</p></li>
<li><p>Package Manager: Added a clearer error message that appears when the UnityPackageManager program is missing.</p></li>
<li><p>Package Manager: Added a loading screen to the Package Manager to give visual feedback when you install a package from a Git URL.</p></li>
<li><p>Package Manager: Added support for returning enterprise entitlement packages from the <code>PackageManager.Client.SearchAll()</code> method. These packages now show in the Package Manager UI <strong>Unity Registry</strong> section when users have the entitlement to use them.</p></li>
<li><p>Package Manager: Added the Package Manager lock file (<code>Packages/packages-lock.json</code>) to the <em>Bug Reporter</em> report.</p></li>
<li><p>Package Manager: Added tooltips to action buttons for packages.</p></li>
<li><p>Package Manager: Improved package interoperability with Unity IAP. Added functionality for Unity IAP package to work directly with UDP Package instead of maintaining it's own UDP.dll.<br> Enabled user permissions to be set at Project level.<br>
Updated UDP settings so that inspector window opens when you invoke the asset file. This allows for faster load and sync times.<br>
Refined general code.</p></li>
<li><p>Package Manager: Improved performance of Package Manager metadata requests sent to the registry.</p></li>
<li><p>Package Manager: Improved visibility of <strong>Import</strong> and <strong>Download</strong> buttons.</p></li>
<li><p>Package Manager: Updated dependency resolution so that it automatically resolves trivial conflicts.</p></li>
<li><p>Package Manager: Updated Unity Package Manager so that it caches state on disk, to improve project loading time.</p></li>
<li><p>Package Manager: Upgraded Cinemachine to 2.6.1.</p></li>
<li><p>Particles: Added a button to the Particle System UI to identify ownership of the system for sub-emitters.</p></li>
<li><p>Particles: Added a new Depth sorting mode, to sort particles based on their distance from the camera plane. (<a href="https://issuetracker.unity3d.com/issues/shuriken-particle-sort-mode-by-distance-does-not-take-depth-into-account-when-particles-are-aligned-by-view">1207573</a>)</p></li>
<li><p>Particles: Improved performance by removing unnecessary calls to <code>ParticleSystemRenderer::UpdateCachedMesh</code>. This especially improves performance of enabling or disabling ParticleSystemRenderers that use meshes consisting of Triangle Strip geometry. (<a href="https://issuetracker.unity3d.com/issues/particles-updatecachedmesh-needlessly-called-when-disabling-thne-enabling-a-particlesystemrenderer">1271169</a>)</p></li>
<li><p>Particles: Improved the Collision and Trigger Modules so they can have any number of colliders.</p></li>
<li><p>Physics: Added tooltips for some of the physics settings in the Editor. (<a href="https://issuetracker.unity3d.com/issues/imgui-auto-sync-transforms-property-tooltip-missing-under-physics-in-the-project-setting-window">1268052</a>)</p></li>
<li><p>Physics: Added tooltips to the properties exposed in the ArticulationBody inspector. (<a href="https://issuetracker.unity3d.com/issues/imgui-articulation-body-components-tooltips-are-missing">1256304</a>)</p></li>
<li><p>Physics: Implemented visualisers for articulation body joint limits (both linear and angular). This update applies to revolute, prismatic and spherical joints.<br></p> 
<div class="inline-frame rel clear mb20">
           <img src="/profiles/unity3d/themes/unity/images/assets/elements/blank-1080.gif" class="blank bg-dg">
           <iframe src="https://www.youtube.com/embed/HCJ9DC6eAvU?HD=1&amp;rel=0&amp;showinfo=0&amp;controls=1&amp;theme=dark&amp;color=white&amp;" frameborder="0" border="0" scrolling="no" allowfullscreen="1" mozallowfullscreen="1" webkitallowfullscreen="1"></iframe>
         </div></li>
<li><p>Prefabs: Added <strong>Create Prefab</strong> item to the asset menu, so you can create and start editing a new Prefab Asset without interfering with the current scene.</p></li>
<li><p>Prefabs: Improved the performance of nested Prefab modification saving.</p></li>
<li><p>Prefabs: Improved the performance of Prefabs in the Editor.<br></p></li>
<li><p>Prefabs: Improved the performance of the prefab editor.</p></li>
<li><p>Prefabs: Introduced the <strong>Allow Auto Save</strong> Project Setting for Prefab Mode. It is enabled by default, which matches the same behavior in previous versions of Unity. However, if you disable this setting, Unity does not auto save while in Prefab Mode, and the toggle is not displayed. This is different to the main Auto Save toggle, which is a per-user setting that carries across projects. This new setting applies to all users of the project. (1141476)</p></li>
<li><p>Prefabs: Prefabs with a lot of properties load faster than before.</p></li>
<li><p>Profiler: Added a progress bar when loading and saving Profiler data.</p></li>
<li><p>Profiler: Added a visualization for Async Loading flow in the CPU Profiler Timeline view.</p></li>
<li><p>Profiler: Added ability to specify a Profiler category for ProfilerMarker.</p></li>
<li><p>Profiler: Added an option to specify a port in the direct Profiler connection UI.</p></li>
<li><p>Profiler: Added the ability to see the metadata associated with a Profiler sample in the Hierarchy View of the CPU Profiler module.</p></li>
<li><p>Profiler: Aligned the Memory and Rendering Profiler module detailed panel test with runtime counter names.</p></li>
<li><p>Profiler: Burst jobs have a different color from normal jobs in CPU Profiler Timeline view.</p></li>
<li><p>Profiler: Changed the load icon in the Profiler window so that it clearly represents loading better.</p></li>
<li><p>Profiler: Fixed an issue where the Profiler window did not process small frames immediately when they come to Profiler Window. (1260269)</p></li>
<li><p>Profiler: Improved the handling of message sending and receipt in <code>PlayerConnection</code>, and split the receipt of messages across multiple frames.</p></li>
<li><p>Profiler: Optimized Profiler Window chart updates.</p></li>
<li><p>Profiler: Updated the Hierarchy and Timeline view to no longer display frame data while profiling unless the "Live" toggle is enabled. This reduces the Editor overhead while profiling the Editor or Play mode.</p></li>
<li><p>Scripting: Added a way to get the stack trace without garbage collection in the Editor.</p></li>
<li><p>Scripting: Added inline documentation, constructors and implicit conversion operators to <code>LazyLoadReference</code>.</p></li>
<li><p>Scripting: Added support for new managed code stripping annotation attributes.</p></li>
<li><p>Scripting: Implemented switching code coverage without needing to restart the Editor. Introduced API to enable/disable code coverage.</p></li>
<li><p>Scripting: Improved performance of the Memory Profiler.</p></li>
<li><p>Scripting: Improved performance of <code>DefineConstraintsHelper</code>.</p></li>
<li><p>Scripting: Improved the query time of Camera.main.</p></li>
<li><p>Scripting: Improved UnsafeUtility.Malloc so that it throws an exception when it is given a positive alignment value that is not also a power of two. Previously this was only flagged as an assert in debug builds.</p></li>
<li><p>Scripting: Improved <code>UnityWebRequest.certificateHandler</code> so it is now invoked for root certificates on Windows.</p></li>
<li><p>Scripting: Updated AtomicSafetyHandle to throw ObjectDisposedExceptions instead of InvalidOperationException when code attempts to access a container after it has been disposed. This mimics the behavior of built-in container types.</p></li>
<li><p>Scripting: Updated Unity to invoke crash handler when Mono runtime encounters an abort or assert.</p></li>
<li><p>Scripting: When an instruction pointer is null, it obtains a full call stack to prevent a crash from happening.</p></li>
<li><p>Scripting: When Unity fails to load a .dll file, a detailed error message is displayed.</p></li>
<li><p>Scripting Upgrade: Added update to avoid logging potentially misleading messages when no assemblies successfully update.</p></li>
<li><p>Serialization: Increased the allowed serialization depth to allow Unity serialize larger, more complex data models.</p></li>
<li><p>Shaders: Added indentation to the compute shader preprocessed source.</p></li>
<li><p>Shaders: Added support for Caching Shader preprocessor to recognise ellipsises (but there is no variadic macros support).</p></li>
<li><p>Shaders: Added the ability to toggle #line directives on and off via a toggle in Shader and Compute Shader inspectors.</p></li>
<li><p>Shaders: Enabled shader live link to cache compilation results on disk.</p></li>
<li><p>Shaders: Improved #line directive output for preprocessed source.</p></li>
<li><p>Shaders: Improved preprocessed source so it is saved in a text file with a different name from compiled source.</p></li>
<li><p>Shaders: Improved the readability of the error produced when SV_VertexID semantic is used with OpenGL ES 2.</p></li>
<li><p>Shaders: Reduced in-Editor memory usage for Compute shaders.</p></li>
<li><p>Shaders: Updated shader live link to only build one shader variant at player build time.</p></li>
<li><p>Terrain: Added "Delete Brush..." button to the brush selection UI.</p></li>
<li><p>Terrain: Added a <strong>Hole Edge Padding</strong> option to terrain Detail Prototype to control how far details objects will be from the hole edge.</p></li>
<li><p>Terrain: Added a warning message that appears after you select a detail prototype, if Terrain cannot hold all the detail GameObjects when you paint at maximum density. (<a href="https://issuetracker.unity3d.com/issues/target-strength-appears-to-be-way-too-strong">1248486</a>)</p></li>
<li><p>Terrain: Added warnings which occur if you paint too many detail objects on terrain. Unity will now draw red boxes highlighting these areas in the scene view and display an error message explaining the issue. (<a href="https://issuetracker.unity3d.com/issues/hitting-the-upper-bound-of-detail-meshes-causes-previously-placed-detail-meshes-to-dissappear">1248488</a>)</p></li>
<li><p>Terrain: Made Terrain per-frame CPU updates less resource-intensive.</p></li>
<li><p>UI: Added secondary list of graphics that are raycast targets to <code>CanvasUpdateRegistry</code>. This prevents iterating over the whole list every frame.</p></li>
<li><p>UI: Added the ability to have wrap around navigation for horizontal and vertical navigation.</p></li>
<li><p>UI: Added the ability to toggle the "Maskable" option from the Inspector as well as from a script.</p></li>
<li><p>UI: Improved UIStruct memory to use bitfields to save.</p></li>
<li><p>UI: Updated documentation for <code>OnRectTransformDimensionsChange</code> to clarify when it can be called.</p></li>
<li><p>UI: Updated UI to save the value of <code>.Count</code> when iterating through loops, instead of accessing it every time.</p></li>
<li><p>UI: Updated <code>ColorBlock</code> to default to a static colorblock.</p></li>
<li><p>UI: Updated <code>GraphicRaycaster</code> <code>eventCamera</code> implementation to cache some calls for performance.</p></li>
<li><p>UI Toolkit: Added import of FontAsset via USS to UI Toolkit. (1266414)</p></li>
<li><p>Universal Windows Platform: Added warnings to Player Settings if any of the required icon images are not set, to alert the user that missing images will result in the application failing Windows certification.</p></li>
<li><p>Version Control: Improved Smart Merge (UnityYamlMerge) so it now sets premerge base to file in correct base values instead of leaving them blank. Blank premerge base values can still be configured - see mergerules.txt for an example.</p></li>
<li><p>Version Control: Updated existing version control icons. Added theme support.</p></li>
<li><p>Windows: Improved <code>Time.deltaTime</code> consistency for D3D11 graphics API.</p></li>
<li><p>Windows: Improved <code>Time.deltaTime</code> consistency for D3D12 graphics API.</p></li>
<li><p>XR: Improved XR Statistics so it caches thread-safe stats that only get promoted to 'live' data after a render pass. A number of data points need to be 'initialized' before you can render a frame.</p></li>
<li><p>XR: Reduced unnecessary Vulkan backbuffer allocations.</p></li>
<li><p>XR: Updated verified packages for AR Foundation and related packages.</p></li>
<li><p>XR: Updated Windows Mixed Reality XR Plugin verified version to 4.1.1.</p></li>
<li><p>XR: Updated XR Plug-in Management to 3.2.16, Update Windows MR XR Plug-in to 4.2.1.</p></li>
</ul>

### Changes
<ul>
<li><p>2D: Added a contextual helper in the Scene view to open the Tile Palette window that appears when you select a GameObject which can be edited with the Tile Palette window.</p></li>
<li><p>2D: Added support for user to edit Tile Palettes with Brushes. For this to work, the Tile Palette must be empty and unlocked, and the Editor must be in Edit mode.</p></li>
<li><p>2D: Added the correct URL to the Tile help icon.</p></li>
<li><p>2D: Removed the <em>Reset Bounds</em> button from the Sprite Skin Editor.</p></li>
<li><p>2D: Removed Tile <em>Create Asset</em> menu item.</p></li>
<li><p>2D: Updated Scriptable Brushes to use <code>layoutGrid</code> for <code>GridBrushEditorBase</code> preview calls.</p></li>
<li><p>Android: Moved <code>UnityEngine.Android.AndroidDevice</code> from <code>UnityEngine.dll</code> to <code>UnityEngine.AndroidJNIModule.dll</code>.</p></li>
<li><p>Android: Moved <code>UnityEngine.Android.Permission</code> from <code>UnityEngine.dll</code> to <code>UnityEngine.AndroidJNIModule.dll</code>.</p></li>
<li><p>Android: Updated gradle template to use <code>enableR8</code> setting in <code>gradle.properties</code> instead of <code>useProguard</code>.</p></li>
<li><p>Android: Upgraded Android Gradle Plugin to 3.6.0 and Gradle to 5.6.4.</p></li>
<li><p>Asset Import: Changed the default material import mode of the model importer from 'Standard' to 'Import via MaterialDescription'.</p></li>
<li><p>Asset Pipeline: Only accept protocol &gt;=TLSv1.2. SECURITY-1828.</p></li>
<li><p>Audio: Updated DSPGraph so that the interleaving of samples in the output buffer happen inside Unity, rather than third-party output hook implementations</p></li>
<li><p>Build Pipeline: Updated build pipleline to always add a copy of the managed symbols to a <code>Temp/ManagedSymbols</code> folder during a build.</p></li>
<li><p>Burst: Asserts that are currently discarded no longer discard arguments with potential side effects.</p></li>
<li><p>Burst: Changed the version of com.unity.mathematics to 1.2.1.</p></li>
<li><p>Burst: Temporarily removed the Burst compiler warning about exception throws not in [Conditional("ENABLE_UNITY_COLLECTIONS_CHECKS")] methods, to let us address user feedback. The next minor version of Burst will reincorporate this in a more friendly manner.</p></li>
<li><p>Burst: Unity temporarily disables <code>Debug.Log</code> output to avoid a deadlock on a domain reload, when used in Burst function pointers and jobs. A fix for the Unity Editor is being developed.</p></li>
<li><p>Compute: Changed the result to NaN from 0 when a 0 is divided by 0. (<a href="https://issuetracker.unity3d.com/issues/the-value-of-a-float-or-double-field-becomes-0-when-inputting-0-slash-0-in-the-inspector">1257445</a>)</p></li>
<li><p>Editor: As part of gizmo optimizations, we've made many gizmos (e.g. collider gizmos) fade out and turn off when they are small on screen. Cameras typically used for planar reflections (ones with oblique clip projection matrix) now also do not render gizmos.</p></li>
<li><p>Editor: Changed the Position handle to follow mouse movements more precisely. (<a href="https://issuetracker.unity3d.com/issues/sceneview-move-tool-axis-move-does-not-follow-the-mouse-position">1217150</a>)</p></li>
<li><p>Editor: Disabled the <em>Maximize</em> option for <em>Preview</em> window when docked. (<a href="https://issuetracker.unity3d.com/issues/inspector-framework-nullreferenceexception-is-thrown-when-the-preview-window-is-maximized">1258262</a>)</p></li>
<li><p>Editor: Marked Unity Remote as deprecated.</p></li>
<li><p>Editor: Modified the <em>Rect Tool</em> when calculating an object's bounds so that <em>GameObjects</em> with a <code>MeshFilter</code> but no <code>MeshRenderer</code> are included.</p></li>
<li><p>Editor: Removed "macOS Color Picker" editor preference setting.</p></li>
<li><p>Editor: Removed 3D With Extras template.</p></li>
<li><p>Editor: Removed Asset Store integration from the Project Browser. (<a href="https://issuetracker.unity3d.com/issues/unityeditor-dot-asynchttpclient-done-error-when-switch-between-in-packages-and-in-assets-for-the-serach-results">1240939</a>)</p></li>
<li><p>Editor: Removed the ability to discard changes to an untitled Scene. (<a href="https://issuetracker.unity3d.com/issues/scene-management-invalidoperationexception-is-thrown-when-discarding-changes-in-deleted-scene">1111388</a>)</p></li>
<li><p>Editor: Revert reintroduction of OnDestroy/Awake calls for ExecuteAlways scripts when we enter Play Mode with the Scene Reload disabled.</p></li>
<li><p>Editor: Updated GameObject creation from a context menu or Scene so new GameObjects are instantiated at the world origin. (1179419)</p></li>
<li><p>Editor: Updated Hierarchy view to automatically enter rename mode when new objects are created. "Rename New Objects" in Hierarchy view settings menu turns this behavior off.</p></li>
<li><p>Editor: Updated interaction mode labels and tooltips.</p></li>
<li><p>Editor: Updated the com.unity.ide.rider package to version 2.0.7 as a verified package.</p></li>
<li><p>Editor: Verified the configurable Enter Play Mode feature.</p></li>
<li><p>GI: Modified the LightingSettings asset so it is now only created when saving an upgraded project.</p></li>
<li><p>GI: Unlocked the maximum number of bounces supported by the lightmapper.<br> Added min bounces and max bounces UI labels for better readability.<br></p></li>
<li><p>GI: Updated 3D template so that new projects created with it support baked light cookies by default.</p></li>
<li><p>GI: Updated Open Image Denoise to the Clang compiled binary instead of IC., This fixed a Rosetta emulation issue on a Mac.</p></li>
<li><p>Graphics: Enabled "Gfx command not handled: 0 (Last command: 10123)" in the Editor's console while in Scene view when using the wireframe mode and Vulkan rendering API. (<a href="https://issuetracker.unity3d.com/issues/graphics-gfx-command-not-handled-error-thrown-continuously-on-switching-editor-to-wireframe-mode-using-vulkan-graphics-api">1276056</a>)</p></li>
<li><p>Graphics: Exposed mesh function to set UV Distribution metric for procedurally generated meshes with mip streaming. (<a href="https://issuetracker.unity3d.com/issues/graphics-scripting-meshes-created-in-c-number-cannot-have-their-uv-distribution-metric-updated">1248390</a>)</p></li>
<li><p>Graphics: Updated the SRP packages and template to version 10.2.2 (<a href="https://issuetracker.unity3d.com/issues/hdrp-opening-template-scene-freezes-or-reboots-mac">1291998</a>)</p></li>
<li><p>iOS: Removed OpenGL ES support on iOS/tvOS.</p></li>
<li><p>iOS: Removed support for Launch Images, to adhere to new Apple guidelines.</p></li>
<li><p>Kernel: Updated native allocators to use slightly larger blocks, to avoid the more resource-intensive overflow allocations that go directly to system memory. This causes a very slight increase in initial memory usage, but avoids some spikes in performance.</p></li>
<li><p>License: Updated the output message after a return license request timeouted. (1146162)</p></li>
<li><p>macOS: MacOS 10.13 is now the minimum OS requirement for the MacEditor and MacPlayer. (1263013)</p></li>
<li><p>Mobile: Changed maximum temperative level to level 10 in Adaptive Performance Samsung Provider GameSDK 3.2.</p></li>
<li><p>Mobile: Fixed Analytics system error with unloaded subsystem in Adaptive Performance.</p></li>
<li><p>Mobile: Provider downloader will now download latest available build instead of verified if verified version is below 2.0.0. This can happen on 2019 and 2020.1 as the verified package version is 1.x.</p></li>
<li><p>Mobile: Removed unnecessary folders and files from the Adaptive Performance package.</p></li>
<li><p>Mobile: Updated Adaptive Performance Samsung Provider GameSDK 3.2. You can use the Adaptive performance CPU and GPU levels until the system reaches warning level 2 (throttling).</p></li>
<li><p>Package Manager: Added a General Preference option to allow the log level used by the Unity Package Manager for the Editor.log and upm.log files to be customized. This preference is saved and re-used across sessions, and it is overridden by the effects of the <code>-enablePackageManagerTraces</code> command-line argument.</p></li>
<li><p>Package Manager: Added the <code>UnityEditor.PackageManager.Client.LogLevel</code> property that allows you to configure the log level that the Unity Package Manager uses for the upm.log file.</p></li>
<li><p>Package Manager: Changed path and file format of global configuration file. The configuration file format is now TOML. The old global configuration file path is deprecated. New global configuration should be set in this new file.</p></li>
<li><p>Package Manager: Changed the design of the items in the Package List to be one line.</p></li>
<li><p>Package Manager: Modified Package Manager to no longer discard the existing package state in case of critical errors such as failure to parse the project manifest.</p></li>
<li><p>Package Manager: Split <code>All Packages</code> into <code>Unity Registry</code> and <code>My Registries</code>.</p></li>
<li><p>Package Manager: Updated functionality to automatically add embedded package files to the version control system.</p></li>
<li><p>Package Manager: Updated how version conflicts involving a direct project dependency are reported. They are now reported like any other version conflict instead of being silenced.</p></li>
<li><p>Package Manager: Updated the com.unity.purchasing package to version 2.1.0.</p></li>
<li><p>Package Manager: Updated the recommended version logic in the Package Item version drop down.</p></li>
<li><p>Package Manager: Upgraded Cinemachine to 2.6.0. See Cinemachine 2.6 release notes.</p></li>
<li><p>Player: Added a dependency on 'com.unity.modules.subsystems' to the Subsystem Registration package.</p></li>
<li><p>Player: Added ToString override to PlayerLoopSystem to show system type.</p></li>
<li><p>Scripting: Reintroduced a warning when a script that is derived from MonoBehaviour has the same name as a built-in component (for example,Transform).</p></li>
<li><p>Scripting: Removed Boo.dll and UnityScript.dll from Mono distribution.</p></li>
<li><p>Scripting: Roslyn Analyzers inside Assembly Definitions Folders are now only applied to the Asmdef Assembly itself and to other Assemblies referencing the Asmdef Assembly - but not to any other code in the project.</p></li>
<li><p>Scripting: Strong Name Assembly references only validate if the assemblies are in different folders.</p></li>
<li><p>Services: Added support to in the In-App Purchasing Service settings for safely migrating the <a href="https://docs.unity3d.com/2019.4/Documentation/Manual/UnityIAP.html">IAP</a> package from older versions to 3.0+. Retained the ability to update to the most recent legacy versions of In-App Purchasing without migrating. Projects without any versions of this package already installed can install 3.0+ from the In-App Purchasing Settings user interface.</p></li>
<li><p>Services: Updated com.unity.purchasing to 2.1.1.</p></li>
<li><p>Shaders: Changed Editor so that it skips warming up shaders from shader collections in the Preloaded shaders section of Graphics settings.</p></li>
<li><p>Shaders: Made Caching Shader preprocessor the default preprocessor for shaders.</p></li>
<li><p>Shaders: Relaxed macro expansion rules in Caching Preprocessor for token pasting to always use expanded arguments instead of non-expanded arguments.</p></li>
<li><p>Timeline: Modified <code>ControlPlayableAsset.searchHierarchy</code> to default to false. You now have to specifically set it to true to search the entire hierarchy.</p></li>
<li><p>Timeline: Updated the default <a href="https://docs.unity3d.com/Packages/com.unity.timeline@1.5/manual/index.html">Timeline</a> package version to 1.4.4.</p></li>
<li><p>UI: Expanded the usable UV to Vector4 instead of the previous limit of Vector2. (<a href="https://issuetracker.unity3d.com/issues/only-2-uv-components-per-channel-are-accessible-in-shader-when-mesh-is-rendered-by-canvasrenderer">1208182</a>)</p></li>
<li><p>UI: Set <code>Switch m_CullTransparentMesh</code> to true so transparent Meshs are culled by default. (1257834)</p></li>
<li><p>UI: Updated the <code>EventSystem.current</code> API so that it doesn't do unnecessary work when setting <code>current</code> to the already current system.</p></li>
<li><p>UI Toolkit: Renamed menu entries of UIElements to UI Toolkit.<br></p> 
<ul>
<li><em>Window/Analysis/UIElements Debugger</em> becomes <em>Window/UI Toolkit/Debugger</em><br></li>
<li><em>Window/UI/UIElements Samples</em> becomes <em>Window/UI Toolkit/Samples</em><br></li>
<li><em>Create/UIElements/Editor Window</em> becomes <em>Create/UI Toolkit/Editor Window</em><br></li>
<li><em>Create/UIElements/USS File</em> becomes <em>Create/UI Toolkit/Style Sheet</em><br></li>
<li><em>Create/UIElements/UXML Template</em> becomes <em>Create/UI Toolkit/UI Document</em><br>
Removed mentions of UIElements in the output of the Editor Window script generator.</li>
</ul></li>
<li><p>XR: Added interface changes for providers to share unresolved MSAA targets between eye texture swap chains. This provides some memory savings. (1254408)</p></li>
<li><p>XR: Changed how temporarily disabling runtime MSAA level is affected if running with Vulkan and XR Management.</p></li>
<li><p>XR: Keep SRP occlusion mesh data accessible from the CPU.</p></li>
<li><p>XR: Removed the ARCore client libraries from Unity. These libraries are now added to a project by installing the ARCore SDK for Unity (distributed by Google).</p></li>
<li><p>XR: Updated the Oculus XR Plugin package to 1.6.1.</p></li>
<li><p>XR: Updated verified packages for AR Foundation and related packages.</p></li>
<li><p>XR: Updated verified version of com.unity.xr.legacyinputhelpers to v2.1.6<br> Changelog for 2.1.6 of com.unity.xr.legacyinputhelpers:<br></p>

<ul>
<li>Fixes error message when using the color camera<br></li>
<li>Changes default near clip plane to 0.01f<br></li>
<li>Fixes rig migration for URP and HDRP.<br></li>
<li>Support for URP/HDRP v10.1.</li>
</ul></li>
</ul>

### API Changes
