# Unity 2022.1.0
https://unity3d.com/unity/whats-new/2022.1.0

## Final 2022.1.0f1 Release Notes


### Features
<ul>
<li><p>2D: Added an actionable console log for the PSDImporter when you encounter vertex count limit exception on Sprite Shape.</p></li>
<li><p>2D: Added an asset upgrading tool, which can upgrade older Sprite Library Assets and Animation Clips to the latest version.</p></li>
<li><p>2D: Added Sortpoint for SpriteShapeRenderer that determines the position for sorting.</p></li>
<li><p>2D: Added support for Color channel in SpriteShape so you can use Vertex Colors.</p></li>
<li><p>2D: Added support for Global Grid Snapping for editing Sprite Shapes with the PSDImporter.</p></li>
<li><p>2D: Added user preferences for the PSDImporter for Controlpoint/Tangent/Spline color.</p></li>
<li><p>2D: Enabled you to selectively indicate which layer to import from a Photoshop file with the PSDImporter.</p></li>
<li><p>2D: Exposed certain PSDImporter import settings as APIs.</p></li>
<li><p>2D: Improved estimation of vertices required for geometry to minimize memory alloction for the PSDImporter.</p></li>
<li><p>Android: Added ability to include custom asset packs into the build if you add assets to the directory that ends with '.androidpack'.</p></li>
<li><p>Android: Added Adaptive Decals for Adaptive Performance.</p></li>
<li><p>Android: Added Adaptive Layer Culling for Adaptive Performance.</p></li>
<li><p>Android: Added Adaptive Physics for Adaptive Performance.</p></li>
<li><p>Android: Added Custom Scaler for Adaptive Performance.</p></li>
<li><p>Android: Added Visual Scripting support for Adaptive Performance.</p></li>
<li><p>Android: Enabled the Unity Editor to create asset packs if you build an Android App Bundle with Split App Binary enabled.</p></li>
<li><p>Animation: Added a DiscreteEvaluation attribute that allows a property to be evaluated as a discrete value in animation playback so the values in between key frames are not interpolated nor is the value blended between clips.</p></li>
<li><p>Asset Import: Updated Preset Editors to support a CustomEditor made with UIToolkit for the Preset Object.</p></li>
<li><p>Asset Pipeline: Added options for Accelerator corruption detection.</p></li>
<li><p>Asset Pipeline: Enabled models imported from the ModelImporter using the DefaultMaterial to re-import correctly to use SRP default material when you change the active Render Pipeline.</p></li>
<li><p>Editor: Added a new "On Play Behavior" dropdown to the GameView. It contains options to maximize the game view or render it as a full screen window on a chosen monitor.</p></li>
<li><p>Editor: Added a new menu entry under <em>Help</em> to display <em>Third Party Notices</em> for the Unity Package Manager.</p></li>
<li><p>Editor: Added granular context capabilities to ShortcutManager.</p></li>
<li><p>Editor: Added support for inheritance between materials in the editor.</p></li>
<li><p>Editor: Updated the Device Simulator to allow you to switch between different screens for devices with multiple screens.</p></li>
<li><p>GI: Added a HDR Cubemap Encoding project setting to the Player tab, which controls the encoding format used for HDR cubemaps.</p></li>
<li><p>Graphics: Added a new Texture Mode called Static to the LineRenderer, TrailRenderer and ParticleSystem trails.</p></li>
<li><p>Graphics: Added a new Texture Scale option to the LineRenderer, TrailRenderer, and ParticleSystem trails.</p></li>
<li><p>Graphics: Added MSAA depth resolve Vulkan support.</p></li>
<li><p>Graphics: Added the <code>RayTracingAccelerationStructure.ClearInstances</code> method that removes all the content from a <code>RayTracingAccelerationStructure</code>.</p></li>
<li><p>Input: Enabled the Input Manager's Physical Keys by default for new projects. This enables layout independent keycodes on all platforms.</p></li>
<li><p>Input System: Added support for PS5 DualSense controllers on Mac and Windows.</p></li>
<li><p>License: Added error analytics for licensing module.</p></li>
<li><p>License: Deprecated the Legacy Licensing module.</p></li>
<li><p>Mobile: Added ability to request cluster info to have details of which and how many cores are available on the device.</p></li>
<li><p>Mobile: Added boost mode to boost CPU and GPU for short periods of time.</p></li>
<li><p>Mobile: Added predefined profiles to easily define and change Adaptive Performance Scalers.</p></li>
<li><p>Mobile: Added the adaptive view distance scaler, which changes the Camera.main view distance automatically.</p></li>
<li><p>Mobile: Added the Feature API to check which Adaptive Performance feature is available on the current platform.</p></li>
<li><p>Mobile: Enabled boost mode during engine startup.</p></li>
<li><p>Mobile: Integrated the Unity Profiler to easily profile Adaptive Performance.</p></li>
<li><p>Mono: Enabled Brotli compression for Windows with the Mono runtime.</p></li>
<li><p>Package: Added a searcher window so you can filter and prioritize search results as needed.</p></li>
<li><p>Package Manager: Added a spinner button in the menu for users to check all download &amp; install progress in the Package Manager.</p></li>
<li><p>Package Manager: Added ability to configure location of both UPM and Asset Store package local cache.</p></li>
<li><p>Package Manager: Added documentation links to feature's included packages when it's customized or manually modified.</p></li>
<li><p>Package Manager: Added multi-selection and bulk operations to the UI.</p></li>
<li><p>Package Manager: Added warning for Unity package versions that have invalid signatures, or are unsigned and sourced from local tarball or scoped registry.</p></li>
<li><p>Package Manager: Enhanced the UI to display the packages' supported platforms. Note: This requires further backend implementation.</p></li>
<li><p>Package Manager: Improved ways to check for <code>Update Available</code> in the Package Manager window.</p></li>
<li><p>Package Manager: Modified the package item so you can see the 'E' icon when the license is Granted or Not granted in a closed network.</p></li>
<li><p>Package Manager: Updated the import window to display the project settings separately from the rest of the package content, when you import a package from the Asset Store.</p></li>
<li><p>Package Manager: Updated the Package Manager so the <em>experimental packages in use</em> button does not reappear if it has been dismissed for the project.</p></li>
<li><p>Package Manager: Updated the Package Manager to display an error message if you don't have the rights to use an entitled package.</p></li>
<li><p>Physics: Added a new batched ClosestPointCommand to calculate the closest point to a convex off the main thread.</p></li>
<li><p>Physics: Added Contact and Query visualization to the Physics Debug window.</p></li>
<li><p>Physics: Added highlights for physics layers when you hover over them in the Physics settings inter-collision matrix.</p></li>
<li><p>Physics: Added the ability to generate Delaunay meshes for specific 2D Colliders. This option will generally produce simple meshes with few primitive physics shapes for enhanced overall performance. Added "PolygonCollider2D.useDelaunayMesh", "TilemapCollider2D.useDelaunayMesh" &amp; "CompositeCollider2D.useDelaunayMesh".</p></li>
<li><p>Physics: Added the option to filter by Unity scene along with physics scene in the Physics Debugger.</p></li>
<li><p>Prefabs: Differentiated between applicable and revertible overrides.</p></li>
<li><p>Profiler: Expanded the platform reach and frame timing information for the FrameTimingManager.</p></li>
<li><p>Scene/Game View: Improved the workflow for you to use ToolContexts.</p></li>
<li><p>Search: Added a query builder to expression search queries using a set of user facing blocks.</p></li>
<li><p>Services: Enhanced Cloud Diagnostics to display C# line numbers in exception stack traces when using IL2CPP.</p></li>
<li><p>Shaders: Added an option to use strict shader variant matching in the player.</p></li>
<li><p>Shaders: Added <code>#pragma dynamic_branch</code> and <code>#pragma dynamic_branch_local</code> directives to declare dynamic branching keywords in shaders.</p></li>
<li><p>Shaders: Removed the ability to opt out from using the Caching preprocessor.</p></li>
<li><p>Shaders: Updated the ray tracing shaders to use the Caching preprocessor.</p></li>
<li><p>Timeline: Added an API to control Timeline Editor Window playback through script.</p></li>
<li><p>UI Toolkit: Added new vector drawing API to VisualElements.</p></li>
<li><p>UI Toolkit: Added UI Toolkit implementation for property drawers.</p></li>
<li><p>UI Toolkit: Added UI Toolkit implementation for UnityEvent drawer and LazyLoadReference drawer.</p></li>
<li><p>UI Toolkit: Added UI Toolkit implementation of MinMaxGradient drawer.</p></li>
<li><p>UI Toolkit: Updated fields to be usable in Runtime:<br> <br></p>

<ul>
<li>BoundsField<br></li>
<li>BoundsIntField<br></li>
<li>DoubleField<br></li>
<li>FloatField<br></li>
<li>Hash128Field<br></li>
<li>IntegerField<br></li>
<li>LongField<br></li>
<li>RectField<br></li>
<li>RectIntField<br></li>
<li>Vector2Field<br></li>
<li>Vector3Field<br></li>
<li>Vector4Field<br></li>
<li>Vector2IntField<br></li>
<li>Vector3IntField</li>
</ul></li>
<li><p>UI Toolkit: Updated InputField to be driven by TextCore.<br> Updated TextCore text assets (FontAsset, Text Settings...) to work in InputFields.<br>
Added an inner ScrollView to InputFields.<br>
Updated TextElements including Labels to be selectable.</p></li>
<li><p>Undo System: Enhanced the UI so you can explore undo history.</p></li>
<li><p>Version Control: * Plastic: Added support to invite other members. This option is available from the gear icon.<br></p> 
<ul>
<li>Plastic: Added support to sign in with Cloud Edition. This is available during the onboarding screen if you've never signed in.<br></li>
<li>Plastic: Added support to turn off Plastic in your project. This option removes the Plastic metadata from your directory. This option is available under <em>Assets</em> &gt; <em>Plastic SCM</em> &gt; <em>Turn off Plastic SCM</em>.<br></li>
<li>Plastic: Added a notification on the Plastic SCM tab title to indicate incoming changes. You no longer need to have the Plastic SCM window visible to know there are incoming changes.<br></li>
<li>Plastic: Added auto configuration of SSO.<br></li>
<li>Plastic: Added a date column in incoming changes.</li>
</ul></li>
<li><p>Version Control: Added "Switch to changeset" menu option in changesets view<br> Added "Go back to changeset" menu option in changesets view.</p></li>
<li><p>Version Control: Added auto sign in when you are logged into your Unity account.</p></li>
<li><p>Version Control: Added branch name column in changeset view.</p></li>
<li><p>Version Control: Added checkout option in scene prefab view.</p></li>
<li><p>Version Control: Added empty state and success state message for Pending Changes tab.</p></li>
<li><p>Version Control: Added horizontal scroll bar to better view Changesets list.<br> Added auto-login for the SSO credentials handler.<br>
Added metrics for changeset tab usage.<br>
Added metrics for checkin actions.<br>
Added a new Undo icon.<br>
Added more API documentation.<br>
Added the ability to modify assets without checkout.<br>
Added the ability to allow empty checkin messages.<br>
Added empty checking message localization.<br>
Added a Plastic toolbar button to Unity editor.<br>
Added a notification icon for incoming changes to Plastic toolbar button.</p></li>
<li><p>Version Control: Added metrics for Branches tab functionalities.</p></li>
<li><p>Version Control: Added option to "Add to ignore file" in context menu in the project view.</p></li>
<li><p>Version Control: Added option to "Save Revision as" to the context menu in the changesets view<br> Added incoming changes overview bar for Gluon workspace.</p></li>
<li><p>Version Control: Added visual overview bar to the incoming changes tab.<br> Added progress dialog for the migration process.<br>
Added a Branches tab that shows a list of all branches in the repository.<br>
Added the option and dialog to create a child branch from selected branch.<br>
Added the option to switch to another branch.<br>
Added the option and dialog to rename a branch.<br>
Added the option to delete a branch.<br>
Added a preference to save if the window is open in the Branches tab by default.<br>
Added metrics for Plastic SCM installation window usage.</p></li>
<li><p>Version Control: Enabled workspace migration from Collab to Plastic, whether or not you have Plastic installed.<br> Added notification status icons.<br>
Added light and dark mode versions of avatar icon.</p></li>
<li><p>VFX Graph: Added criteria to sort the particles of an output context:<br> <br></p>

<ul>
<li>By Distance<br></li>
<li>Youngest in front<br></li>
<li>Oldest in front<br></li>
<li>By Depth<br></li>
<li>Custom</li>
</ul></li>
<li><p>Video: Added support for Mac for advanced video encoding controls for H.264.</p></li>
<li><p>Visual Scripting: Made the High Performance Interpreter public in version 1.8.0-pre.1. You can download this using the package manager if you enable experimental packages.</p></li>
<li><p>WebGL: Added a WebGL template for Progressive Web Apps.</p></li>
<li><p>WebGL: Added mobile keyboard support for WebGL to enter text in UI input fields.</p></li>
<li><p>WebGL: Added texture compression format setting to WebGL's player settings.</p></li>
<li><p>WebGL: Added UI options for control WASM memory heap size and growth.</p></li>
<li><p>WebGL: Improved caching of data files and asset bundles.</p></li>
<li><p>WebGL: Removed mobile browser warning from builds.</p></li>
</ul>

### Improvements
<ul>
<li><p>2D: Added Preset Support to SpriteAtlas V2.</p></li>
<li><p>2D: Added support for Build Only SpritePacking in SpriteAtlas V2.</p></li>
<li><p>2D: Cache internal reflection to speed up Sprite editing data access.</p></li>
<li><p>2D: Improved Console log to display all affected Sprites.</p></li>
<li><p>2D: Improved performance of RuleTile caching.</p></li>
<li><p>2D: Sprite Dynamic Batching Vertex Limit is now configurable through PlayerSettings.</p></li>
<li><p>2D: Sprite Frame module's pivot unit mode now persists after entering and exiting playmode.</p></li>
<li><p>2D: Sprite outline shape calculation is faster now (Sprite.Create, or importing sprite textures), especially for large textures.</p></li>
<li><p>2D: SpriteAtlas Cache max Size should be Project Settings instead of Preferences.</p></li>
<li><p>2D: Updated 2D URP template starting folder structure for better clarification of usage.</p></li>
<li><p>2D: Updated Skinning Editor tooltips text.</p></li>
<li><p>Android: Added boot-config/command-line switch "platform-android-cpucapacity-threshold" that can be used to specify which CPU cores are treated as big cores. The cpu capacity is a value in the range between 0 and 1024. A capacity value of 870 yields the same behavior as before the fix for case 1349057.</p></li>
<li><p>Android: Added support for HDR display output.</p></li>
<li><p>Android: Builds will fail early and with a human readable error message, when Unity project is located in path with Non ASCII characters. Android Tools like clang don't work correctly when operating in paths with non ascii characters and the error is not very clear, thus Unity will provide a better error message. (1340631)</p></li>
<li><p>Android: Bump Android Logcat package to 1.2.3.</p></li>
<li><p>Android: Editor log will contain more information about the location from where OnPostGenerateGradleAndroidProject are called.</p></li>
<li><p>Android: Improved VideoPlayer performance on Android when using Vulkan on devices that support VK_ANDROID_external_memory_android_hardware_buffer.</p></li>
<li><p>Android: Improved WebCamTexture when using Vulkan on Android devices that support VK_ANDROID_external_memory_android_hardware_buffer.</p></li>
<li><p>Android: Input System will now send text events for combinations Ctrl + [A..Z].</p></li>
<li><p>Android: Native Input Backend will send less Move Events to the input system package. It will ignore Move Events which position didn't change from previous event. This should improve performance when touching screen with multiple fingers.</p></li>
<li><p>Android: OBB loading performance improved and removed excessive asks for external storage read permission.</p></li>
<li><p>Asset Import: Improved performance of asset import particularly when importing large numbers of small files such as scripts.</p></li>
<li><p>Asset Pipeline: Clarified the behaviour of Resources.Load() in the Scripting API documentation.</p></li>
<li><p>Asset Pipeline: Do not assert on race when receiving import worker results for a deleted asset.</p></li>
<li><p>Asset Pipeline: Improved upload and download path.</p></li>
<li><p>Asset Pipeline: New diagnostic setting to enable writing of asset database events to Logs/AssetDatabase.log. This log file can assist when troubleshooting asset importing.</p></li>
<li><p>Asset Pipeline: Reduced import overhead for small files by 65%.</p></li>
<li><p>Asset Pipeline: Various performance optimisations for projects with large numbers of assets.</p></li>
<li><p>Audio: DSPGraph: Changed mixer thread scripting runtime attachment assertion to a warning, to better reflect the intent of the message.</p></li>
<li><p>Audio: Import now supports multiprocess.</p></li>
<li><p>Build Pipeline: Made copying of assemblies part of the incremental player to save time on subsequent builds.</p></li>
<li><p>Build Pipeline: Make error messages about microphone or camera usage more visible.</p></li>
<li><p>Build Pipeline: On platforms using incremental player builds, data builds will now be skipped if data has not changed, even for non-development builds.</p></li>
<li><p>Build Pipeline: Reference documentation improvements in area of Build Pipeline.</p></li>
<li><p>Build System: Bee_backend/win32: buffer child ouput without temp files.</p></li>
<li><p>Build System: Use a linux clang compiler optimized for speed instead of size.</p></li>
<li><p>Build System: Use a linux clang toolchain built with a newer bootstrap compiler.</p></li>
<li><p>Burst: Ability to partially select and copy text in the burst inspector.</p></li>
<li><p>Burst: Branch flow arrows in inspector are now clickable, directing to the other end of the arrow.</p></li>
<li><p>Burst: Branch flow arrows in inspector now enlarge when hovered.</p></li>
<li><p>Burst: Improved Inspector UI.</p></li>
<li><p>Burst: Right clicking the inspector view reveals a context menu, allowing selecting all text and copying selection.</p></li>
<li><p>Core: Job Debugger performance was improved.</p></li>
<li><p>Documentation: Added proper example for PhysicsScene.Simulate.</p></li>
<li><p>Documentation: Improved Scripting API docs page for RayTracingAccelerationStructure. Added See Also section.</p></li>
<li><p>Documentation: Physics: Elaborate on how ForceMode affects the velocity and angular velocity in AddForce/AddTorque.</p></li>
<li><p>Editor: (Dynamic Hints) If the target window of a Dynamic Hint is available but unfocused, it becomes focused before the Dynamic Hint is shown.</p></li>
<li><p>Editor: Added a character limit to the scene template title and dependency search field to avoid over limit errors. (<a href="https://issuetracker.unity3d.com/issues/warnings-in-the-console-window-when-a-scene-template-asset-has-a-long-title-or-description">1363618</a>)</p></li>
<li><p>Editor: Added a new badge system for scene templates that allows for a visual categorization.</p></li>
<li><p>Editor: Added an option to improve enter playmode speed by skipping unnecessary scene backups.</p></li>
<li><p>Editor: Added Async compilation of Selection Shader Passes.</p></li>
<li><p>Editor: Added GameObject pings in the Hierarchy window to more errors, when clicking on console messages.</p></li>
<li><p>Editor: Added support for Editor asynchronous load and upload of textures set up for mipmapped streaming.</p></li>
<li><p>Editor: EditorStyles.iconButton is now public so custom editor windows can implement help, settings and other icon buttons.</p></li>
<li><p>Editor: Enable packages to define their Service Group in the Services tab of packman without needing to update the Editor.</p></li>
<li><p>Editor: Greatly reduced time taken up by static batching when entering playmode or making a build.</p></li>
<li><p>Editor: Improved Dynamic Batching feedback in the Frame Debugger for the "Objects are rendered using different rendering functions." message.</p></li>
<li><p>Editor: Improved Editor responsiveness when a large number of textures are selected in the Project Browser.</p></li>
<li><p>Editor: Improved mac editor process guard in order to catch all types of exceptions and early handle cases where the ADB process might have already shut down.</p></li>
<li><p>Editor: Improved package retrieval process when loading editor window.</p></li>
<li><p>Editor: Improved performance of AssetDatabase.GetAllLabels.</p></li>
<li><p>Editor: Improved performance of picking large objects in Scene View.</p></li>
<li><p>Editor: Improved performance of Scene View with many LODGroups selected.</p></li>
<li><p>Editor: Improved performance of scrolling the scene hierarchy with large numbers of game objects when some objects are hidden or unpickable.</p></li>
<li><p>Editor: Improved performance when creating a new asset (especially in a large project).</p></li>
<li><p>Editor: Improved scene saving performance. (<a href="https://issuetracker.unity3d.com/issues/the-time-required-to-load-gameobjects-or-prefab-instances-does-not-scale-linearly">1185953</a>)</p></li>
<li><p>Editor: Improved the scene template instantiation experience.</p></li>
<li><p>Editor: MacOS editor launch screen now has an integrated progress display (Windows &amp; Linux coming later).</p></li>
<li><p>Editor: MacOS now has an Editor launch screen too.</p></li>
<li><p>Editor: Make rotation angles editable individually when multiple GameObjects are selected. (<a href="https://issuetracker.unity3d.com/issues/all-selected-gameobjects-rotation-values-are-copied-to-the-first-gameobjects-in-hierarchy-when-changing-only-one-axis-value">1298482</a>)</p></li>
<li><p>Editor: Normal Map textures now have a new "Flip Green Channel" import setting (useful for textures that were baked in 3dsmax/Unreal/Source/CryEngine convention). All textures got a Swizzle advanced import setting, for arbitrary color channel remapping/flipping.</p></li>
<li><p>Editor: Now Console window shows a clear message if no search result found.</p></li>
<li><p>Editor: Now shaders will have SHADER_API_(DESKTOP|MOBILE) define set according to the target build platform.</p></li>
<li><p>Editor: Opening a project without a "last opened scene" will open a scene template (if any) instead of the default scene.</p></li>
<li><p>Editor: Optimized AddComponent menu for projects with large amount of scripts.</p></li>
<li><p>Editor: Optimized calculating the size of Undo operations, making many changes to GameObjects should now be cheaper to add to the Undo system.</p></li>
<li><p>Editor: Optimized GameObjectInspector.CalculatePrefabStatus which could result up to a 3X speedup for complex prefabs.</p></li>
<li><p>Editor: Optimized Inspector.InitOrRebuild - shaves several seconds when working with large selections in large scene.</p></li>
<li><p>Editor: Optimized prefab editing, will knock about 20% off the cost of changing a large prefab.</p></li>
<li><p>Editor: Optimized SavePrefab_Internal, cutting time in this code for a large prefab from 20 seconds to 20 milliseconds.</p></li>
<li><p>Editor: Optimized StripPrefabObjectsWhichAreNotUsed, representing up to a 28% speedup for large scenes.</p></li>
<li><p>Editor: Project opening can now be cancelled while loading.</p></li>
<li><p>Editor: Reduced overhead of property editor when changing objects in the editor with an inspector window open.</p></li>
<li><p>Editor: Reduced time to enter playmode.</p></li>
<li><p>Editor: Refactored the Background task window for better performance and support multiple nested levels of progress.</p></li>
<li><p>Editor: Revamped the type dropdown in the scene template project settings.</p></li>
<li><p>Editor: The IMGUI TreeView control now has support for rendering hover effect on row items as well as rendering row contents greyed out based on the GUI.enabled flag.</p></li>
<li><p>Editor: UnityEvent callbacks can be reordered.</p></li>
<li><p>Editor: Updated the Unity logo in anticipation of the brand identity refresh scheduled for October 5th.</p></li>
<li><p>Editor: When a prefab is larger than 8MB, show a static preview image to save the time of loading animations etc.</p></li>
<li><p>EmbeddedLinux: A port field is now exposed for the managed debugger in Build settings when Debugging script is checked.</p></li>
<li><p>GI: Bake performance section shows "Infinity mrays/sec" when baking the first lightmap on macOS.</p></li>
<li><p>GI: Expose number of Enlighten worker threads to the command line. Example: Use <code>enlighten-job-worker-count 16</code> to force 16 threads for Enlighten.</p></li>
<li><p>GI: Maximum environment sample is 2048, as no quality improvements could be seen beyond that threshold.</p></li>
<li><p>GI: Moved indirect resolution to realtime GI area.</p></li>
<li><p>GI: Multiple Importance Sampling naming was misleading.</p></li>
<li><p>GI: Performance improvement when mesh renderers do not have their light probe property set to 'none' and there are no light probes in the scene. (<a href="https://issuetracker.unity3d.com/issues/cullperobjectlights-have-ms-increase-every-frame-when-light-probe-property-is-set-to-blend-probes">1310218</a>)</p></li>
<li><p>GI: Sample counts for the lightmapper are now rounded to the closest power of two in the UI.</p></li>
<li><p>GI: Showing a warning in the Mesh renderer inspector when the Contribute GI option is selected and a mesh is invalid.</p></li>
<li><p>GI: The Radeon denoiser will now use fp16 during progressive updates to conserve memory when supported hardware is available (AMD Radeon Vega and later GPUs).</p></li>
<li><p>GI: UI change consolidating min bounces and max bounces into single row.</p></li>
<li><p>Graphics: - MaterialEditor - Remove context menu for "Double Sided Global Illumination".<br></p> 
<ul>
<li>MaterialEditor - Make colour picker consistent with core editor.<br></li>
<li>MaterialEditor - Remove context menu for "Enable GPU Instancing".
(<a href="https://issuetracker.unity3d.com/issues/quality-audit-material-editor">1340650</a>)</li>
</ul></li>
<li><p>Graphics: Added a warning when a texture has no mip maps and exceeds device texture size limits to inform a default texture will be used instead.</p></li>
<li><p>Graphics: Added an error when DrawTexture() is used with Virtual Texturing.</p></li>
<li><p>Graphics: Added an usage example of RayTracingAccelerationStructure.CullInstances function in Scripting API docs.</p></li>
<li><p>Graphics: Bind last frame's vertex buffer of Skinned Mesh Renderers to ray tracing shaders in order to support motion vector calculation.</p></li>
<li><p>Graphics: Changed the Gear Icon for a Burger Menu for the Asset Settings Providers.</p></li>
<li><p>Graphics: Changing the version of a TexturePostProcessor script now only reimports the affected texture shapes.</p></li>
<li><p>Graphics: Clarified the warning message shown when setting msaa texture as a camera target texture.</p></li>
<li><p>Graphics: Exposed SystemInfo.supportsIndirectArgumentsBuffer to check if the indirect arguments buffer is supported.</p></li>
<li><p>Graphics: Improved CPU performance of the main thread when using ray tracing effects.</p></li>
<li><p>Graphics: Improved CPU performance of the main thread when using ray tracing effects. Simple effects (AO, Shadows, Path Tracing) that don't use too many builtin shader properties (e.g. unity_SHAr, unity_Lightmap, etc.) will be 15-30% faster.</p></li>
<li><p>Graphics: Improved CPU performance on the render thread when setting up resources for ray tracing hit groups.</p></li>
<li><p>Graphics: Improved DX12 constant binding performance.</p></li>
<li><p>Graphics: Improved error messages in the Console Window when building a RayTracingAccelerationStructure and using invalid Mesh data.</p></li>
<li><p>Graphics: LightProbe Group UX improvements<br></p> 
<ul>
<li>Change the size of the edit button.<br></li>
<li>Show Wireframe is never disabled.<br></li>
<li>Remove ringing is never disabled.</li>
</ul></li>
<li><p>Graphics: LineRenderer and TrailRenderer gain support for Sprite Masks.</p></li>
<li><p>Graphics: Optimized GfxDeviceD3D12.SetRayTracingInstanceShaders performance on the render thread (almost 2x faster).</p></li>
<li><p>Graphics: QualitySettings.maxQueuedFrames now works in Vulkan API.</p></li>
<li><p>Graphics: Reduced main thread hitching caused by Shader loading.</p></li>
<li><p>Graphics: Refactor VFX graph update to run VisualEffect updates in different threads.</p></li>
<li><p>Graphics: Set name of Vulkan VkRenderPass objects when using external debugging tool.</p></li>
<li><p>Graphics: Support linear color space in LineRenderer, TrailRenderer and ParticleSystem trails. (<a href="https://issuetracker.unity3d.com/issues/line-renderer-color-is-incorrect-when-using-linear-color-space">1339154</a>)</p></li>
<li><p>Graphics: The previously existing S8_UInt format can now be used as a RenderTexture DepthStencil format.</p></li>
<li><p>Graphics: Translate HLSL printf to debugPrintfEXT that is implemented in Vulkan validation layers and RenderDoc.</p></li>
<li><p>Graphics: Updated and add missing tooltips for light and reflection probes.</p></li>
<li><p>Graphics: Upgraded astc encoder to latest bugfix release of version 2.5.</p></li>
<li><p>Graphics: When using an AMD GPU, D24_UNorm_S8_UInt was reported as supported on some APIs which is incorrect, this has been resolved. Internally, the driver fell back to D32_S8 anyhow so the behavior does not change, but the user will have more clarity now.</p></li>
<li><p>HDRP: Fixed anchor position offset property for the Light Anchor component. (1362809)</p></li>
<li><p>HDRP: Fixed the FreeCamera and SimpleCameraController mouse rotation unusable at low framerate.</p></li>
<li><p>HDRP: Minor UX improvements on Quality Settings Panel.</p></li>
<li><p>IL2CPP: Added full support for System.Reflection.MemberInfo.GetCustomAttributesData.</p></li>
<li><p>IL2CPP: Added support for calling generic instances that were not found at conversion time.</p></li>
<li><p>IL2CPP: Added support for Il2CppSetOption attribute on structs and assemblies.</p></li>
<li><p>IL2CPP: Enabled sparse_hash_map and sparse_hash_set for Android and iOS for lower runtime memory usage.</p></li>
<li><p>IL2CPP: Fire the AppDomain.ProcessExit event when the runtime shuts down.</p></li>
<li><p>IL2CPP: Fixed issue that could cause finally blocks to run more than once.</p></li>
<li><p>IL2CPP: Fixed possible deadlock on player shutdown.</p></li>
<li><p>IL2CPP: Improved Span Indexer performance. Added an intrinsic for Span get_Item/indexer to improve performance when accessing a large number of Span items.</p></li>
<li><p>IL2CPP: Improved the performance of invoking delegates.</p></li>
<li><p>IL2CPP: Improved the run time performance of managed code when script debugging is enabled by lowering the cost of each sequence point check.</p></li>
<li><p>IL2CPP: Optimized out boxing on null checks on nullable types in generic code.</p></li>
<li><p>IL2CPP: Reduced executable size by reducing generic metadata output.</p></li>
<li><p>IL2CPP: Use intrinsics for System.Runtime.CompilerServices.Unsafe methods.</p></li>
<li><p>Input System: Touch input is handled from USB secondary capacitive touch screens on Android.</p></li>
<li><p>License: License type remove from editor title and about window.</p></li>
<li><p>License: Show proper license error dialog when editor is opened with a build license.</p></li>
<li><p>Linux: Default texture compression for EmbeddedLinux is now configurable from the player settings.</p></li>
<li><p>macOS: Minimum supported macOS version can now be set.</p></li>
<li><p>Mono: Removed extra uneeded library from editor build.</p></li>
<li><p>Networking: Optimized player loop callback on server builds.</p></li>
<li><p>Networking: Player loop callback was optimized for server builds.</p></li>
<li><p>Package: - Support of Editor Play mode (Uses IAP products defined locally; UDP methods are stubbed: Purchase and Consume will always be successful; Editor console outputs)<br></p> 
<ul>
<li>New Purchase() callback status: onPurchasePending<br></li>
<li>Scripting API documentation update<br></li>
<li>Inclusion of an Implementation Guide that uses the In-Editor Tutorial framework (in Unity Editor 2019.4 and above)<br></li>
<li>Information architecture changes to comply with the centralization of Services in the Package Manager<br></li>
<li>Misc bugfixes and optimization.</li>
</ul></li>
<li><p>Package Manager: Added hover background color to menu toolbar spinner that monitor package download progress.</p></li>
<li><p>Package Manager: Added Package Name as a selectable label to Package Details in Package Manager Window.</p></li>
<li><p>Package Manager: Improved the wording on the warning message when a user is using a different version of a package than the recommended version.</p></li>
<li><p>Package Manager: Include Sign In hint in startup error dialog when Package Manager resolution fails due to missing authentication information.</p></li>
<li><p>Package Manager: Log package entitlement check failures in Unity editor console.</p></li>
<li><p>Package Manager: Package manager toolbar is now always kept active during refresh operations.</p></li>
<li><p>Package Manager: Small tweaks to Package Manager scripting reference documentation.</p></li>
<li><p>Package Manager: Terrain Tools package is now included in the Worldbuilding 3D feature set.</p></li>
<li><p>Particles: Added a ping back to Hierarchy view Game Object, when selecting relevant Particle System profile markers.</p></li>
<li><p>Particles: Moved Particle System Prewarming to worker threads.</p></li>
<li><p>Particles: Particle Systems can now choose whether the Gravity Modifier applies 2D or 3D Physics System gravity.</p></li>
<li><p>Physics: Changed "Collider2D.GetShapeHash()" so that it calculates the hash incrementally rather than when entirely when it is called. This results in the time take being constant rather than scaling as the number of physics shapes increases.</p></li>
<li><p>Physics: Improved the Physics Visualiser layout and moved the Rigidbody and Articulation Body Info panels to the Physics Visualiser.</p></li>
<li><p>Physics: Joint Inspector will display only 1 of connected body, depending on which one is set.</p></li>
<li><p>Physics: Optimise Rigidbody interpolation so that it doesn't require excess syncing of transforms internally, it is about 20% faster base line, but can be much faster if there were transform changes made from scripts.</p></li>
<li><p>Physics: Updated ArticulationBody.AddForce and other related method Scripting API documentation with information about current PhysX limitations.</p></li>
<li><p>Physics: Updated RaycastCommand's Scripting API to mention that it won't return more than one hit.</p></li>
<li><p>Physics: Updated the Collider.ClosestPoint Scripting API to mention that the input position will be returned if the Collider is disabled.</p></li>
<li><p>Physics: Updated to PhysX 4.1.2, a minor bugfix release. Release notes are available here: https://github.com/NVIDIAGameWorks/PhysX/blob/4.1/physx/release_notes.html.</p></li>
<li><p>Profiler: Added icons for File Access and Asset Loading Profiler Modules.</p></li>
<li><p>Scene/Game View: Added shortcut keys to cycle between available tool contexts.</p></li>
<li><p>Scene/Game View: ESC key is exiting from the current custom tool and go back to the latest persistent tool.</p></li>
<li><p>Scene/Game View: Greatly reduced overhead of OnSceneGUI callback when multi-editing many objects.</p></li>
<li><p>Scene/Game View: Improved Gizmo rebuild performance.</p></li>
<li><p>Scene/Game View: Improved outline rendering performance in the editor.</p></li>
<li><p>Scene/Game View: Improved performance for Handles.DrawWireCube.</p></li>
<li><p>Scene/Game View: Improved performance of selecting many objects.</p></li>
<li><p>Scene/Game View: Made Picking more responsive by enabling Async Shader Compilation of Picking Shaders.</p></li>
<li><p>Scene/Game View: Reduced Gizmo rendering overhead in large scenes with many Gizmos.</p></li>
<li><p>Scene/Game View: <code>EditorToolContext</code> settings are now displayed in the <em>Tool Settings</em> Overlay.</p></li>
<li><p>Scripting: Added EditorApplication.projectWindowItemInstanceOnGUI that is similar to projectWindowItemOnGUI but can also be used to customize sub-assets. (<a href="https://issuetracker.unity3d.com/issues/editorapplication-dot-projectwindowitemongui-should-also-return-the-targeted-sub-asset">1182858</a>)</p></li>
<li><p>Scripting: Added GameObject link to Warning message: "SendMessage cannot be called during Awake, CheckConsistency, or OnValidate.".</p></li>
<li><p>Scripting: Allow user code to build against .NET Standard 2.1 and .NET Framework 4.8.</p></li>
<li><p>Scripting: Display dialog that informs user that it is now safe to attach a managed debugger now displays the port that the debugger is waiting for a connection on.</p></li>
<li><p>Scripting: Improved AssemblyUpdater to not try to connect to VCS unless there assemblies under VCS that needs updating.</p></li>
<li><p>Scripting: Improved invalid ApiUpdater configs detection.</p></li>
<li><p>Scripting: Include Roslyn Analyzer diagnostics for "EnableDomainReloadTimings" diagnostic switch.</p></li>
<li><p>Scripting: Introduced a cache to speed up look up of ApiUpdater configurations.</p></li>
<li><p>Scripting: Make JsonUtility.FromJson[Overwrite] faster on inputs with long string-valued fields.</p></li>
<li><p>Scripting: Optimized searching for scripts when the assembly name is not supplied which can significantly improve performance entering PlayMode amongst other areas.</p></li>
<li><p>Scripting: Rename ".NET Standard" to ".NET Standard 2.1" in the Api Compatibility Level options to be more precise.</p></li>
<li><p>Scripting: Switched CSharpCompiler utility to use roslyn instead of legacy mcs compilation.</p></li>
<li><p>Scripting: The Managed Stripping Level for new projects when targeting the IL2CPP backend will be Minimal.</p></li>
<li><p>Scripting: Unity engine and editor managed code is now compiled with .net standard 2.1.</p></li>
<li><p>Search: Improved query builder UX and UI.</p></li>
<li><p>Search: Many UI and UX search improvements.</p></li>
<li><p>Serialization: Added more examples to the reference for dealing with Arrays with SerializedProperty.</p></li>
<li><p>Serialization: Added more reference documentation and examples for SerializedObject and SerializedProperty.</p></li>
<li><p>Serialization: Avoid unnecessary serialization when calling SerializedObject.ApplyModifiedProperties in the single target case.</p></li>
<li><p>Serialization: Improved performance of StreamedBinaryWrite in specific scenarios.</p></li>
<li><p>Serialization: Improved SerializedFileWrite to minimize file rewrite, this comes with many performance improvements.</p></li>
<li><p>Serialization: Improved the use of SerializationCache.</p></li>
<li><p>Serialization: SerializedProperty.boxedValue property supports reading and writing entire Structs.</p></li>
<li><p>Shaders: Optimized parsing of #line directives, making import of large shaders with many #line / #include directives faster.</p></li>
<li><p>Shaders: Some GLSL reserved words are now usable in shaders. (937467)</p></li>
<li><p>UI Elements: Improved performance of mesh processing in the renderer.</p></li>
<li><p>UI Toolkit: Clarified the message displayed to the user when deleting a style sheet that is being used in the UI Builder. (1354492)</p></li>
<li><p>UI Toolkit: Fixed list view preview size in UI Builder. (1349018)</p></li>
<li><p>UI Toolkit: Fixed selectors quick sheet styling in UI Builder. (1352270)</p></li>
<li><p>UI Toolkit: Improved in-place editing of a Label to match the underlying style (UI Builder). (1354493)</p></li>
<li><p>UI Toolkit: Removed unnecessary calls to HandleEvent when no associated callbacks are present for the corresponding event.</p></li>
<li><p>UI Toolkit: TransitionEvents are now collapsed when relevant.</p></li>
<li><p>UI Toolkit: TransitionEvents reentrance is properly handled.</p></li>
<li><p>Version Control: - Stability and performance improvements.</p></li>
<li><p>Version Control: Added Checkin and Update confirmation notification.</p></li>
<li><p>Version Control: Added support for TLSv1.2 connections to Perforce servers. The Plugin is now using Perforce API v17.2. (1404016)</p></li>
<li><p>Version Control: Improved load time performance.</p></li>
<li><p>VFX Graph: Improved the following issues with the Bounds recording in the VFX Graph<br></p> 
<ul>
<li>System bounds are now always computed in local space, in order to avoid lossy transformations of AABB between spaces.<br></li>
<li>Effects containing Automatic systems are now forced to refresh every frame, so that the automatic systems can update their bounds even when off-screen.<br></li>
<li>The last known padding can now be accessed from C# through an internal binding.</li>
</ul></li>
<li><p>Virtual Texturing: Tile requests are now returned via <code>PopRequests</code> more frequently.</p></li>
<li><p>Virtual Texturing: <code>InvalidateRegion</code> calls now generate new tile requests in their "importance" order. The importance is defined as a combination of the tile's screen space size and the the number of frames since the tile has been requested. This makes completing tile requests contribute more to the rendering result when <code>InvalidateRegion</code> is called continuously.</p></li>
<li><p>Visual Scripting: Eliminating domain reload cost for users when not using Visual Scripting.</p></li>
<li><p>WebGL: Enabled Play Mode tests for WebGL platform.</p></li>
<li><p>Windows: Alt + Enter now defaults to native resolution rather than the resolution that the window was in windowed mode. This makes the image more crisp and reduces the chance of letterboxing.</p></li>
<li><p>XR: Added profiler markers for some XR Display subsystem entry points. Markers are named XR.Display.*.</p></li>
<li><p>XR: Added SRP batcher support for late latching.</p></li>
<li><p>XR: Return proper boolean values for TryGetBoundaryPoints.</p></li>
<li><p>XR: Updated Oculus Android manifest with intent-filter.</p></li>
</ul>

### API Changes
<ul>
<li><p>2D: Added: Added Tilemap.GetTilesBlockNonAlloc API.</p></li>
<li><p>2D: Added: SortingGroup.ignoreParentSortingGroup to allow a Sorting Group to ignore all parents and sort on a global level instead of being a child of the parent Sorting Group.</p></li>
<li><p>2D: Added: Tilemap.tilemapPositionsChanged.</p></li>
<li><p>2D: Changed: Made Tilemap.tilemapTileChanged available in Runtime.</p></li>
<li><p>Android: Added: New APIs to manage fast-follow and on-demand delivered asset packs. The APIs wrap Google's PlayCore functionality.</p></li>
<li><p>Android: Changed: UnityPlayer Java class now explicitly requires Activity instead of Context in constructors.</p></li>
<li><p>Animation: Deprecated: Deprecated the Play function in the AnimationPlayableUtilities API to prevent potential issues when passing Timeline Playables into the function. (<a href="https://issuetracker.unity3d.com/issues/timeline-audio-track-in-playable-graph-is-not-played-when-the-animator-update-mode-is-set-to-animate-physics">1279412</a>)</p></li>
<li><p>Apple TV: Added: Identifier for 2nd generation Apple TV 4K.</p></li>
<li><p>Apple TV: Changed: Identifiers for Apple TV HD and first generation Apple TV 4K.</p></li>
<li><p>Asset Import: Added: ModelImporter setting to enable FBX relaxed checks. (1360524)</p></li>
<li><p>Asset Import: Changed: Updated the Import Overrides API &amp; adds support for composite extensions.</p></li>
<li><p>Asset Pipeline: Added: It is now possible to control the execution order of AssetPostprocessor.OnPostprocessAllAssets by defining the dependencies using the attributes RunAfterClassAttribute, RunBeforeClassAttribute, RunAfterAssemblyAttribute, RunBeforeAssemblyAttribute, RunAfterPackageAttribute and RunBeforePackageAttribute.</p></li>
<li><p>Build Pipeline: Deprecated: BuildReport.files has been deprecated. Use BuildReport.GetFiles() instead.</p></li>
<li><p>Build Pipeline: Deprecated: UnityLinkerBuildPipelineData.inputDirectory is obsolete, as we no longer take input assemblies for builds all from a single directory.</p></li>
<li><p>Burst: Added: Added support for DOTS Runtime running / loading .Net Core assemblies.</p></li>
<li><p>Burst: Added: Added support for <code>System.Span</code> and <code>System.ReadOnlySpan</code> within Bursted code. These types are not allowed as entry-point arguments.</p></li>
<li><p>Burst: Added: BurstAuthorizedExternalMethodAttribute is now used to mark external functions that are safe to call potentially multiple times from static constructors (pure functions, with no side effects).</p></li>
<li><p>Editor: Added: A method to be able to draw the cookie widget providing your own Property, GUIContent and LightType.</p></li>
<li><p>Editor: Added: Added pen support in the macOS and Windows Editor for old and new input systems. Adds access to pen position, twist, tilt, pressure, and pen status (e.g. button state). On Windows, adds an addition API for coalesced pen events. The missing events can be retrieved with Input.GetPenEvent(). The count of accumulated pen events is retrieved with Input.penEventCount, and the queue of coalesced events cleared with Input.ResetPenEvents().</p></li>
<li><p>Editor: Removed: Made Il2CppEagerStaticClassConstructionAttribute internal to avoid conflicts with other definitions outside of the package.</p></li>
<li><p>GI: Added: Eliminate breaking change in LightingExplorerTab constructor by reintroducing the previous constructor. (1348261)</p></li>
<li><p>GI: Added: LightingSettings.lightmapCompression has been added and determines the quality of compression used for lightmaps.</p></li>
<li><p>GI: Deprecated: Deprecate the unused UNITY_USE_NATIVE_HDR keyword. HDR decoding is now unconditionally supported in shaders.</p></li>
<li><p>GI: Deprecated: LightmapSettings.textureCompression has been deprecated in favor of LightingSettings.lightmapCompression.</p></li>
<li><p>Graphics: Added: A class for drawing shadow cascades <code>UnityEditor.Rendering.ShadowCascadeGUI.DrawShadowCascades</code>.</p></li>
<li><p>Graphics: Added: A field to the CullingParameters structure to allow for adjustment to the near clipping plane for shadow clipping - this is independent of the rendering camera near clipping plane.</p></li>
<li><p>Graphics: Added: A new API to replace the use cases of the ShadowAuto, DepthAuto and VideoAuto GraphicsFormat enum members (which will be deprecated in the future).</p></li>
<li><p>Graphics: Added: A new Handles.DrawOutline API that allows drawing an outline in the Scene View around specified Game Objects.</p></li>
<li><p>Graphics: Added: Added a new GraphicsFormatUtility function: IsDepthStencilFormat. Returns true if the format is a depth or stencil format, returns false otherwise.</p></li>
<li><p>Graphics: Added: Added common support code for FSR.</p></li>
<li><p>Graphics: Added: Added DebugFrameTiming class that can be used by render pipelines to display CPU/GPU frame timings and bottlenecks in Rendering Debugger.</p></li>
<li><p>Graphics: Added: Added function to allocate RTHandles using <code>RenderTextureDescriptor</code>.</p></li>
<li><p>Graphics: Added: Added new DebugUI widget types: ProgressBarValue and ValueTuple.</p></li>
<li><p>Graphics: Added: Added new depth/stencil format to GraphicsFormat: D16_UNorm_S8_UInt.</p></li>
<li><p>Graphics: Added: Added support for high performant unsafe (uint only) Radix, Merge and Insertion sort algorithms on CoreUnsafeUtils.</p></li>
<li><p>Graphics: Added: Added <code>vrUsage</code> support for RTHandles allocation.</p></li>
<li><p>Graphics: Added: Allowing Rendering Layer Names to not collide in UI. Includes a new API RenderPipelineAsset.prefixedRenderingLayerMaskNames to fetch a unique list of rendering layer mask names for UI needs.</p></li>
<li><p>Graphics: Added: AMD FidelityFX shaders which were originally in HDRP.</p></li>
<li><p>Graphics: Added: An option to change the visibilty of the Volumes Gizmos (Solid, Wireframe, Everything), available at Preferences &gt; Core Render Pipeline.</p></li>
<li><p>Graphics: Added: API function inside DynamicResolutionHandler and new settings in GlobalDynamicResolutionSettings to control low res transparency thresholds. This should help visuals when the screen percentage is too low.</p></li>
<li><p>Graphics: Added: D16_UNorm_S8_UInt and S8_UInt can now be selected as depth/stencil formats inside the RenderTexture inspector.</p></li>
<li><p>Graphics: Added: Debug Panels Framework see <code>IDebugDisplaySettingsQuery</code>.</p></li>
<li><p>Graphics: Added: Exposed LockBufferForWrite and UnlockBufferAfterWrite for GraphicsBuffer (it only existed for ComputeBuffer before under the names Begin/EndWrite).<br> Exposed GraphicsBufferHandle.</p></li>
<li><p>Graphics: Added: Extended various texture constructors with the ability to create uninitialized textures. This allows for performance improvements and reduced memory usage.</p></li>
<li><p>Graphics: Added: Helper for Volumes (Enable All Overrides, Disable All Overrides, Remove All Overrides).</p></li>
<li><p>Graphics: Added: IndentLevelScope (for VolumeComponentEditor child class only) to handle indentation of the field and the checkbox.</p></li>
<li><p>Graphics: Added: New API to customize the rtHandleProperties of a particular RTHandle. This is a temporary work around to assist with viewport setup of Custom post process when dealing with DLSS or TAAU.</p></li>
<li><p>Graphics: Added: New callback: <code>QualitySettings.currentActiveQualityLevelChanged</code> It will be raised when the current quality level has been changed. The first parameter of the callback will be the previous quality level, and the second is the current one.</p></li>
<li><p>Graphics: Added: New IVolumeDebugSettings interface and VolumeDebugSettings&lt;T&gt; class that stores the information for the Volumes Debug Panel.</p></li>
<li><p>Graphics: Added: New RayTracingAccelerationStructure.CullInstances Scripting API for populating acceleration structures.</p></li>
<li><p>Graphics: Added: OverridablePropertyScope (for VolumeComponentEditor child class only) to handle the Additional Property, the override checkbox and disable display and decorator attributes in one scope.</p></li>
<li><p>Graphics: Added: SystemInfo.computeSubGroupSize API, allows users to query the size of the compute thread group that supports efficient memory sharing on the GPU.</p></li>
<li><p>Graphics: Added: SystemInfo.maxTexture3DSize API, allows users to query the largest 3D Texture size that the graphics hardware supports.</p></li>
<li><p>Graphics: Added: SystemInfo.maxTextureArraySlices API, allows users to query the maximum number of slices in a Texture array that the graphics hardware supports.</p></li>
<li><p>Graphics: Added: SystemInfo.supportsMultisampleStencilResolve API.</p></li>
<li><p>Graphics: Added: UNITY_PREV_MATRIX_M and UNITY_PREV_MATRIX_I_M shader macros to support instanced motion vector rendering.</p></li>
<li><p>Graphics: Added: VolumeComponentMenuForRenderPipelineAttribute to specify a volume component only for certain RenderPipelines.</p></li>
<li><p>Graphics: Changed: BatchRendererGroup API new design.</p></li>
<li><p>Graphics: Changed: Fixed backwards compatibility issue introduced by  #116845  (Allow the default specular reflection cubemap to be a RenderTexture (with dimensions CUBE)).</p></li>
<li><p>Graphics: Deprecated: ShadowAuto, DepthAuto and VideoAuto graphics formats and introduce a new alternative api. (See the Upgrade Guide for details.).</p></li>
<li><p>Graphics: Removed: Removed GraphicsFormatUtility.GetDepthStencilFormat(int) after being public for two alpha releases.</p></li>
<li><p>Graphics: Removed: Removed PlayerSettings.uploadClearedTextureDataAfterCreationFromScript in favor of explicit constructors on the various texture classes.</p></li>
<li><p>HDRP: Added: A built-in custom pass to draw object IDs.</p></li>
<li><p>HDRP: Added: A custom post process injection point AfterPostProcessBlurs executing after depth of field and motion blur.</p></li>
<li><p>HDRP: Added: A dialog box when you import a Material that has a diffusion profile to add the diffusion profile to global settings.</p></li>
<li><p>HDRP: Added: A minimum motion vector length to the motion vector debug view.</p></li>
<li><p>HDRP: Added: A property to control the fallback of the last bounce of a RTGI, RTR, RR ray to keep a previously existing side effect on user demand.</p></li>
<li><p>HDRP: Added: A rendering feature flag to disable LightProbeGroup editor when an alternative to standard probe is provided by the SRP.</p></li>
<li><p>HDRP: Added: Added API to edit diffusion profiles and set IES on lights.</p></li>
<li><p>HDRP: Added: Added minimal picking support for DOTS 1.0 (on parity with Hybrid Renderer V2).</p></li>
<li><p>HDRP: Added: Added new configuration ShderOptions.FPTLMaxLightCount in ShaderConfig.cs for maximum light count per fine pruned tile.</p></li>
<li><p>HDRP: Added: Added new functions that sample the custom buffer in custom passes (CustomPassSampleCustomColor and CustomPassLoadCustomColor) to handle the RTHandleScale automatically.</p></li>
<li><p>HDRP: Added: Added new panels to Rendering Debugger Display Stats panel, displaying improved CPU/GPU frame timings and bottlenecks.</p></li>
<li><p>HDRP: Added: Added option to use full ACES tonemap instead of the approximation.</p></li>
<li><p>HDRP: Added: Added public API to edit materials from script at runtime.</p></li>
<li><p>HDRP: Added: Added public API to reset path tracing accumulation, and check its status.</p></li>
<li><p>HDRP: Added: Added support for HDR output devices.</p></li>
<li><p>HDRP: Added: Added support for orthographic camera in path tracing.</p></li>
<li><p>HDRP: Added: Added support for SensorSDK's Lidar and camera models in path tracing.</p></li>
<li><p>HDRP: Added: Better support for LODs in the ray tracing acceleration structure.</p></li>
<li><p>HDRP: Added: Dependency to mathematics and burst, HDRP now will utilize this to improve on CPU cost. First implementation of burstified decal projector is here.</p></li>
<li><p>HDRP: Added: Info box when low resolution transparency is selected, but its not enabled in the HDRP settings. This will help new users find the correct knob in the HDRP Asset.</p></li>
<li><p>HDRP: Added: SG node to get the main directional light direction.</p></li>
<li><p>HDRP: Added: Shortcut to HDRP Wizard documentation.</p></li>
<li><p>HDRP: Added: Slider that controls how much the volumetric clouds erosion value affects the ambient occlusion term.</p></li>
<li><p>HDRP: Added: Slides to control the shape noise offset.</p></li>
<li><p>HDRP: Added: Support for "Always Draw Dynamic" option for directional light cached shadows.</p></li>
<li><p>HDRP: Added: Support for internal plugin materials and HDSubTarget with their versioning system.</p></li>
<li><p>HDRP: Added: Support for the camera bridge in the graphics compositor.</p></li>
<li><p>HDRP: Added: Support of motion vector buffer in custom postprocess.</p></li>
<li><p>HDRP: Added: Three animation curves to control the density, erosion, and ambient occlusion in the custom submode of the simple controls.</p></li>
<li><p>HDRP: Added: Tooltips for content inside the Rendering Debugger window.</p></li>
<li><p>HDRP: Added: ValidateMaterial callbacks to ShaderGUI.</p></li>
<li><p>HDRP: Added: Volumetric clouds support for baked and realtime reflection probes.</p></li>
<li><p>HDRP: Added: Warning for when a light is not fitting in the cached shadow atlas and added option to set maximum resolution that would fit.</p></li>
<li><p>iOS: Added: Identifiers for all iPhone 13 models, 6th generation iPad Minis, 9th generation iPads.</p></li>
<li><p>iOS: Obsoleted: PlayerSettings.iOS.allowHTTPDownload replaced by cross platform setting PlayerSettings.insecureHttpOption.</p></li>
<li><p>iOS: Removed: Removed the obsolete iOS Notification Services API. Please consider using the the "Mobile Notifications" package (available in the Unity package manager) which implements the iOS UserNotifications framework.</p></li>
<li><p>Package: Changed: Mobile Notifications 2.0.0: Fix NotificationSettings.iOSSettings.DefaultAuthorizationOptions having incorrect return type (was PresentationOption, now AuthorizationOption).</p></li>
<li><p>Package: Changed: Mobile Notifications 2.0.0: iOSNotificationTrigger.Type is no longer static and returns iOSNotificationTriggerType instead of int.</p></li>
<li><p>Particles: Added: ParticleSystem.totalTime API, to return the playback time plus any start delay.</p></li>
<li><p>Physics: Added: Added Inverse Dynamics force getter methods for Articulation Bodies.</p></li>
<li><p>Physics: Added: All the physics batch queries can now run in physics scenes other than default (see an extra RaycastCommand constructor that has physics scene as the first argument for instance).</p></li>
<li><p>Physics: Added: Expose a variant of Physics.BakeMesh that accepts cooking options.</p></li>
<li><p>Physics: Added: Expose linear and angular velocity of both of the bodies in a contact modification pair (see ModifiableContactPair.bodyLinearVelocity for example).</p></li>
<li><p>Physics: Added: Exposed per-point collision impulse (see ContactPoint.impulse).</p></li>
<li><p>Physics: Added: Exposed the forces applied to the articulation body by the articulation drives.</p></li>
<li><p>Physics: Added: Exposed the Rigidbody.maxLinearVelocity property.</p></li>
<li><p>Physics: Added: Rigidbody.Move method for moving and rotating a kinematic Rigidbody at the same time.</p></li>
<li><p>Profiler: Added: Expose <code>FrameTimingManager::IsFeatureEnabled()</code> to C#.</p></li>
<li><p>Profiler: Added: StackedArea to ProfilerModuleChartType for displaying a stacked area chart with non-time-based units.</p></li>
<li><p>Scene/Game View: Added: Added ability to specify a default container and alignment for new Overlays.</p></li>
<li><p>Scene/Game View: Added: EditorToolContext.GetAdditionalTools(), enabling Tool Contexts to define additional default tools in the same category as Move, Rotate, Scale.</p></li>
<li><p>Scene/Game View: Added: GizmoUtility class for accessing gizmo and icon visibility per component type.</p></li>
<li><p>Scene/Game View: Added: ObjectFactory.PlaceGameObject, which provides a method for placing instantiated GameObjects in the scene with the same preferences that default GameObjects are created with.</p></li>
<li><p>Scene/Game View: Added: OverlayCanvas.Add, OverlayCanvas.Remove methods to create and display Overlay instances.</p></li>
<li><p>Scene/Game View: Added: SceneView.AddActiveViewOverlay and SceneView.RemoveActiveViewOverlay to add Overlay instances that automatically follow the active Scene View.</p></li>
<li><p>Scene/Game View: Added: <code>Editor</code> classes for <code>EditorTool</code> can now implement the <code>ICreateToolbar</code> interface to create horizontal and vertical styled Overlay toolbars in addition to panel layouts.</p></li>
<li><p>Scene/Game View: Obsoleted: Moved UnityEditor.Overlays.EditorToolbarDropdownToggle to UnityEditor.Toolbars.EditorToolbarDropdownToggle. (1346398)</p></li>
<li><p>Serialization: Added: SerializedProperty has a new read only property "contentHash" to better track changes to the SerializedProperty's data.</p></li>
<li><p>Serialization: Added: SerializedProperty.boxedValue property.</p></li>
<li><p>Serialization: Added: SerializedProperty.gradientValue to the public API.</p></li>
<li><p>Serialization: Added: SerializedProperty.numericType that exposes the precise type of a numeric property (for example float versus double).</p></li>
<li><p>Serialization: Added: UintValue and ulongValue to SerializedProperty API.</p></li>
<li><p>Shadergraph: Added: A Tessellation Option to PositionNode settings, to provide access to the pre-displaced tessellated position.</p></li>
<li><p>Shadergraph: Added: A <code>Sprite</code> option to Main Preview, which is similar to <code>Quad</code> but does not allow rotation. <code>Sprite</code> is used as the default preview for URP Sprite shaders.</p></li>
<li><p>Shadergraph: Added: Added ability to automatically cast Bools to Vector types in ShaderGraph. (1359160)</p></li>
<li><p>Shadergraph: Added: Added an automatically generated material subasset on ShaderGraphs.</p></li>
<li><p>Shadergraph: Added: Added normal transforms to the Transform node.</p></li>
<li><p>Shadergraph: Added: Added ShaderGraph import warning to old nodes and properties, and ability to dismiss the warning if old behavior is desired.</p></li>
<li><p>Shadergraph: Added: Control of anisotropic settings on inline Sampler state nodes in ShaderGraph.</p></li>
<li><p>Shadergraph: Added: Custom interpolator documentation.</p></li>
<li><p>Shadergraph: Added: Information about selecting and unselecting items to the Blackboard article.</p></li>
<li><p>Shadergraph: Added: Many node synonyms for the Create Node search so that it's easier to find nodes.</p></li>
<li><p>Shadergraph: Added: Selection highlight and picking shader passes for URP target.</p></li>
<li><p>Shadergraph: Added: ShaderGraph animated preview framerate throttle.</p></li>
<li><p>Shadergraph: Added: Visible errors for invalid stage capability connections to shader graph.</p></li>
<li><p>Shaders: Added: Added LocalKeyword.isDynamic API to tell which keywords are declared as dynamic branching keywords for this shader.</p></li>
<li><p>UI Toolkit: Added: Added a MultiColumnListView control in UI Toolkit.</p></li>
<li><p>UI Toolkit: Added: Added a MultiColumnTreeView control in UI Toolkit.</p></li>
<li><p>UI Toolkit: Added: Added TreeView to the public UI Toolkit API.</p></li>
<li><p>UI Toolkit: Added: Allow custom USS styles to reference any kind of asset (through UnityEngine.Object).</p></li>
<li><p>UI Toolkit: Added: Exposed ProgressBar.lowValue and ProgressBar.highValue.</p></li>
<li><p>UI Toolkit: Added: View controllers used for ListView and TreeView are now public and can be inherited from for more control.</p></li>
<li><p>UI Toolkit: Changed: DropdownField now derives from PopupField. BasePopupField, PopupField, EnumField are moved to UnityEngine. (1308473)</p></li>
<li><p>UI Toolkit: Removed: Removed non-generic overload for retrieving a custom style property of type UnityEngine.Object.</p></li>
<li><p>URP: Added: Added Adaptive Performance Decals scaler.</p></li>
<li><p>URP: Added: Added Depth Priming support for Vulkan with MSAA.</p></li>
<li><p>URP: Added: Added Depth Texture setting for Overlay Camera.</p></li>
<li><p>URP: Added: Added Display Stats panel to Rendering Debugger that displays CPU/GPU frame timings and bottlenecks.</p></li>
<li><p>URP: Added: Added minimal picking support for DOTS 1.0 (on parity with Hybrid Renderer V2).</p></li>
<li><p>URP: Added: Added Shadows and Additional Lights off variants stripping.</p></li>
<li><p>URP: Added: Added support for <code>RTHandle</code>.</p></li>
<li><p>URP: Added: Depth Texture setting for Overlay Camera.</p></li>
<li><p>URP: Added: Emulate alpha for multiply blend mode by whitening the base map colors using the alpha value. Keyword _ALPHAMODULATE_ON is set for multiply blend mode.</p></li>
<li><p>URP: Added: Exposed public API for DebugDisplaySettings.</p></li>
<li><p>URP: Added: GetUniversalAdditionalLightData, a method that returns the additional data component for a given light or create one if it doesn't exist yet.</p></li>
<li><p>URP: Added: Help button on material editor to show the shader documentation page.</p></li>
<li><p>URP: Added: Lights 2D to the Light Explorer window.</p></li>
<li><p>URP: Added: Motion Vector render pass for URP.</p></li>
<li><p>URP: Added: Preserve Specular blend mode toggle for glass like materials where the specular reflection itself is not transparent.</p></li>
<li><p>URP: Added: Public api and updated docs for Light2D shape properties.</p></li>
<li><p>URP: Added: Render Settings Converter to the Render Pipeline Converter, this tool creates and assigns URP Assets based off rendering settings of a Builtin project.</p></li>
<li><p>URP: Added: Support for default sprite mask shaders for the 2D Renderer in URP.</p></li>
<li><p>URP: Added: Terrain grass shader alpha changed to always write 1 to alpha. Enabled alpha channel write mask.</p></li>
<li><p>URP: Added: Two new URP specific scene templates, Basic which has a camera and directional light, then Standard which has the addition of a global volume with basic post effects setup.</p></li>
<li><p>URP: Added: URP global setting for stripping off shader variants.</p></li>
<li><p>URP: Added: URP global setting for stripping post processing shader variants.</p></li>
<li><p>URP: Added: VFX: Fix light cookies integration.</p></li>
<li><p>URP: Added: XR: Added Late Latching support to reduce VR latency (Quest).</p></li>
<li><p>URP: Changed: Fixed incorrect shadow fade in deferred rendering mode.</p></li>
<li><p>VFX Graph: Added: An 'Is Inside' subgraph into VFX Graph additions package.</p></li>
<li><p>VFX Graph: Added: HDRP Decal output context.</p></li>
<li><p>VFX Graph: Added: Motion vectors enabled for particle strips.</p></li>
<li><p>VFX Graph: Added: Multiple VFX graphs can be opened at the same time.</p></li>
<li><p>VFX Graph: Added: New options to select how to sort particles in the Output Context.</p></li>
<li><p>VFX Graph: Added: Provide explicit access to spawnCount in graph.</p></li>
<li><p>VFX Graph: Added: Structured Graphics Buffer support as exposed type.</p></li>
<li><p>VFX Graph: Added: Support of direct link event to initialize context (which support several event within the same frame).</p></li>
<li><p>VFX Graph: Added: The VFX editor will now automatically attach to the current selection if the selected gameobject uses the currently edited VFX asset.</p></li>
<li><p>VFX Graph: Added: Two new buttons are available in the editor's tool bar. One will display a popup panel to handle attachement and the other to lock/unlock the current attachment.</p></li>
<li><p>WebGL: Deprecated: For WebGL builds, the WebGL 1 API is no longer included in the Auto Graphics API option (the default). If you need to build for both WebGL 1 and WebGL 2, uncheck the Auto Graphics API and manually add WebGL 1 to the Graphics APIs list.</p></li>
<li><p>Windows: Added: UnityEngine.Windows.Input.ForwardRawInput now has a second overload that is usable without enabling unsafe code.</p></li>
<li><p>XR: Added: Support for late latched previous view matrix for URP motion vectors.</p></li>
</ul>

### Changes
<ul>
<li><p>2D: 2D Template now starts with Sprite Atlas v2 as default Sprite Packing method.</p></li>
<li><p>2D: 2D URP Template now starts with Sprite Atlas v2 as default Sprite Packing method.</p></li>
<li><p>2D: Allow non-public fields with the SerializeField attribute as custom fields for RuleTile.</p></li>
<li><p>2D: Changed some of PSDImporter settings to use checkboxes instead of drop down.</p></li>
<li><p>2D: Changed Sprite Inspector to show border values in pixel unit.</p></li>
<li><p>2D: Changed the information in the Sprite Editor Window's slicing tool to clarify the different slicing methods available.</p></li>
<li><p>2D: Replace usage of Triangle.Net with in house tessellation solution.</p></li>
<li><p>2D: Updated 2D Template to use new package format structure.</p></li>
<li><p>2D: Updated 2D URP Template to use new package format structure.</p></li>
<li><p>Android: Allow Android Player to use Vulkan on GPUs that are currently unknown to Unity on Android 11 or newer.</p></li>
<li><p>Android: Android Gradle Plugin version upgraded from 3.6.0 to 4.0.1.</p></li>
<li><p>Android: Gradle version upgraded from 5.6.4 to 6.1.1.</p></li>
<li><p>Android: Pdb files in development builds will now be stored along with the main apk file or main asset pack.</p></li>
<li><p>Animation: Added a warning to the user in case a transition that is smaller than a fixed update with root motion and non looping clip is made. (<a href="https://issuetracker.unity3d.com/issues/the-movement-speed-of-an-animation-is-inconsistent-for-a-single-frame-when-transitioning-between-animations">1336151</a>)</p></li>
<li><p>Build Pipeline: Enabling or disabling modules will now cause a data rebuild in the incremental build pipeline.</p></li>
<li><p>Build Pipeline: It is no longer possible to build a player when a script reload is pending. (<a href="https://issuetracker.unity3d.com/issues/crash-caused-by-compile-pipeline-contradiction-with-corrupted-class-slash-scene-loading">1325753</a>)</p></li>
<li><p>Burst: Burst now generates a link.xml automatically to avoid issues with stripping causing missing symbols at runtime from static constructor usage.</p></li>
<li><p>Burst: Burst now produces at most 100 jobs per DLL it creates, meaning that big assemblies will still benefit from multithreading while retaining the benefits of Burst 1.7 (significantly less DLLs, and batching of frontend and optimizer costs).</p></li>
<li><p>Burst: Burst now waits for all threads to complete on shutdown, rather than performing a thread abort, as that could lead to a race condition with Dispose.</p></li>
<li><p>Burst: Changed how we display the timings when a user has the <strong>Show Timings</strong> option enabled in the Burst menu, by cleaning up and presenting the information in a (hopefully!) clearer way.</p></li>
<li><p>Burst: Changed the optimization pipeline to run the loop unroller <em>exclusively</em> after the loop vectorizer. This improves codegen in a lot of cases (mostly because the SLP vectorizer is unable to vectorize all the code that the loop unroller could have).</p></li>
<li><p>Burst: Don't move pdbs out of build folder for UWP builds.</p></li>
<li><p>Burst: Fixed "error while hashing" message that could appear during compilation.</p></li>
<li><p>Burst: Improved iteration time by triggering Burst compilation immediately after .NET assemblies have been compiled.</p></li>
<li><p>Burst: Improved the compiler performance when doing large struct copies by detecting more cases where a load/store can be safely converted to a move-memory operation.</p></li>
<li><p>Burst: Intrinsics: Neon vst1 APIs are now fully supported.</p></li>
<li><p>Burst: Made the cost of initializing Direct Call methods for execution 33x faster during domain reload.</p></li>
<li><p>Burst: Made the <code>SharedStatic</code> initialization cost during static constructor initialization time 13.3x faster.</p></li>
<li><p>Burst: Made <code>fmod</code> and floating-point modulus use a faster algorithm to improve performance.</p></li>
<li><p>Burst: Removed the player build <code>BC1370</code> exception warnings as users only found them annoying.</p></li>
<li><p>Burst: Removed the <code>Use Platform SDK Linker</code> option from Burst AOT Settings for desktop platforms.</p></li>
<li><p>Burst: Updated the minimum Xcode required for Burst to compile for the Apple iOS/tvOS plaforms to 12.0.</p></li>
<li><p>Burst: Upgraded Burst to use LLVM Version 12.0.0 by default, bringing the latest optimization improvements from the LLVM project.</p></li>
<li><p>Burst: Used <code>BuildReport::summary::subtarget</code> to detect headless (server) player builds on 2022.1+.</p></li>
<li><p>Editor: Contextual shortcuts are now preferred over global ones and no longer cause conflicts in ShortcutManager.</p></li>
<li><p>Editor: EditorGUI.MaskField now uses the same dropdown UI style as the EditorGUI.LayerMaskField.</p></li>
<li><p>Editor: Excluded Mesh, Texture2D and Texture2dArray from Presets. (<a href="https://issuetracker.unity3d.com/issues/crash-after-selecting-presets-for-large-textures">1325555</a>)</p></li>
<li><p>Editor: Removed Project Settings Service default entries. It should be empty if no Services package are installed.</p></li>
<li><p>Editor: Script names will be displayed together with their namespaces in the Add Component search results. (1264749)</p></li>
<li><p>Editor: UI widget used for Light Cookies from the standard Property Field to the ObjectField that provides texture preview and asset directory search capabilities, across HDRP and built-in.</p></li>
<li><p>Editor: Use order_preserving_vector_set_hashed to store gameobjects, filtered and transform (same data structure as Selection.objects). This ensures assigning to the selection preserve order of the items. (<a href="https://issuetracker.unity3d.com/issues/selection-dot-transforms-returns-a-randomly-ordered-array">915931</a>)</p></li>
<li><p>Editor: When a Mask Field contains mixed values it will now show a list of the values in the label. The label will revert back to showing "Mixed..." when there is not enough space to show the list. (<a href="https://issuetracker.unity3d.com/issues/culling-mask-component-value-displays-as-mixed-dot-dot-dot-when-two-or-more-items-are-selected">1266226</a>)</p></li>
<li><p>Editor: When performing incremental build (Android, Windows, OSX, WebGL, iOS), player assemblies will be placed now in Library/Bee folder rather than Library folder, and will persist until the next build.</p></li>
<li><p>Graph Tool Foundation: Graph Tools Foundation edges drawing was changed from Bezier curves to Z-lines.</p></li>
<li><p>Graphics: Added depth resolve support to the RenderPass API for the case when the RenderTexture is not in the tempRT stack.</p></li>
<li><p>Graphics: Added depth resolve support to the RenderPass API.</p></li>
<li><p>Graphics: Creating a RenderTexture with no depth bits specified will now fail instead of continuing with a warning. (1348764)</p></li>
<li><p>Graphics: Cubemap pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData &amp; SetPixel/SetPixels/SetPixels32/SetPixelData) now throw an ArgumentException when encountering an error.</p></li>
<li><p>Graphics: CubemapArray pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData &amp; SetPixel/SetPixels/SetPixels32/SetPixelData) now throw an ArgumentException when encountering an error.</p></li>
<li><p>Graphics: DX12 doesn't revert to worse texture detail anymore, when the GPU memory is running out.</p></li>
<li><p>Graphics: DynamicResolutionHandler.GetScaledSize function now clamps, and  will never allow to return a size greater than its input.</p></li>
<li><p>Graphics: Improved IntegrateLDCharlie() to use uniform stratified sampling for faster convergence towards the ground truth.</p></li>
<li><p>Graphics: Improved the warning messages for Volumes and their Colliders.</p></li>
<li><p>Graphics: LensFlare (SRP) can be now disabled per element.</p></li>
<li><p>Graphics: LensFlare (SRP) tooltips now refer to meters.</p></li>
<li><p>Graphics: LensFlare Element editor now have Thumbnail preview.</p></li>
<li><p>Graphics: Mark OpenGL ES 2.0 as deprecated in Graphics API selection UI.</p></li>
<li><p>Graphics: Removed DYNAMIC_RESOLUTION snippet on lens flare common shader. Its not necessary any more on HDRP, which simplifies the shader.</p></li>
<li><p>Graphics: Serialize the Probe Volume asset as binary to improve footprint on disk and loading speed.</p></li>
<li><p>Graphics: Texture2DArray pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData &amp; SetPixel/SetPixels/SetPixels32/SetPixelData) now throw an ArgumentException when encountering an error.</p></li>
<li><p>Graphics: Texture3D pixel access functions (GetPixel/GetPixels/GetPixels32/GetPixelData &amp; SetPixel/SetPixels/SetPixels32/SetPixelData) now throw an ArgumentException when encountering an error.</p></li>
<li><p>Graphics: Uniformize the names in ReflectionProbes along render pipelines.</p></li>
<li><p>Graphics: Updated icon for IES, LightAnchor and LensFlare.</p></li>
<li><p>Graphics: WebCamTexture pixel access functions (GetPixel/GetPixels/GetPixels32) now throw an ArgumentException when encountering an error. Calling these functions before the first frame update will throw an exception instead of returning blank data.</p></li>
<li><p>HDRP: Added controls for the users to manually feed the ray tracing acceleration structure that should be used for a given camera.</p></li>
<li><p>HDRP: Changed light reset to preserve type.</p></li>
<li><p>HDRP: Changed the Channel Mixer Volume Component UI.Showing all the channels.</p></li>
<li><p>HDRP: Changed the debug panel mip bias functions from public to internal.</p></li>
<li><p>HDRP: Changed the NVIDIA install button to the standard FixMeButton.</p></li>
<li><p>HDRP: Changed the storage format of volumetric clouds presets for easier editing.</p></li>
<li><p>HDRP: Disabled the "Reflect Sky" feature in the case of transparent screen space reflections for the water system.</p></li>
<li><p>HDRP: Display an info box and disable MSAA  asset entry when ray tracing is enabled.</p></li>
<li><p>HDRP: Fixed minor readability issues in the ray tracing code.</p></li>
<li><p>HDRP: Hair uses GGX LTC for area light specular.</p></li>
<li><p>HDRP: HD's SpeedTree 8 upgrader now sets up CullModeForward as well.</p></li>
<li><p>HDRP: Ignore hybrid duplicated reflection probes during light baking.</p></li>
<li><p>HDRP: Improved a bit the area cookie behavior for higher smoothness values to reduce artifacts.</p></li>
<li><p>HDRP: Improved sampling of overlapping point/area lights in path-traced volumetric scattering. (1358777)</p></li>
<li><p>HDRP: Improved the DynamicArray class by adding several utility APIs.</p></li>
<li><p>HDRP: Improved the fly through ghosting artifacts in the volumetric clouds.</p></li>
<li><p>HDRP: Improved to the RTGI denoising.</p></li>
<li><p>HDRP: Improved volumetric clouds (added new noise for erosion, reduced ghosting while flying through, altitude distortion, ghosting when changing from local to distant clouds, fix issue in wind distortion along the Z axis).</p></li>
<li><p>HDRP: In path tracing, camera ray misses now return a null value with Minimum Depth &gt; 1.</p></li>
<li><p>HDRP: Increased the minimal density of the volumetric clouds.</p></li>
<li><p>HDRP: Integrate a help box to inform users of the potential dependency to directional lights when baking.</p></li>
<li><p>HDRP: Made ACEScg the default color space for color grading.</p></li>
<li><p>HDRP: Make LitTessellation and LayeredLitTessellation fallback on Lit and LayeredLit respectively in DXR.</p></li>
<li><p>HDRP: MaterialReimporter.ReimportAllMaterials and MaterialReimporter.ReimportAllHDShaderGraphs now batch the asset database changes to improve performance.</p></li>
<li><p>HDRP: Modified HDRP to use common FSR logic from SRP core.</p></li>
<li><p>HDRP: Moved AMD FidelityFX shaders to core.</p></li>
<li><p>HDRP: Moved area light's shadow frustum: light's surface no longer passes through the apex, and instead aligns with the 0-offset near plane.</p></li>
<li><p>HDRP: Moved invariants outside of loop for a minor CPU speedup in the light loop code.</p></li>
<li><p>HDRP: Moved supportRuntimeDebugDisplay option from HDRPAsset to HDRPGlobalSettings.</p></li>
<li><p>HDRP: Optimizations for the physically based depth of field.</p></li>
<li><p>HDRP: Optimized color grading LUT building.</p></li>
<li><p>HDRP: Optimized FSR by merging the RCAS logic into the FinalPass shader.</p></li>
<li><p>HDRP: Path-traced volumetric scattering now takes fog color into account, adding scattered contribution on top of the non-scattered result (case 1346105, 1358783). (<a href="https://issuetracker.unity3d.com/issues/hdrp-dxr-path-tracing-renders-distant-volumetric-fog-pure-black-if-maximum-height-fog-parameter-is-lower-than-camera-height">1346105</a>, 1358783)</p></li>
<li><p>HDRP: PrepareLightsForGPU CPU Light loop performance improvement (40% to 70% faster), utilizing burst and optimized. Utilizing better sorting, distributing work in jobs and improving cache access of light data.</p></li>
<li><p>HDRP: Reduced the maximum distance per ray step of volumetric clouds.</p></li>
<li><p>HDRP: Removed Bilinear and Lanczos upscale filter.</p></li>
<li><p>HDRP: Removed redundant Show Inactive Objects and Isolate Selection checkboxes from the Emissive Materials tab of the Light Explorer.</p></li>
<li><p>HDRP: Renaming Decal Projector to HDRP Decal Projector.</p></li>
<li><p>HDRP: Replaced the context menu by a search window when adding custom pass.</p></li>
<li><p>HDRP: Restore old version of the RendererList structs/api for compatibility.</p></li>
<li><p>HDRP: Restructured data under Display Stats panel to use column layout.</p></li>
<li><p>HDRP: Surface ReflectionTypeLoadExceptions in HDUtils.GetRenderPipelineMaterialList(). Without surfacing these exceptions, developers cannot act on any underlying reflection errors in the HDRP assembly.</p></li>
<li><p>HDRP: TAA jitter is disabled while using Frame Debugger now.</p></li>
<li><p>HDRP: The HDRP Render Graph now uses the new RendererList API for rendering and (optional) pass culling.</p></li>
<li><p>HDRP: Updated the recursive rendering documentation.</p></li>
<li><p>HDRP: Use RayTracingAccelerationStructure.CullInstances to filter Renderers and populate the acceleration structure with ray tracing instances for improved CPU performance on the main thread.</p></li>
<li><p>HDRP: Various improvements to the volumetric clouds.</p></li>
<li><p>HDRP: Visual Environment ambient mode is now set to Dynamic by default.</p></li>
<li><p>HDRP: When a ray hits the sky in the ray marching part of mixed ray tracing, it is considered a miss.</p></li>
<li><p>IL2CPP: Code generation option moved from build settings (EditorUserBuildSettings.il2CppCodeGeneration<br> ) to player settings (PlayerSettings.SetIl2CppCodeGeneration/PlayerSettings.GetIl2CppCodeGeneration). This option is now per platform and persisted with the project.</p></li>
<li><p>IL2CPP: Removed un-needed generic method context initialization calls.</p></li>
<li><p>Input System: When exceptions occur in user code inside of Input System callbacks, the exception message is now printed first and details about the callback second to avoid hiding exception details.</p></li>
<li><p>iOS: IOS 12 is now minimum supported iOS version.</p></li>
<li><p>Networking: UnityWebRequest by default is HTTPS only now. Plain text HTTP can be enabled in Player Settings.</p></li>
<li><p>Package: (Recorder) Prevent invalid GPU callback data from being written to a frame: this change skips the problematic frame and logs an error message.</p></li>
<li><p>Package: Added the Code Coverage package to the Engineering feature set.</p></li>
<li><p>Package: Updated nodejs ini package to fix vulnerability issue. (1345229)</p></li>
<li><p>Package: Visual Scripting<br></p> 
<ul>
<li>Removed unused Preferences<br></li>
<li>Renamed preference "Update Units Automatically" to "Update Nodes Automatically".</li>
</ul></li>
<li><p>Package Manager: Changed error and warning box to look like the info box.</p></li>
<li><p>Package Manager: Following the review of the 2 new tabs (Tools &amp; Services) in package manager, the PM and Design Team recommended to remove the Tools tab.</p></li>
<li><p>Package Manager: Replaced the communication layer between Unity and the Unity Package Manager to connect using IPC instead of HTTP in order to solve a number of connectivity issues.</p></li>
<li><p>Package Manager: The Git LFS cache enabled by setting the <code>UPM_ENABLE_GIT_LFS_CACHE</code> environment variable is now always located under the global cache root, even when the cache root location is customized.</p></li>
<li><p>Package Manager: We are no longer using SCSS files, only USS from now on.</p></li>
<li><p>Package Manager: We now cache whether each asset version is a full project or not after clicking Import on it for the first time.</p></li>
<li><p>Prefabs: Removed disconnected state for Prefab instances.</p></li>
<li><p>Profiler: Added UnityEngine.Object lifecycle tracing to the Unity Profiler.</p></li>
<li><p>Profiler: The command-line argument "-profiler-log-file" now not only sets profiler target file but also activates profiler. (1339129)</p></li>
<li><p>Scene/Game View: Removed Component Tools Overlay, these tools are now available in the regular Tools Overlay.</p></li>
<li><p>Scene/Game View: Unavailable tools are now hidden rather than disabled in the Scene View Tools Overlay.</p></li>
<li><p>Search: Improved asset indexer performances and index size. (1343812)</p></li>
<li><p>Services: Added Services top menu for services discovery.</p></li>
<li><p>Services: Unity Analytics renamed to Legacy Analytics in order to aid deprecation of the Analytics package.</p></li>
<li><p>Shadergraph: Adjusted Blackboard article to clarify multi-select functionality.</p></li>
<li><p>Shadergraph: Changed "Create Node" action in ShaderGraph stack separator context menu to "Add Block Node" and added it to main stack context menu.</p></li>
<li><p>Shadergraph: Changed the title suffix on old nodes and properties rom "Deprecated" to "Legacy".</p></li>
<li><p>Shadergraph: Only ShaderGraph keywords count towards the shader permutation variant limit, SubGraph keywords do not.</p></li>
<li><p>Shadergraph: Removed use of deprecated UNITY_USE_NATIVE_HDR keyword in shaders.</p></li>
<li><p>Shadergraph: ShaderGraph SubGraphs will now report errors and warnings in a condensed single error.</p></li>
<li><p>uGUI: Removed the HideFlags.HideAndDontSave on the mesh inside Graphics for it to get properly cleaned up on both managed and native side. (<a href="https://issuetracker.unity3d.com/issues/ui-meshes-and-event-system-objects-not-removed-between-instances-of-player">1319556</a>)</p></li>
<li><p>uGUI: Updated the context menu order and grouped all non-TMP game objects and components under legacy.</p></li>
<li><p>UI Toolkit: Asset types referenced from USS files are now enforced on a per-property basis and generates warnings instead of errors.</p></li>
<li><p>UI Toolkit: The inner hierarchy of InputFiels was altered. Queries that relied on a specific hierarchy order might be affected. Callbacks that were registered on inner components of the InputField might also be affected.<br> Examples of such queries:<br></p>

<ul>
<li>field.hierarchy[1]<br></li>
<li>visualElement.Q&lt;ScrollView&gt;()<br>
Example of invalid RegisterCallback:<br></li>
<li>Field.Q("unity-text-input").RegisterCallback&lt;Event&gt;(OnEvent);<br>
Might need to be updated to:<br></li>
<li>Field.RegisterCallback&lt;Event&gt;(OnEvent, TrickleDown.TrickleDown);.</li>
</ul></li>
<li><p>URP: 2D Lights now inherit from Light2DBase.</p></li>
<li><p>URP: Changed default target sorting layers of Light2D to "Everything". Newly added sorting layers will be included in Light2Ds that have target sorting layers already set to "Everything".</p></li>
<li><p>URP: Changed the default name when a new urp asset is created.</p></li>
<li><p>URP: Converted internal render targets to use <code>RTHandle</code> targets instead of <code>RenderTargetHandle</code> and <code>RenderTargetIdentifier</code>.</p></li>
<li><p>URP: Improved blending modes trigger a material update which tries to keep the existing look intact. This is not always possible and manual blend mode changes might be required.</p></li>
<li><p>URP: Main light shadow, additional light shadow and additional light keywords are now enabled based on urp setting instead of existence in scene. This allows better variant stripping.</p></li>
<li><p>URP: MaterialReimporter.ReimportAllMaterials now batches the asset database changes to improve performance.</p></li>
<li><p>URP: Multiply blend now keeps DstAlpha as it's RGB only.</p></li>
<li><p>URP: Now using the SpeedTree8 PBRLit shadergraph as the default SpeedTree8 shader for Universal.</p></li>
<li><p>URP: Particle AlphaModulate() renamed to AlphaModulateAndPremultiply() as it does both. Moved separate AlphaModulate() and AlphaPremultiply() to URP shader library. Fix double alpha multiply for ParticleLit.</p></li>
<li><p>URP: Refactored some of the array resizing code around decal projector rendering to use the new APIs in render core.</p></li>
<li><p>URP: Removed experimental tile deferred code.</p></li>
<li><p>URP: Removed the name input for the SSAO and Screen Space Shadows renderer features.</p></li>
<li><p>URP: Removed use of deprecated UNITY_USE_NATIVE_HDR keyword in shaders.</p></li>
<li><p>URP: Separated Premultiplied blend mode and Preserve Specular Lighting feature from each other. Premultiplied blend mode is now true straight premultiply mode. Preserve Specular Lighting, which applies alpha differently for diffuse and specular parts of lighting, is now a separate option for Alpha and Additive blend modes. The results of previous Premultiplied blend implementation can be achieved by using Alpha blend mode with Preserve Specular Lighting toggled on.</p></li>
<li><p>URP: Set usage of <code>RenderTargetHandle</code> and public functions using <code>RenderTargetIdentifier</code> as obsolete for future removal.</p></li>
<li><p>URP: Split RendererFeatures <code>AddRenderPasses</code> into two functions with <code>SetupRenderPasses</code> so render targets can be used after allocation.</p></li>
<li><p>URP: Stripping shader variants per renderer features instead of combined renderer features.</p></li>
<li><p>URP: The behavior of setting a camera's Background Type to "Dont Care" has changed on mobile. Previously, "Dont Care" would behave identically to "Solid Color" on mobile. Now, "Dont Care" corresponds to the render target being filled with arbitrary data at the beginning of the frame, which may be faster in some situations. Note that there are no guarantees for the exact content of the render target, so projects should use "Dont care" only if they are guaranteed to render to, or otherwise write every pixel every frame.</p></li>
<li><p>URP: UniversalRendererData and ForwardRendererData GUIDs have been reversed so that users coming from 2019LTS, 2020LTS and 2021.1 have a smooth upgrade path.  For 2021.2 Alpha/Beta users, you may encounter issues and are strongly recommended to start with a fresh library if initial upgrade fails.</p></li>
<li><p>URP: URP Asset Inspector - Advanced settings have been reordered under <code>Show Additional Properties</code> in each section.</p></li>
<li><p>URP: URP Asset Inspector - <code>General</code> section has been renamed to <code>Rendering</code>.</p></li>
<li><p>URP: URP will no longer render via an intermediate texture unless actively required by a Renderer Feature. See the upgrade guide for compatibility options and how assets are upgraded.</p></li>
<li><p>URP: VFX: New shadergraph support directly on Universal target.</p></li>
<li><p>URP: When MSAA is enabled and a depth texture is required, the opaque pass depth will be copied instead of scheduling a depth prepass.</p></li>
<li><p>Version Control: ### Changed<br></p> 
<ul>
<li>Updating license to better conform with expected customer usage.<br></li>
<li>Updated documentation file to meet standards.<br></li>
<li>Updated third-party usage.<br></li>
<li>No longer requires downloading of the full Plastic client. Basic features will work without additional installation. Features that require the full Plastic client will allow download and install as needed.<br></li>
<li>Usability improvements around checking in code<br></li>
<li>Improved update workspace tab UX<br></li>
<li>Plastic SCM context menu is now available even if the Plastic SCM window is closed.</li>
</ul></li>
<li><p>Version Control: Changed the default metadata columns shown in the Incoming Changes screen.</p></li>
<li><p>Version Control: Migration tests<br> Improved usage analytics around Editor and Plugin version<br>
Workspace Migration Adjustments.</p></li>
<li><p>Version Control: Moved Plastic Package settings to the Unity Project Settings window<br> Refined styling for Updating Workplace success state<br>
Updated texts for empty state and overview bar<br>
Removed Incoming Changes notification from empty state<br>
Updated the text for Forced Checkout option<br>
Refined the status overlay icons<br>
Updated the refresh icon on the toolbar<br>
Updated the texts for empty checkin message dialog.</p></li>
<li><p>Version Control: Removed category icons from views<br> Removed "com.unity.services.core" package dependency.</p></li>
<li><p>Version Control: Removed pinstriping in the Gluon Incoming Changes window.</p></li>
<li><p>Version Control: Removed the "Nothing to download" bar from the Incoming Changes window when there are no items to download.</p></li>
<li><p>Version Control: Removed the unneeded refresh button from History Tab<br> Moved search bar to the top right global icon section in all tabs<br>
Updated capitalization of options in the Settings context menu<br>
Updated tab button styling to be consistent with Unity Editor conventions<br>
Status bar visible across all tabs<br>
Moved refresh button to the toolbar at the top right corner of the window<br>
Moved changesets time period selector to the right corner of the window<br>
Removed "Changes of changeset" header on the Changesets tab<br>
Moved number of selected items next to "Item" metadata title on the Pending Changes tab<br>
Improved refresh icon resolution<br>
Changed changesets detail to appear in vertical column<br>
Reduced default number of columns in changesets tab<br>
The number of changesets is no longer displayed in changesets tab<br>
Changed Launch branch explorer into an icon with tooltip<br>
Removed the hide changes button in changesets tab<br>
Moved incoming change prompt and button into a status bar<br>
Changed "Launch Plastic" to "Launch Plastic SCM" in options menu<br>
Wording change for plastic installation<br>
Updated file status icons.</p></li>
<li><p>Version Control: Simplified UI: decluttered UI.</p></li>
<li><p>Version Control: Updated checkin comment box to keep the last comment after checkin error.</p></li>
<li><p>Version Control: Updated file overlay icon size to adapt to project window zoom level<br> Updated the styling of number of items in a category in Gluon incoming changes view.</p></li>
<li><p>Version Control: Updated status bar notification icons<br> Updated texts for workspace modes selection and checkin comment box.</p></li>
<li><p>Version Control: Updated styling of number of items in incoming changes category<br> Improved plugin initialization process and let the plugin functions without needing the Plastic window opened<br>
Disabled the invite button when user does not have invite permission or not on a cloud repo.</p></li>
<li><p>Version Control: Updated the alignment of sorting arrows to the right of the column.</p></li>
<li><p>VFX Graph: Search window now lists more nodes variants and they are organized by attribute first instead of operation.</p></li>
<li><p>VFX Graph: Transform integrated to VFXTypes : Circle, ArcCircle, Sphere, ArcSphere, Torus, ArcTorus, Cone, ArcCone.</p></li>
<li><p>Virtual Texturing: Now <code>PopRequests</code> allows the destination list to have a different size than the texture stack's <code>maxActiveRequests</code> value.</p></li>
<li><p>XR: Renamed XR Tools Utilities package to XR Core Utilities package.</p></li>
</ul>

### Fixes
<ul>
<li><p>2D: A non-descriptive error is thrown when building with a Texture that has it's rectangle out of bounds. (<a href="https://issuetracker.unity3d.com/issues/a-non-descriptive-error-is-thrown-when-building-with-a-texture-that-has-its-rectangle-out-of-bounds">1300130</a>)</p></li>
<li><p>2D: Activated Tile Palette Tool is now deactivated when Tool is removed from Default Tools. (1342201)</p></li>
<li><p>2D: Fixed an issue where Renderers SortingOrder property could not be animated. (<a href="https://issuetracker.unity3d.com/issues/2d-sorting-layer-order-in-layer-key-resets-to-0-in-animation-window-and-in-inspector">1386158</a>)</p></li>
<li><p>2D: Fixed an issue with culling of TilemapRenderer Tiles when a user sets a value for the Camera's culling matrix and a SRP asset is used. (<a href="https://issuetracker.unity3d.com/issues/chunk-and-individual-mode-tilemaps-are-culled-when-the-tilemaps-vertex-position-is-displaced-with-a-shader">1362522</a>)</p></li>
<li><p>2D: Fixed artifacts on images when flatten for PSDImporter.</p></li>
<li><p>2D: Fixed editor crash when calling SpriteAtlasUtility.PackAtlases. (<a href="https://issuetracker.unity3d.com/issues/sprite-atlas-v1-editor-crashes-when-calling-spriteatlasutility-dot-packatlases">1353609</a>)</p></li>
<li><p>2D: Fixed exception "PsdInvalidException: Unrecognized layer section type" when importing certain files.</p></li>
<li><p>2D: Fixed exception when adding a new Rule when no Rule is selected.</p></li>
<li><p>2D: Fixed issue where a scriptedTile without LockTransform set but has a transform matrix in GetTileData is dropped onto the Tile Palette, the Tile on the Tile Palette does not match the transform matrix as defined in GetTileData. (1341938)</p></li>
<li><p>2D: Fixed Sprite Editor Window does not show texture preview with the correct filtering mode. (1350446)</p></li>
<li><p>2D: Fixed Sprite Editor Window to be disabled when readonly assets are selected. (1343237)</p></li>
<li><p>2D: Fixed Sprite Frame module inspector size jitters in certain occasions.</p></li>
<li><p>2D: Fixed the isolate behavior in the Sprite tab in the Visibility panel. (1387184)</p></li>
<li><p>2D: Fixed Tile Palette window incorrectly preventing selection in Scene View when Tilemap Tools are inactive. (<a href="https://issuetracker.unity3d.com/issues/gameobjects-in-the-scene-are-not-selectable-when-using-w-after-painting-with-tile-pallete">1365564</a>)</p></li>
<li><p>2D: Fixed upgrade issue when atlas v1 to v2 causes objects in folders to become ungrouped. (<a href="https://issuetracker.unity3d.com/issues/2d-sprite-atlas-v2-upgrading-atlas-to-v2-causes-objects-in-folders-to-become-ungrouped">1354054</a>)</p></li>
<li><p>2D: Secondary Texture AssetImporter reference error when using same texture as Main Texture in Sprite Editor. (<a href="https://issuetracker.unity3d.com/issues/secondary-texture-assetimporter-reference-error-when-using-same-texture-as-main-texture-in-sprite-editor">1331542</a>)</p></li>
<li><p>2D: Validate and refresh Tilemap when loaded from a separate scene. (<a href="https://issuetracker.unity3d.com/issues/tiles-are-not-animated-when-one-scene-loads-from-another-scene">1344979</a>)</p></li>
<li><p>2D: [RuleTile] Fixed error in RuleTileEditor when removing all Rules and adding a new Rule.</p></li>
<li><p>AI: Fixed crashes from building the NavMesh from meshes without valid vertex data. (<a href="https://issuetracker.unity3d.com/issues/crash-on-rasterizetri-when-static-batching-passes-invalid-mesh-data-into-the-navmesh-build-process">1315584</a>)</p></li>
<li><p>AI: Fixed how the NavMesh is computed in some situations where multiple ledges in the environment form a steep slope (e.g. computing NavMesh on a narrow stair which has hand rails). (<a href="https://issuetracker.unity3d.com/issues/a-small-gap-is-created-in-the-default-navmesh-when-setting-step-height-from-0-dot-76-to-1-dot-08-and-baking-navmesh">1074084</a>)</p></li>
<li><p>Android: Changed boost documentation and timing values in the simulator to reflect the boost mode timing of 10s instead of the previous 15 seconds as it changes on the driver side.</p></li>
<li><p>Android: Changed bottleneck profiler colors to reflect warning states correctly.</p></li>
<li><p>Android: Fixed error to log about isHdr method not found on Android 7 devices. (<a href="https://issuetracker.unity3d.com/issues/android-profiler-nosuchmethoderror-is-thrown-when-auto-connecting-profiler-to-samsung-galaxy-s8">1402949</a>)</p></li>
<li><p>Android: Fixed exporting Android Studio project to non-existing folder using Editor API. (<a href="https://issuetracker.unity3d.com/issues/buildpipeline-dot-buildplayer-throws-the-build-cannot-be-appended-exception-when-using-acceptexternalmodificationstoplayer-option">1347960</a>)</p></li>
<li><p>Android: Fixed frequency change error case (e.g. when boost is activated). Does not retry every frame. Manual retry is required.</p></li>
<li><p>Android: Fixed simulator where temperature level and trend would not get updated when thermal action was updated.</p></li>
<li><p>Android: Il2cpp resources will be extracted during player launch only when needed, for ex., changes in scripts. Previously they would be extracted each time you make a new build from Unity.</p></li>
<li><p>Android: In the new input system, the search, call, endcall, camera, focus, and headsethook keys were all mapped to various function keys. These mappings are not helpful on any current platforms, and in the case of the search key, this mapping is wrong on Chrome OS keyboards which have separate search and F2 keys. (1343608)</p></li>
<li><p>Android: Provide user friendly error message when attempting to use application patching on Chrome OS devices. (<a href="https://issuetracker.unity3d.com/issues/chromeos-when-patch-and-patch-and-run-build-options-are-used-there-is-no-clear-error-message-why-the-build-fails">1367588</a>)</p></li>
<li><p>Android: Removed 'Experimental' tag from Split APK by architectures, since this feature was stable for years, we simply forgot to remove 'Experimental' tag. (<a href="https://issuetracker.unity3d.com/issues/android-split-apks-by-target-architecture-experimental-label-is-not-fully-displayed-at-android-player-settings">1364276</a>)</p></li>
<li><p>Android: Toggling Build App Bundle in the Build Player Window will now prompt for a save location rather than attempting to use the last build location which would have been the incorrect type of package. (<a href="https://issuetracker.unity3d.com/issues/android-building-app-using-ctrl-plus-b-shortcut-uses-the-last-used-configuration-instead-of-the-current-one">1329922</a>)</p></li>
<li><p>Animation: Animation Clip Preview Window's component stripping strips away all required components but the last batch. (1306349)</p></li>
<li><p>Animation: Animator.GetBoneTransform() is now working with disabled gameobject/animator. Exception are throw if avatar is null or not a humanoid. (<a href="https://issuetracker.unity3d.com/issues/animator-dot-getbonetransform-does-not-return-null-when-animator-is-disabled">1351090</a>)</p></li>
<li><p>Animation: Fixed an issue where large int would lose precision in the animation clip. (<a href="https://issuetracker.unity3d.com/issues/recorded-large-int-values-in-animationclip-are-not-preserved">1278866</a>)</p></li>
<li><p>Animation: Fixed an issue where the animation blend would not occur when interrupting an empty state transition. (<a href="https://issuetracker.unity3d.com/issues/animation-blend-does-not-occur-when-translating-from-any-state">1204145</a>)</p></li>
<li><p>Animation: Fixed Animation component not releasing shader property blocks when disabled. (<a href="https://issuetracker.unity3d.com/issues/material-changes-are-not-visible-in-the-game-slash-scene-view-when-the-animation-component-with-renderer-property-has-been-deleted">1293179</a>)</p></li>
<li><p>Animation: Fixed Animation window property selection from displaying duplicate Components when one Component type derives from another. (<a href="https://issuetracker.unity3d.com/issues/shadow-property-is-replaced-in-animation-window-property-selection-when-shadow-component-is-below-the-outline-in-the-inspector">1248925</a>)</p></li>
<li><p>Animation: Fixed error message spam "BlendTreeWorkspace is NULL" when saving the scene when an animation preview is active. (<a href="https://issuetracker.unity3d.com/issues/blendtreeworkspace-is-null-error-spam-while-a-blendtree-state-is-open-in-animator-window-after-saving-scene">1343833</a>)</p></li>
<li><p>Animation: Fixed GameObject flying when Root Motion is enabled and the Animation is using Motion Time parameter. Root motion will now be disabled when using Motion Time parameter. (<a href="https://issuetracker.unity3d.com/issues/animation-object-goes-flying-when-root-motion-is-enabled-and-the-animation-is-using-motion-time-parameter">1334739</a>)</p></li>
<li><p>Animation: Fixed HumanPoseHandler to no longer crash when calling the SetHumanPose function with a destroyed Root Transform. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-humanposehandler-dot-sethumanpose-is-called-after-its-animator-is-destroyed">1351876</a>)</p></li>
<li><p>Animation: Fixed keyframing of the "Active" property in constraint components. (<a href="https://issuetracker.unity3d.com/issues/warning-message-when-constraint-dot-active-is-added-as-property-in-the-animationclip">1317876</a>)</p></li>
<li><p>Animation: Fixed UndoPropertyModification currentValue returning null when changing Material's properties in the Inspector while keyframing. (<a href="https://issuetracker.unity3d.com/issues/undopropertymodification-currentvalue-returns-null-when-changing-materials-properties-in-the-inspector">1343018</a>)</p></li>
<li><p>Animation: GameObject is not animated when the Animator Component is enabled during Play Mode and Culling Mode is set to "Cull Completely". (<a href="https://issuetracker.unity3d.com/issues/gameobject-is-not-animated-when-the-animator-component-is-enabled-during-play-mode-and-culling-mode-is-set-to-cull-completely">1263490</a>)</p></li>
<li><p>Animation: StateMachine callbacks (OnStateEnter(), OnStateUpdate() and OnStateExit()) where called twice when a playable was bound to an animator with a state machine. They are now called only once, as expected. (<a href="https://issuetracker.unity3d.com/issues/onstateenter-and-onstateexit-are-called-multiple-times-when-using-timeline-with-control-track">1299849</a>)</p></li>
<li><p>Animation: The engine could crash when calling Rebind() on an animator. (1338736)</p></li>
<li><p>Animation: Updated sort method for animation clips in animation window using alphanum/natural sort. (<a href="https://issuetracker.unity3d.com/issues/animation-animation-clip-naming-does-not-follow-ascending-naming-convention">1261365</a>)</p></li>
<li><p>Animation: [Avatar] AvatarBuilder.BuildHumanAvatar sets NaN positions with some avatars. (<a href="https://issuetracker.unity3d.com/issues/avatarbuilder-dot-buildhumanavatar-sets-nan-positions-with-some-avatars">1200354</a>)</p></li>
<li><p>Apple TV: Fixed Game Center's dashboard opening instead of achievements screen when using UnityEngnine.Social.ShowAchievementsUI(). (1341949)</p></li>
<li><p>Asset Bundles: - Improved performance of AssetBundle.UnloadAsync.<br></p> 
<ul>
<li>Added new API to block on the main thread until an async AssetBundle unload completes.</li>
</ul></li>
<li><p>Asset Bundles: Fixed an edge case causing Asset Bundle hash version to change based on the order in which dependent bundles were assigned. (1307113)</p></li>
<li><p>Asset Bundles: Fixed an issue where moving an asset would not trigger an Asset Bundle rebuild. (<a href="https://issuetracker.unity3d.com/issues/assetbundle-does-not-update-when-only-the-path-of-the-file-is-modified">1346529</a>)</p></li>
<li><p>Asset Bundles: Fixed rare issue where AssetBundle.RecompressAssetBundleAsync would do a full recompress even if both the source and target AssetBundles are LZ4 compressed. (1293912)</p></li>
<li><p>Asset Import: Asset Pipeline: AssetDatabase.IsLoadingAssetPreview() is now correctly returning true when a preview is being generated. (<a href="https://issuetracker.unity3d.com/issues/assetpreview-dot-isloadingassetpreview-returns-false-when-a-preview-is-requested">1323729</a>)</p></li>
<li><p>Asset Import: AssetDatabase.SetImporterOverride now fails when used on folders and does not write to the .meta file. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-setimporteroverride-doesnt-fail-when-used-on-folders">1333997</a>)</p></li>
<li><p>Asset Import: BlendShape normals are recalculated when a meshes normals are set to 'calculate', and the blendshape normals are set to 'import'. (1363962)</p></li>
<li><p>Asset Import: BlendShapes value defaults to 0 when importing FBX model. (<a href="https://issuetracker.unity3d.com/issues/blendshapes-value-defaults-to-0-when-importing-fbx-model">1359606</a>)</p></li>
<li><p>Asset Import: Changing texture shape no longer causes NullReferenceExceptions. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-when-changing-texture-shape">1355120</a>)</p></li>
<li><p>Asset Import: Default Presets are applied correctly to ScriptableObjects created using the CreateAssetMenu. (<a href="https://issuetracker.unity3d.com/issues/preset-is-not-applied-to-scriptableobject-created-from-context-menu-when-using-a-glob-filter">1343776</a>)</p></li>
<li><p>Asset Import: Duplicates in overrideExts are now allowed and do not prevent the registration of other ScriptedImporters anymore. (<a href="https://issuetracker.unity3d.com/issues/other-scriptedimporters-in-the-project-are-not-registered-when-a-scriptedimporterattribute-contains-duplicates-in-overrideexts">1333985</a>)</p></li>
<li><p>Asset Import: Elides the file path shown on the asset importing dialogue on Windows. (<a href="https://issuetracker.unity3d.com/issues/longer-asset-names-get-cut-off-when-importing-assets">1298775</a>)</p></li>
<li><p>Asset Import: Fixed for Failing Importer Performance Tests on Linux. (1364226)</p></li>
<li><p>Asset Import: Fixed null ref exception when rebuilding inspectors due to a preset overwrite. (<a href="https://issuetracker.unity3d.com/issues/value-cannot-be-null-parameter-name-source-exception-is-thrown-when-overwriting-preset-file-while-inspector-is-empty">1375929</a>)</p></li>
<li><p>Asset Import: Fixed RenderToCubeMap artifacts when used with a Physical Camera. (<a href="https://issuetracker.unity3d.com/issues/using-rendertocubemap-using-a-camera-with-the-physicalparameter-produces-an-incorrect-cubemap">1370847</a>)</p></li>
<li><p>Asset Import: Fixed wrong settings being saved when trying to overwrite Preset. (<a href="https://issuetracker.unity3d.com/issues/input-manager-reverts-to-old-settings-when-trying-to-overwrite">1284602</a>)</p></li>
<li><p>Asset Import: GetAvailableImporters does not return AssetImporter types for native importers that don't have a matching C# Type. (<a href="https://issuetracker.unity3d.com/issues/getavailableimportertypes-returns-duplicates-assetimporter-types">1334266</a>)</p></li>
<li><p>Asset Import: Large SpeedTree imports. (1364523)</p></li>
<li><p>Asset Import: PanelSettingAssets is displayed with its UIToolkit CustomEditor as expected. (<a href="https://issuetracker.unity3d.com/issues/uitoolkit-scale-dynamic-and-clear-settings-dropdowns-are-missing-in-the-panel-settings-asset-preset">1330718</a>)</p></li>
<li><p>Asset Import: Reverted Save As list item to an actual button. (<a href="https://issuetracker.unity3d.com/issues/input-preset-save-current-to-button-in-input-manager-needs-to-be-double-clicked-to-activate">1376466</a>)</p></li>
<li><p>Asset Import: Scripted Importers can be registered to Native Importer extensions where the case is changed. (1360156)</p></li>
<li><p>Asset Import: SetImporterOverride now validates that the arguments are correct before performing the operation. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-setimporteroverride-does-not-set-a-specific-importer-when-asset-is-scriptableobject">1309105</a>)</p></li>
<li><p>Asset Import: Textures passed to AssetPostprocessor methods have no name.</p></li>
<li><p>Asset Pipeline: Added Editor Preference to make Bump Map check optional. (<a href="https://issuetracker.unity3d.com/issues/assetpostprocessors-loads-all-assets-of-the-same-type-into-memory-at-once">1345444</a>)</p></li>
<li><p>Asset Pipeline: AssetModificationProcessor.OnWillDeleteAsset is called when deleting an orphaned meta file. (<a href="https://issuetracker.unity3d.com/issues/second-same-created-asset-disappears-from-project-browser">1326312</a>)</p></li>
<li><p>Asset Pipeline: Blender and Maya files now import at the correct scale. (<a href="https://issuetracker.unity3d.com/issues/model-file-to-unity-scaling-is-defined-as-1m-file-to-100m-unity-when-importing-blend-file">1320649</a>)</p></li>
<li><p>Asset Pipeline: Call to AssetDatabase.ForceReserializeAssets() throws exception, if being called from callback, while scene is also being modified. It is recommended to call AssetDatabase.ForceReserializeAssets() from menu item style entry point. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-forcereserializeassets-breaks-the-scene-when-used-in-onenable">1089842</a>)</p></li>
<li><p>Asset Pipeline: Calling CreateAsset twice on the same location with the same asset didn't update ProjectBrowser. (<a href="https://issuetracker.unity3d.com/issues/asset-gets-treated-as-a-root-folder-after-creating-a-sprite-asset-from-the-same-texture-multiple-times">1345123</a>)</p></li>
<li><p>Asset Pipeline: Calling CreateAsset with a path that is an existing folder now generates an error. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-createasset-overwites-folder-without-a-warning">1344954</a>)</p></li>
<li><p>Asset Pipeline: Fixed a bug where subsequent builds or manually-selected script only builds could result in incorrect code stripping.</p></li>
<li><p>Asset Pipeline: Fixed an infinite import loop that could occur on case-sensitive file systems if similarly named meta files were encountered. (<a href="https://issuetracker.unity3d.com/issues/editor-is-stuck-on-loading-scripting-assemblies-when-there-is-a-meta-file-of-non-existent-asset-and-asset-database-v2-is-used">1345905</a>)</p></li>
<li><p>Asset Pipeline: Fixed an issue where Importer/Rig Update button does not update. (<a href="https://issuetracker.unity3d.com/issues/importer-slash-rig-update-button-does-not-update">1324031</a>)</p></li>
<li><p>Asset Pipeline: Fixed an issue where it was possible invalid and unusable Presets without any errors. The Preset constructor now throws an exception when doing so. (<a href="https://issuetracker.unity3d.com/issues/creating-a-preset-of-an-asset-type-marked-as-excluded-from-presets-is-allowed-but-the-generated-preset-is-not-usable">1348271</a>)</p></li>
<li><p>Asset Pipeline: Fixed an issue where Model Importer Rig Tab Update button doesn't work properly with multi-selection. (1330281)</p></li>
<li><p>Asset Pipeline: Fixed an issue where NullReferenceException is thrown when assigning a duplicated Avatar to an Animation Source. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-assigning-a-duplicated-avatar-to-an-animation-source">1274098</a>)</p></li>
<li><p>Asset Pipeline: Fixed an issue where the Model Importer Rig Tab's Avatar Source doesn't refresh. (1330278)</p></li>
<li><p>Asset Pipeline: Fixed an issue where Unity could crash when attempting to repair a scene containing multiple components with missing GameObjects while opening it. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-gameobject-activateawakerecursivelyinternal-when-opening-a-specific-scene">1347557</a>)</p></li>
<li><p>Asset Pipeline: Fixed an issue where user fields in assets containing 'guid' could cause incorrect asset dependencies to be shown. (<a href="https://issuetracker.unity3d.com/issues/select-dependencies-of-an-asset-is-missing-1-texture-2d-dependency-of-the-total-when-guid-string-is-longer-than-8-characters">1363953</a>)</p></li>
<li><p>Asset Pipeline: Fixed crash when opening project with asset that a broken reference to mono script. (<a href="https://issuetracker.unity3d.com/issues/crash-on-pthread-kill-when-opening-a-project-with-a-broken-prefab">1351825</a>)</p></li>
<li><p>Asset Pipeline: Fixed exception inside Import Activity Window that would happen when inspecting asset's that were reimported after switching RenderPipeline. (1377678)</p></li>
<li><p>Asset Pipeline: Fixed race condition triggering an assert when downloading from cache server and not refreshing.</p></li>
<li><p>Asset Pipeline: Improved quality of imported JPEG textures. (<a href="https://issuetracker.unity3d.com/issues/a-jpeg-image-has-artifacts-that-do-not-appear-when-loading-the-texture-with-texture2d-dot-loadimage">1345890</a>)</p></li>
<li><p>Asset Pipeline: Ported runtime test to playmode, to workaround an instability in the runtime test runner that was affecting it. (1403932)</p></li>
<li><p>Asset Pipeline: Reloading Arrays are kept in Sync. (1327830)</p></li>
<li><p>Asset Pipeline: Tags can now be deleted from the TagManager Presets. (<a href="https://issuetracker.unity3d.com/issues/preset-unable-to-delete-a-tag-from-tagmanager-preset-asset">1317709</a>)</p></li>
<li><p>Audio: Fixed calculation of channel audibility such that a signal which is branched off via send/receive effects in a mixer group and fully attenuated after the branching correctly retain the audibility contributed by the send-receive connection. (<a href="https://issuetracker.unity3d.com/issues/audio-mixer-with-sends-and-receives-reports-0-audibilty-to-profiler">1309971</a>)</p></li>
<li><p>Audio: Fixed performance impact on SaveAndReimport when AudioMixer window is shown. (<a href="https://issuetracker.unity3d.com/issues/saveandreimport-performance-on-textureimporter-impacted-when-audiomixer-window-is-shown">1327645</a>)</p></li>
<li><p>Audio: Fixed rare access violation crash in audio update of main thread. (1352816)</p></li>
<li><p>Audio: For complex send-receive configurations branching the signals between two mixer groups an order-dependent buffering delay was introduced that caused flange-like effects. The correct evaluation order of all effects is now enforced to prevent this. (<a href="https://issuetracker.unity3d.com/issues/audio-gets-distorted-after-reordering-the-audio-groups-inside-an-audio-mixer">1309970</a>)</p></li>
<li><p>Build Pipeline: Errors from catastrophically failing incremental build pipeline steps are now clearer.</p></li>
<li><p>Build Pipeline: Fixed a bug where data builds would unnecessarily rerun in incremental player builds if the project contained editor resources.</p></li>
<li><p>Build Pipeline: Fixed a bug where UnityLinker would unnecessarily rerun without changes in incremental player builds.</p></li>
<li><p>Build Pipeline: Fixed a potential file name issue on windows in incremental player builds.</p></li>
<li><p>Build Pipeline: Fixed a regression that Unity will now properly detect a Visual Studio Build Tools installation.</p></li>
<li><p>Build Pipeline: Fixed an issue where some projects wouldn't build if they were located on a drive different from the Editor.</p></li>
<li><p>Build Pipeline: iOS and tvOS now use the new incremental build pipeline.</p></li>
<li><p>Build Pipeline: Removing the Lumin (Magic Leap 1) platform from being added as part of the installer for Windows and Mac.</p></li>
<li><p>Build Pipeline: The build subtarget is now adjusted to kStandaloneBuildSubtargetServer when BuildPipeline.BuildPlayer is called with the deprecated option BuildOptions.EnableHeadlessMode set to true so the scripted build pipeline remains backward compatible until the option is effectively removed. (<a href="https://issuetracker.unity3d.com/issues/deprecated-buildoptions-dot-enableheadlessmode-needs-clearer-warning-for-its-conflicts-with-buildoptions-dot-subtarget-field">1354146</a>)</p></li>
<li><p>Build System: Fixed error "Cannot find mono image in MonoManager for assembly x" during assembly reload when calling <code>ContentBuildInterface:GetPlayerObjectIdentifiersInAsset</code>.</p></li>
<li><p>Burst: Arrows were rendered even though they were not within the current view.</p></li>
<li><p>Burst: Burst will now handle projects special characters in their project-name.</p></li>
<li><p>Burst: Crash in burst module initialization if multiple modules are compiled and then linked in a different order.</p></li>
<li><p>Burst: Detects if the simulator is the target of a player build for iOS/tvOS and disables burst, as at present this configuration is not supported by burst.</p></li>
<li><p>Burst: Error if install in build folder is used without ever using a regular build.</p></li>
<li><p>Burst: Fixed "UnityException: CompileAsyncDelegateMethod can only be called from the main thread." error that was logged in standalone players when the first invocation of a direct-call method was from a background thread.</p></li>
<li><p>Burst: Fixed a bug in 2022.1+ where calling <code>Debug.Log</code> in a static constructor would result in a Burst failure.</p></li>
<li><p>Burst: Fixed a bug in the entry-point finding code whereby we wouldn't correctly resolve a nested generic struct's job if it was within a concrete generic class that was outwith the root assembly set.</p></li>
<li><p>Burst: Fixed a bug in the fixed string processing whereby we'd miscompile a fixed string that was within a struct inside a <code>SharedStatic</code> (depending on how it was used).</p></li>
<li><p>Burst: Fixed a bug that could prevent Visual Studio locating .pdb files while debugging.</p></li>
<li><p>Burst: Fixed a bug that meant Burst was accidentally enabled in secondary Unity processes, including the asset import worker and out-of-process profiler (see changelog entry for 1.6.0-pre.1 for more context around this).</p></li>
<li><p>Burst: Fixed a bug that was exposed by a Script Updater running against the Entities tests, whereby if some sort of pre-domain-reload code (some sort of teardown like thing) called into Burst, the script updater could have caused Burst to purge valid function pointers, resulting in us trying to execute a DLL location that we had already unloaded.</p></li>
<li><p>Burst: Fixed a bug where a player build that had multiple assemblies that had structs declared with the same name and same contents but different <code>[BurstCompile]</code> methods in them, would wrongly only pick a single struct to Burst-compile.</p></li>
<li><p>Burst: Fixed a bug where codegen differences could occur when using a local vector variable that was being captured by reference and passed to a called function, versus when it wasn't.</p></li>
<li><p>Burst: Fixed a bug where if you had a long running compilation and a new compilation came in, some threads in the thread pool could (if unlucky) block trying to dirty the assembly in our Burst caching infrastructure while waiting for the compilation to complete.</p></li>
<li><p>Burst: Fixed a bug where our <code>[BurstCompile]</code> job finding code would not find methods in generic base classes in places where we knew the concrete-generic type (for instance <code>struct Foo { [BurstCompile] struct MyJob : IJob { void Execute() {} } }</code>, <code>struct Bar : Foo {}</code>, and <code>struct Haz : Bar {}</code> - we wouldn't find the concrete <code>Foo::MyJob</code> in Burst).</p></li>
<li><p>Burst: Fixed a bug where the compiler would reject a <code>try</code>/<code>finally</code> statement if it was the first thing in a method.</p></li>
<li><p>Burst: Fixed a bug where we could leave background tasks around forever when we had actually completed them (could only happen if two re-compilation requests arrived close together, meaning we'd cancel the first but never report to the background tasks that we had cancelled them!).</p></li>
<li><p>Burst: Fixed a bug where <code>fixed</code> used in conjunction with <code>Span</code> or <code>ReadOnlySpan</code> would cause a compiler error.</p></li>
<li><p>Burst: Fixed a bug whereby complicated <code>try</code>/<code>finally</code> nesting could trip up the compiler.</p></li>
<li><p>Burst: Fixed a bug whereby sometimes some LLVM intrinsics could be incorrectly marked as unused causing invalid codegen with calls to <code>math.acos</code>.</p></li>
<li><p>Burst: Fixed a bug with <code>sqrt_ps</code> for 128-bit types where it would crash the compiler.</p></li>
<li><p>Burst: Fixed a codegen issue with Unity 2021.2 and <code>System.Buffer.MemoryCopy</code>.</p></li>
<li><p>Burst: Fixed a compiler miscompile if you loaded a <code>static readonly v128</code> and passed it straight to a function as an argument.</p></li>
<li><p>Burst: Fixed a crash that could occur when loading legacy Burst AOT settings and then entering play mode.</p></li>
<li><p>Burst: Fixed a performance regression affecting some vectorization in Burst 1.7+ (LLVM 12+).</p></li>
<li><p>Burst: Fixed a performance regression with <code>IJobParallelFor</code> where vectorization didn't happen for cases where it previously would have.</p></li>
<li><p>Burst: Fixed a really subtle caching bug in the compiler where if you had a job that compiled successfully at least once, then it failed (you used managed state for instance), then you closed the editor and restarted, if the compiler threads started in precisely a strange combination then Burst might accidentally never recompile the job which failed previously.</p></li>
<li><p>Burst: Fixed a super rare bug whereby if you kicked off two compilations very close together (most likely when running Unity in some sort of headless build-a-player mode), Burst could throw an exception on a burst hash cache file being locked by the process.</p></li>
<li><p>Burst: Fixed a Unity 2021.2 and newer bug that manifested with UWP builds - we were using the wrong <code>unityaot</code> folder in the Unity editor distribution with Burst.</p></li>
<li><p>Burst: Fixed access violation error that could occur when reading from a static readonly variable.</p></li>
<li><p>Burst: Fixed an exception that could occur if you had the Burst AOT Settings menu docked in the Editor, and then did a player build. Trying to change any of the Burst AOT Settings would throw an exception (unless you closed and reopened the Burst AOT Settings).</p></li>
<li><p>Burst: Fixed an internal compiler error when casting a void* to a pointer-to-vector and then access the element.</p></li>
<li><p>Burst: Fixed an issue where Debug.LogError logs from Bursted code would be treated as compiler errors. (1354070)</p></li>
<li><p>Burst: Fixed an issue where dsym folders would be not be copied across to the DoNotShip folder when building a multi architecture build for mac os.</p></li>
<li><p>Burst: Fixed an issue where with optimizations disabled, using half conversions on platforms that did not natively support half could cause linker errors.</p></li>
<li><p>Burst: Fixed bug that could lead to "Failed to resolve method with name hash X and signature hash Y" compiler error.</p></li>
<li><p>Burst: Fixed bug that could lead to incorrect compiler errors for calls to <code>GetHashCode</code> from a generic type.</p></li>
<li><p>Burst: Fixed compiler crash when trying to load a generic static field.</p></li>
<li><p>Burst: Fixed compiler error that occurred when calling <code>BurstCompiler.CompileFunctionPointer</code> with a delegate type that was decorated with a custom attribute.</p></li>
<li><p>Burst: Fixed constant folding when using <code>Hint.Likely</code> or <code>Hint.Unlikely</code> intrinsics - the compiler is now able to fold these calls away entirely if the input value is constant.</p></li>
<li><p>Burst: Fixed editor crash when trying to debug a DirectCalled method.</p></li>
<li><p>Burst: Fixed error when trying to Direct Call a method belonging to a private nested type.</p></li>
<li><p>Burst: Fixed for the <code>X.pdb: The process cannot access the file because it is being used by another process</code> issue our users were seeing. We were taking a <code>FileShare.Read</code> lock, when we needed to take <code>FileShare.ReadWrite</code>.</p></li>
<li><p>Burst: Fixed issue that could cause bcl.exe to fail with an exit code of 1 but not output any compilation errors.</p></li>
<li><p>Burst: Fixed our platform documentation to accurately reflect the current supported platforms with Burst.</p></li>
<li><p>Burst: Fixed potential hang in Editor when compiling a Burst entry point method that is defined in a generic class.</p></li>
<li><p>Burst: Fixed some memory leaks between the C# and C++ parts of the Burst compiler, and added some CI tooling to ensure this doesn't happen again.</p></li>
<li><p>Burst: Fixed that implicitly casting a scalar half to a vector type would cause the compiler to crash.</p></li>
<li><p>Burst: Fixed the "could not find path tempburstlibs" error message popping up when building for Android and Burst is disabled.</p></li>
<li><p>Burst: Fixed the Burst <code>link.xml</code> output to preserve C# methods we rely on, alongside the static constructors that we preserved previously.</p></li>
<li><p>Burst: Fixed the documentation to note that the <code>System.Runtime.CompilerServices</code> attributes <code>[CallerLineNumber]</code>, <code>[CallerMemberName]</code>, and <code>[CallerFilePath]</code> work with Burst, with the restriction that you cannot format the <code>[CallerMemberName]</code>, and <code>[CallerFilePath]</code> strings yet.</p></li>
<li><p>Burst: Fixed the very rare bug whereby the Burst Hash Cache files (*.bhc) will sometimes cause an exception in the editor log.</p></li>
<li><p>Burst: Fixed the [bug @tertle found](https://forum.unity.com/threads/burst-error-bc0102-unexpected-internal-compiler-error.1173977/) when loading a vector from a struct pointer that is marked as <code>in</code>.</p></li>
<li><p>Burst: Fixed type initialization error, and invalid log messages about needing to add <code>[MonoPInvokeCallback]</code> to be compatible with IL2CPP, that could occur in a player build with Burst disabled.</p></li>
<li><p>Burst: ILPP issue for dots runtime whereby a calli patch could generate bad IL if the first instruction replaced was the target of a branch.</p></li>
<li><p>Burst: Improved UWP linker error message to clarify which VS components need to be installed for UWP.</p></li>
<li><p>Burst: Incorrect conversions between signed and unsigned vector types.</p></li>
<li><p>Burst: Inspector menu buttons were seen as available, even though they were not supported, when viewing i.e. .NET IL code.</p></li>
<li><p>Burst: Keybindings for copy and selection did not depend on OS. Now has proper "select all" and "copy" shortcuts for MacOS.</p></li>
<li><p>Burst: Linker errors on macOS due to long command lines, swapped to using filelists for inputs.</p></li>
<li><p>Burst: Linking would fail on non-Windows platforms if the project folder contained a single-quote.</p></li>
<li><p>Burst: Made it save the actual line numbers for code blocks in <code>_blockLine</code> even when the block is below the view.</p></li>
<li><p>Burst: Made <code>--burst-force-sync-compilation</code> command-line option actually work.</p></li>
<li><p>Burst: Missing output messages from some tools when a failure occurred.</p></li>
<li><p>Burst: One Definition Rule optimisation would break if multiple modules shared static constructors due to an issue with sharing code but not data.</p></li>
<li><p>Burst: Performance regression.</p></li>
<li><p>Burst: Removed the starting newline character when copying, and when rendering plain assembly kind.</p></li>
<li><p>Burst: Stack overflow caused by placement of alloca under certain function transforms.</p></li>
<li><p>Burst: Static constructor cyclic checks also included method calls when this is not necessary and fails on burst runtime logging code.</p></li>
<li><p>Burst: Static constructor sorting didn't account for dependencies within calls' IL.</p></li>
<li><p>Burst: The cache for pdbs was becoming stale. This caused issues with wrong source information being shown in the inspector, and potentially wrong debug information being generated for bursted code in editor sessions.</p></li>
<li><p>Burst: <code>ArgumentOutOfRangeException</code> due to <code>_renderBlockStart</code> and <code>_renderBlockEnd</code> not being probably initialized when all blocks were above the scroll position.</p></li>
<li><p>Burst: <code>[SkipLocalsInit]</code> now correctly doesn't zero-initialize variables in a function (previously it only avoided zero-initialization of <code>stackalloc</code> created variables).</p></li>
<li><p>Core: Corrected disposed NativeArray and NativeSlice instance behaviour when accessing the Length property. An exception is now thrown instead of returning 0. An exception is also thrown when accessing the NativeArray indexer or attempting to iterate over disposed instances.</p></li>
<li><p>Core: Fixed bug where shadows disappear in the frustum corners from false positives in the shadow culling.</p></li>
<li><p>Core: Fixed bug with shadow fade where the shadows will be culled with a hard line across the fade and also stretches the fade beyond the projected shadow.</p></li>
<li><p>Core: Unity.Collections.LowLevel.Unsafe::AtomicSafetyHandle method CheckExistsAndThrow throws exception ObjectDisposedException instead of InvalidOperationException.</p></li>
<li><p>Core: Updated NativeArray and NativeSlice Enumerator MoveNext functions with a define conditional<br> atomic safety handle boolean check to ensure that existing enumerators return false<br>
when MoveNext() is called instead of throwing an exception.</p></li>
<li><p>Core: When ENABLE_UNITY_COLLECTIONS_CHECKS is defined some additional AtomicSafetyHandle struct validation methods are available.</p></li>
<li><p>Documentation: Fixed incorrect measurement units for ArticulationDrive.forceLimit.</p></li>
<li><p>DX12: Fixed crash copying block compressed textures. (<a href="https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-building-project-for-dx12">1360034</a>)</p></li>
<li><p>DX12: Fixed crash on present in Editor.</p></li>
<li><p>Editor: (Dynamic Hints) Fixed: NullReferenceException when a prefab with a missing script is hovered in the ProjectBrowser.</p></li>
<li><p>Editor: Added a new filter in project browser for VFX Asset files. (1382786)</p></li>
<li><p>Editor: Added additional diacritics support to the Linux Editor for multi-key characters. (<a href="https://issuetracker.unity3d.com/issues/linux-characters-with-diacritics-can-not-be-entered-when-2-keys-are-required-to-enter-the-character">1344560</a>)</p></li>
<li><p>Editor: Added BOM SJSON parsing support. (1373091)</p></li>
<li><p>Editor: Added pen delta calculation for the new input system. (<a href="https://issuetracker.unity3d.com/issues/pen-delta-is-always-0-0">1168556</a>)</p></li>
<li><p>Editor: Added progress scopes for shader compilation and scene opening. (1331846)</p></li>
<li><p>Editor: Advanced Drop-down now calculates the initially needed size correctly, avoiding scrollbars if the size fits into view or the defined max size of the window. (<a href="https://issuetracker.unity3d.com/issues/advanced-dropdown-is-2-3-lines-too-short-for-no-reason-requiring-scrolling">1335631</a>)</p></li>
<li><p>Editor: Android window dimension PlayerSettings visibility is now controlled by the Full Screen Mode rather than resizability of the window. (<a href="https://issuetracker.unity3d.com/issues/secondary-windows-opening-in-fullscreen">1386717</a>)</p></li>
<li><p>Editor: Copy Path property' in transform inspector now returns the correct property when constrain proportions are disabled. (1365045)</p></li>
<li><p>Editor: Do not show Beta users thank you link if the build is not final. (<a href="https://issuetracker.unity3d.com/issues/broken-slash-not-available-to-public-forum-site-is-opened-when-special-thanks-to-our-beta-users-button-is-pressed">1363606</a>)</p></li>
<li><p>Editor: Ensure current Settings Provider gets Activated if NotifySettingsProvider change is called. (<a href="https://issuetracker.unity3d.com/issues/hdrp-nullreferenceexception-in-unityeditor-dot-preferencesprovider-dot-writerecentappslist-after-clicking-clean-gi-cache-button">1343598</a>)</p></li>
<li><p>Editor: Ensure no SearchReportWindow are created when using old OverlayPresets.asset. (1368837)</p></li>
<li><p>Editor: Ensure RootEditor does not prevent from dropping in scene view. (<a href="https://issuetracker.unity3d.com/issues/rooteditor-predicate-for-gameobjects-disables-drag-and-drop-in-the-scene-view">1373165</a>)</p></li>
<li><p>Editor: Ensured compact mode works fine with Asset store provider. (<a href="https://issuetracker.unity3d.com/issues/package-publisher-name-is-displayed-instead-of-package-name-when-using-the-smallest-view-mode-in-the-search-window">1357617</a>)</p></li>
<li><p>Editor: Ensured that when creating a new scene through the scene template mechanism the EditorSceneManager.newScene event has the proper arguments and all the defaults objects are properly created according to the type of builtin template. (<a href="https://issuetracker.unity3d.com/issues/wrong-newscenemode-is-passed-to-editorscenemanager-dot-newscenecreated-and-default-objects-cannot-be-found-when-creating-a-scene">1347256</a>)</p></li>
<li><p>Editor: Ensured the tips section doesn't wordwrap as this cause resizing problem at scaling 125%. (1345630)</p></li>
<li><p>Editor: Enums in the inspector can now be sorted in alphabetical order by using [InspectorOrder] attribute.</p></li>
<li><p>Editor: Fixed a bug regarding repeat command for integration tests (DSTP-562).</p></li>
<li><p>Editor: Fixed a bug which prevented the access token to be refreshed after it expired. This issue required the user to close and reopen the editor every time the access token expired to get it refreshed.</p></li>
<li><p>Editor: Fixed a crash when cancelling a project loading in certain cases. (<a href="https://issuetracker.unity3d.com/issues/macos-editor-crashes-after-closing-the-splash-screen">1380096</a>)</p></li>
<li><p>Editor: Fixed a regression in Shader Graph tool that prevented keyboard interaction and navigation with the search results until the list is explicitly clicked/focused on. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-cant-navigate-the-node-creation-menu-with-keyboard-while-search-is-focused">1396759</a>)</p></li>
<li><p>Editor: Fixed Advanced Dropdown (Add Component Menu) to allow mouse interactions in the search text field. (1352677)</p></li>
<li><p>Editor: Fixed an issue causing C# serializable generic types to incorrectly contain data for editor only fields in serialized data when in a player context.</p></li>
<li><p>Editor: Fixed an issue to set correct EnumFlagsFields for sbyte, byte, short and ushort. (<a href="https://issuetracker.unity3d.com/issues/none-or-mixed-option-gets-set-to-enumflagsfield-when-selecting-the-everything-option">1337072</a>)</p></li>
<li><p>Editor: Fixed an issue where console errors are thrown when terrain inspector is shrunk. (1305724)</p></li>
<li><p>Editor: Fixed an issue where the cursor would flicker between different cursors near resize panes. (<a href="https://issuetracker.unity3d.com/issues/mouse-cursor-flickering-when-hovering-over-editor-window-edges-on-windows-platform">1333668</a>)</p></li>
<li><p>Editor: Fixed an occasional exception when reordering expanded elements.</p></li>
<li><p>Editor: Fixed ArgumentOutOfRangeException when interacting with Scene Hierarchy window after exiting playmode. (<a href="https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-right-clicking-certain-hierarchy-window-items-during-play-mode-exit-process">1351981</a>)</p></li>
<li><p>Editor: Fixed assert throwing when instantiating a new scene from a modal window. (<a href="https://issuetracker.unity3d.com/issues/scene-management-creating-a-scene-from-a-template-fails-when-no-scene-dependencies-are-toggled-on-and-called-from-modal-window">1355520</a>)</p></li>
<li><p>Editor: Fixed build and run menu and its shortcut still working when build and run is disabled by Editor extension. (<a href="https://issuetracker.unity3d.com/issues/cannot-build-and-run-the-player-when-a-save-prompt-is-shown-and-architecture-is-set-to-apple-silicon">1345699</a>)</p></li>
<li><p>Editor: Fixed can't resize the Inspector window when a script is attached to a GameObject and Sirenix Odin Inspector plugin is installed. (<a href="https://issuetracker.unity3d.com/issues/cannot-resize-the-inspector-window-when-a-script-component-is-attached-to-a-gameobject">1359807</a>)</p></li>
<li><p>Editor: Fixed Console Window log hyperlinks cursor hovering.</p></li>
<li><p>Editor: Fixed crash when entering Play Mode if a ScriptableObject Resource is loaded and unloaded while being displayed in the Inspector. (<a href="https://issuetracker.unity3d.com/issues/crash-when-entering-play-mode-if-a-scriptableobject-resource-is-loaded-and-unloaded-while-being-displayed-in-the-inspector">1359247</a>)</p></li>
<li><p>Editor: Fixed drag and drop of render texture with incorrect dimesion on light cookie field. (1376464)</p></li>
<li><p>Editor: Fixed editor crash when accessing properties on canvas in some cases. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-propertyinfo-dot-getvalue-is-called-for-properties-from-component-dot-gettype-dot-getproperties">1340354</a>)</p></li>
<li><p>Editor: Fixed editor crash while processing static batching meshes during enter playmode. (1370676)</p></li>
<li><p>Editor: Fixed editor crashes when exiting and keeping a tutorial project.</p></li>
<li><p>Editor: Fixed editor freezes for a moment when moved from one screen to another with different resolution scale. (<a href="https://issuetracker.unity3d.com/issues/editor-is-repainted-and-freezes-for-a-moment-when-moved-from-one-screen-to-another-with-different-resolution-scale">1322959</a>)</p></li>
<li><p>Editor: Fixed editor window leak on window close. (1372919)</p></li>
<li><p>Editor: Fixed elements overlap one another in the Inspector window when using MinAttributes and resizing the Inspector window. (<a href="https://issuetracker.unity3d.com/issues/elements-overlap-one-another-in-the-inspector-window-when-using-minattributes-and-resizing-the-inspector-window">1363190</a>)</p></li>
<li><p>Editor: Fixed empty reason on passed tests results xml (DSTR-63).</p></li>
<li><p>Editor: Fixed EnumMaskField showing "Mixed.." when the value was non-zero but none of the actual flags were set.</p></li>
<li><p>Editor: Fixed EnumMaskField showing the label "Mixed.." when all flags were set but the mask value was not set to the everything value. This will now also handle cases where obsolete enum values were present in the enum but not set or displayed.</p></li>
<li><p>Editor: Fixed error messages overflowing on new versions of macOS. (1312314)</p></li>
<li><p>Editor: Fixed errors being thrown from the RenderTexture editor after selecting the Tex2DArray dimension. (<a href="https://issuetracker.unity3d.com/issues/creating-another-render-texture-causes-assigning-3d-texture-to-2darray-texture-property-maintex-dimensions-must-match">1287189</a>)</p></li>
<li><p>Editor: Fixed exceptions when assigning array size via array size field in ReorderableList inspector control.</p></li>
<li><p>Editor: Fixed floating window behavior for mac editor fullscreen so that windows remain on the desktop when the editor enters or exits fullscreen on a second monitor. (<a href="https://issuetracker.unity3d.com/issues/unity-editor-windows-switch-macos-spaces-when-maximizing-the-unity-editor-or-exiting-full-screen-mode">1321315</a>)</p></li>
<li><p>Editor: Fixed for Scroll bars scrolling up and down when holding down the left mouse button on the left edge of the scroll bar area. (<a href="https://issuetracker.unity3d.com/issues/scroll-bars-keeps-scrolling-up-and-down-when-holding-down-the-left-mouse-button-on-the-left-edge-of-the-scroll-bar-area">1347294</a>)</p></li>
<li><p>Editor: Fixed GameObjectChangeTracker initialization issue causing it to trigger assertion failure errors. (1376716)</p></li>
<li><p>Editor: Fixed glitching when resizing editor windows with a popup open in the Windows editor. (<a href="https://issuetracker.unity3d.com/issues/scene-slash-game-view-glitching-out-when-resizing-their-windows-and-rect-transform-anchors-presets-window-is-open">1333410</a>)</p></li>
<li><p>Editor: Fixed gradient picker was forced to always use gamma colorspace (ignoring provided parameter). (1383095)</p></li>
<li><p>Editor: Fixed GUIClip errors are shown after deleting all objects from multiple loaded Scenes in the Hierarchy. (<a href="https://issuetracker.unity3d.com/issues/guiclip-errors-are-shown-after-deleting-all-objects-from-multiple-loaded-scenes">1363623</a>)</p></li>
<li><p>Editor: Fixed handling of special hotkey characters in the Open Recent Scene sub-menu. (<a href="https://issuetracker.unity3d.com/issues/scene-cant-be-enabled-because-it-doesnt-exist-error-appears-when-deleting-a-scene-in-a-and-opening-package-manager">1364651</a>)</p></li>
<li><p>Editor: Fixed incorrect OnApplicationPause pauseStatus after losing focus on macOS. (<a href="https://issuetracker.unity3d.com/issues/onapplicationpause-pausestatus-is-incorrect-after-losing-focus-on-macos">1344918</a>)</p></li>
<li><p>Editor: Fixed incorrect primitive counts for meshes with multiple sub meshes in the LOD Inspector. (<a href="https://issuetracker.unity3d.com/issues/editor-lod-group-triangle-count-is-inaccurate-for-sub-meshes">1349756</a>)</p></li>
<li><p>Editor: Fixed issue when <code>.</code> suffix was applied to BuildTargets without extension.</p></li>
<li><p>Editor: Fixed issue where Console Log is selected but no info is shown when selecting a log, entering and exiting Play Mode. (<a href="https://issuetracker.unity3d.com/issues/console-log-is-selected-but-no-info-is-shown-when-selecting-a-log-entering-and-exiting-play-mode">1341773</a>)</p></li>
<li><p>Editor: Fixed Linux Editor not reporting scroll values with new input system. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-ignores-mouse-scroll-wheel-input-when-the-cursor-is-locked-on-the-new-input-system">1354498</a>)</p></li>
<li><p>Editor: Fixed Mac Editor crash that happened in multi-scene builds that were using BuildOptions.DetailedBuildReport.</p></li>
<li><p>Editor: Fixed missing labels for properties. (<a href="https://issuetracker.unity3d.com/issues/missing-labels-in-naninovel-project-settings">1332116</a>)</p></li>
<li><p>Editor: Fixed modal progress window stuck on top of other applications on macOS. (<a href="https://issuetracker.unity3d.com/issues/unity-compiling-c-number-scripts-dialog-pops-over-all-dialogs-from-all-apps-on-osx">1358626</a>)</p></li>
<li><p>Editor: Fixed mouse move events not properly being received by the game view when not in maximize mode. (1381985)</p></li>
<li><p>Editor: Fixed OpenGL context error messages when entering or exiting play mode. (1338849)</p></li>
<li><p>Editor: Fixed possible crash when remapping assets during template instantiation. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-editorutility-remapassetreferences-when-creating-a-new-scene-from-an-hdrp-template">1387380</a>)</p></li>
<li><p>Editor: Fixed Project Browser ping effect is misaligned in grid view. (1367601)</p></li>
<li><p>Editor: Fixed Render Settings being lost when instantiating a template with no cloneable dependencies. (<a href="https://issuetracker.unity3d.com/issues/creating-a-new-scene-from-custom-template-scene-opens-a-new-scene-when-no-file-is-cloned">1371682</a>)</p></li>
<li><p>Editor: Fixed ReorderableList custom element height callback exception when there are no elements in the list. (<a href="https://issuetracker.unity3d.com/issues/reorderablelist-out-of-bounds-exeception">1399803</a>)</p></li>
<li><p>Editor: Fixed ReorderableList first element height when the element uses PropertyDrawer. (<a href="https://issuetracker.unity3d.com/issues/first-array-element-expansion-is-broken-for-arrays-that-use-custom-property-drawers">1409773</a>)</p></li>
<li><p>Editor: Fixed Repeat and Retry attribute for UnityTest in PlayMode (DSTR-237).</p></li>
<li><p>Editor: Fixed repeat functionality for native test runner(DSTP-668).</p></li>
<li><p>Editor: Fixed scene template instantiate when no cloneable dependency. (<a href="https://issuetracker.unity3d.com/issues/scene-template-instantiating-a-new-scene-from-template-with-no-dependencies-checked-does-not-create-the-new-scene-asset">1354371</a>)</p></li>
<li><p>Editor: Fixed selection shift selection in the Scene Hierarchy. (<a href="https://issuetracker.unity3d.com/issues/wrong-elements-are-selected-when-holding-shift-and-selecting-game-objects-in-the-scene-hierarchy-1">1368196</a>)</p></li>
<li><p>Editor: Fixed so that dialogs displayed with EditorUtility.DisplayDialog open in front of other windows in the macOS Editor. (1350447)</p></li>
<li><p>Editor: Fixed spelling mistake.</p></li>
<li><p>Editor: Fixed the issue when an older user layout was loaded in the Editor and resulted in InvalidCastException. (<a href="https://issuetracker.unity3d.com/issues/invalidcastexception-is-thrown-with-specific-layout-when-selecting-anything-in-the-services-tab">1347313</a>)</p></li>
<li><p>Editor: Fixed the platform string. A proper platform string is now returned for server platforms (windows, linux and OSX). (1360107)</p></li>
<li><p>Editor: Fixed the validation of the Application Identifier.</p></li>
<li><p>Editor: Fixed tooltips staying open in the macOS editor when space changes or a window is minimized. Also fixes "ghost" tooltips in dual monitor set-up with multiple spaces. (<a href="https://issuetracker.unity3d.com/issues/probuilder-window-tooltips-show-up-when-the-window-is-minimized-using-macos-spaces">1295787</a>)</p></li>
<li><p>Editor: Fixed touchcount not resetting when exit playmode with a finger down. (<a href="https://issuetracker.unity3d.com/issues/input-touchcount-doesnt-reset">1258785</a>)</p></li>
<li><p>Editor: Fixed Transform Component update with HideFlags.DontSave objects. (<a href="https://issuetracker.unity3d.com/issues/transform-component-of-the-object-is-not-being-updated-properly-when-it-is-marked-as-hideflags-dot-dontsave">1091293</a>)</p></li>
<li><p>Editor: Fixed unicode input in Windows Editor modal windows so that non-Latin characters can be entered. (<a href="https://issuetracker.unity3d.com/issues/non-latin-characters-are-displayed-incorrectly-when-entering-them-in-the-text-field-of-the-modal-editor-window">1297206</a>)</p></li>
<li><p>Editor: Fixed Unity Package Manager diagnostic tool failing to run when started via the launch script.</p></li>
<li><p>Editor: Inspector correctly refreshes after adding the CanEditMultipleObjects attibute to an inspector. (<a href="https://issuetracker.unity3d.com/issues/inspector-does-not-allow-multi-object-editing-after-adding-a-caneditmultipleobjects-attribute-and-re-compiling-the-code">1348788</a>)</p></li>
<li><p>Editor: Inspector does not show prefab overrides anymore if the prefab asset is missing. (1369171)</p></li>
<li><p>Editor: Installing Linux mono and IL2CPP support on mac will no longer keep only the most recently installed of the two. (<a href="https://issuetracker.unity3d.com/issues/macos-targetsupport-installers-for-linux-overwrite-their-content">1331946</a>)</p></li>
<li><p>Editor: New parent is now placed properly if default parent is set. (<a href="https://issuetracker.unity3d.com/issues/scene-hierarchy-argumentexception-is-thrown-on-applying-recursive-parenting-for-objects">1324389</a>)</p></li>
<li><p>Editor: On macOS, fixed an issue where clicking on the game view in play mode would cause unexpected mouse delta data. (1343436)</p></li>
<li><p>Editor: Prefab instances no longer lose their modifications after a scene template instantiation.</p></li>
<li><p>Editor: Prevent context menus near the edge of the screen from popping far away from the context-click on macOS. (<a href="https://issuetracker.unity3d.com/issues/macos-some-native-dropdown-menu-shifts-upwards-when-dropdown-that-is-clicked-is-close-to-the-bottom-of-the-screen">1339181</a>)</p></li>
<li><p>Editor: Properly restore Settings Window splitter position when domain reload happens. (<a href="https://issuetracker.unity3d.com/issues/project-settings-panel-width-changes-when-reimporting-a-script">1359479</a>)</p></li>
<li><p>Editor: Reduced the autocomplete popup width and trimmed the search item label to support long search terms. (1348672)</p></li>
<li><p>Editor: Reduced time processing mesh static batches when loading scenes additively. (<a href="https://issuetracker.unity3d.com/issues/static-batching-is-recalculated-for-every-loaded-scene-additively-when-using-multiple-scenes">1143037</a>)</p></li>
<li><p>Editor: Shader search window will now display results based on whether the search string matches any part of the full Shader path. (1334043)</p></li>
<li><p>Editor: The Project window lock icon will now show a ping indicator if an attempt to frame/ping an asset is made and the window is locked. (<a href="https://issuetracker.unity3d.com/issues/sprite-is-not-highlighting-in-the-project-window-when-using-specific-layout">1362598</a>)</p></li>
<li><p>Editor: Tooltips not closing automatically when the mouse moves out from the rect of the ui part that triggered them.</p></li>
<li><p>Editor: Unified the il2cpp default order for managed stripping levels in the Player Settings drop-down menu to the one of Mono (Minimal &gt; Low &gt; Medium &gt; High).</p></li>
<li><p>Editor: Updating EditorScript behavior in SceneView based on Inspector visibility. (<a href="https://issuetracker.unity3d.com/issues/onscenegui-is-not-being-called-when-using-a-certain-layout">1340534</a>)</p></li>
<li><p>Editor: Values of UnityEngine.Device.Screen.width/height are now consistent when using Device Simulator and don't change during different events. (<a href="https://issuetracker.unity3d.com/issues/incorrect-screen-dot-width-and-screen-dot-height-values-returned-in-onenable-when-reenabling-a-monobehavior-in-the-editor-during-playmode">1335981</a>)</p></li>
<li><p>Editor: When in a different editormode, ensure ExecuteMenuItem works with default menu paths. (<a href="https://issuetracker.unity3d.com/issues/possible-regression-editorapplication-dot-executemenuitem-wont-execute-a-menu-item-hidden-by-an-active-editor-mode">1377944</a>)</p></li>
<li><p>GI: Added test is disabled on all Editor platforms. (1361081)</p></li>
<li><p>GI: Avoid falling back to CPU Lightmapper in scenes with only black direct lights. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-error-compositorcoresettings-dot-m-directenabled-and-fallback-to-cpu-plm-after-starting-gi-bake">1356606</a>)</p></li>
<li><p>GI: Baking with progressive updates ON or OFF with the GPULM always gives the same result. (<a href="https://issuetracker.unity3d.com/issues/plm-different-results-are-generated-when-progressive-updates-is-on-or-off-while-progressive-gpu-lightmapper-is-selected">1352923</a>)</p></li>
<li><p>GI: Exposed API for environmentMIS property in LightingSettings. (<a href="https://issuetracker.unity3d.com/issues/environmentmis-property-in-lightingsettings-is-not-exposed">1338804</a>)</p></li>
<li><p>GI: Fixed a bug where additively loading a scene could cause lighting data assets to be altered, and new lighting data assets to be created. (1381583)</p></li>
<li><p>GI: Fixed a small offset in GPULM light cookie textures. (<a href="https://issuetracker.unity3d.com/issues/baked-cookies-are-offset-between-gpu-and-cpu-lightmapper">1333945</a>)</p></li>
<li><p>GI: Fixed an issue where changing Lightmap Encoding would cause Texture Importers for HDR cubemaps to enter an invalid state when targeting mobile platforms. (<a href="https://issuetracker.unity3d.com/issues/encoding-slash-compression-lightmap-encoding-changes-cause-unexpected-textureimporter-state-on-reflection-probes-ios">1297258</a>)</p></li>
<li><p>GI: Fixed an issue where it was possible to set the value of maxBounces to less than that of minBounces when setting these values via the API. (<a href="https://issuetracker.unity3d.com/issues/api-the-value-of-minbounces-can-go-over-that-of-maxbounces-when-set-through-the-api">1350279</a>)</p></li>
<li><p>GI: Fixed case where the Enlighten Realtime GI charting visualization would not work. (<a href="https://issuetracker.unity3d.com/issues/enlighten-uv-charts-visualization-is-not-shown-with-multiple-errors-when-opening-through-the-lightmap-preview-window">1353283</a>)</p></li>
<li><p>GI: Fixed denoising issues with OIDN and OptiX denoisers on GPULM when using different values for direct lighting sample count and indirect lighting sample count. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-denoising-artifacts-after-baking-gi-on-a-scene-with-certain-lighting-settings-and-denoising-enabled">1337396</a>)</p></li>
<li><p>GI: Fixed issue where error messages from baking cannot be cleared when clearing lighting from the lighting panel. (<a href="https://issuetracker.unity3d.com/issues/pathtracer-failed-to-add-geometry-for-mesh-mesh-contains-non-finite-values-dot-error-cant-be-cleared-when-baking-lightning">1323367</a>)</p></li>
<li><p>GI: Fixed issue where lightmaps would be lost when loading a scene additively when the main scene uses realtime GI and is baked with auto mode. (<a href="https://issuetracker.unity3d.com/issues/lightmap-is-lost-when-loading-additive-scene">1346566</a>)</p></li>
<li><p>GI: Fixed issue with the Lightmap Exposure value getting lost when entering and exiting Playmode. (<a href="https://issuetracker.unity3d.com/issues/when-in-draw-mode-using-baked-lightmap-the-lightmap-exposure-resets-after-returning-from-play-mode">1362687</a>)</p></li>
<li><p>GI: Fixed light reset, remove any cookie that might be attached to the light. (1335363)</p></li>
<li><p>GI: Fixed NullReferenceException when viewing the reflection probe inspector while a custom editor for Cubemap exists. (<a href="https://issuetracker.unity3d.com/issues/reflection-probe-inspector-preview-breaks-whith-custom-cubemap-inspector">1341400</a>)</p></li>
<li><p>GI: Fixed realtime GI assertion errors from terrain lighting caused by mesh in scene with broken UV2s. (1348485)</p></li>
<li><p>GI: Fixed regression where the GPU Lightmapper hangs when exporting training data in a scene with no active lights. (1350077)</p></li>
<li><p>GI: Fixed unexpected fallbacks from the GPULM to the CPULM when changing filtering settings during a bake. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-fallback-to-cpu-plm-with-useradeon-radeondenoiser-dot-isnull-after-switching-filtering-settings-and-rebaking-gi">1364204</a>)</p></li>
<li><p>GI: Normalized normals in the meshes is now passed to the progressive lightmappers. (1356670)</p></li>
<li><p>GI: Small lighting settings UI tweaks.</p></li>
<li><p>Graphics: Added new renderingLayerMask parameter for RendererListDesc. This will parameter will allow users to configure the rendering layer mask filter for the respective renderer list.</p></li>
<li><p>Graphics: Added rendering layer support to instanced terrain details. (<a href="https://issuetracker.unity3d.com/issues/terrain-details-hdrp-noticeable-lighting-difference-when-a-detail-prefab-painted-on-terrain">1334605</a>)</p></li>
<li><p>Graphics: Attempting to draw with disposed argument buffer with DrawProceduralNow functions now issues an error to the log instead of a crash. (<a href="https://issuetracker.unity3d.com/issues/crash-when-using-graphics-dot-drawproceduralindirectnow">1356448</a>)</p></li>
<li><p>Graphics: Enabled Depth Sharing in Vulkan.</p></li>
<li><p>Graphics: Enabled support for dynamic resolution when using Vulkan on Windows and Linux. (<a href="https://issuetracker.unity3d.com/issues/dynamic-resolution-doesnt-work-when-graphics-api-is-set-to-vulkan">1337161</a>)</p></li>
<li><p>Graphics: Fixed 16bpc to 8bpc quantizing bug in the texture importer for type Sprite. (1303552)</p></li>
<li><p>Graphics: Fixed a crash on Vulkan/Metal when trying to preview non-Float or non-UNorm format RenderTextures. (1332920)</p></li>
<li><p>Graphics: Fixed a crash when using OpenGL and SRP batcher with async shader compilation. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-gfxdevicegles-drawbuffersbatchmode-when-loading-a-scene">1374270</a>)</p></li>
<li><p>Graphics: Fixed a critical issue on android devices &amp; lens flares. Accidentally creating a 16 bit texture was causing gpus not supporting them to fail.</p></li>
<li><p>Graphics: Fixed a deadlock that can occur when MasterTextureLimit is changed while a texture has an in-progress upload request. (<a href="https://issuetracker.unity3d.com/issues/unity-freezes-when-modifying-mastertexturelimit-while-texture-mipmap-streaming-is-in-the-fly">1382467</a>)</p></li>
<li><p>Graphics: Fixed a large, visible stretch ratio in a LensFlare Image thumbnail.</p></li>
<li><p>Graphics: Fixed a performance issue in the SRP Render loop. (<a href="https://issuetracker.unity3d.com/issues/hdrp-renderloop-dot-prepare-takes-up-a-lot-of-cpu">1369766</a>)</p></li>
<li><p>Graphics: Fixed alignment in Volume Components.</p></li>
<li><p>Graphics: Fixed an assert spam (data != nullptr) in the Console Window when ray tracing effects are used in HDRP. (1380929)</p></li>
<li><p>Graphics: Fixed an error message logged by RenderTexture assets suggesting an incorrect/confusing fallback format when attempting to use an incompatible color format while "Enable Compatible Format" was turned off. Additionally, the RenderTexture.graphicsFormat getter no longer logs errors/warnings. (1353831)</p></li>
<li><p>Graphics: Fixed an incorrect preprocessor define causing ImageConversion.EncodeArrayToTGA (and overloads) to always fail. (1340467)</p></li>
<li><p>Graphics: Fixed an issue causing Render Graph execution errors after a random amount of time.</p></li>
<li><p>Graphics: Fixed an issue in DynamicResolutionHandler when camera request was turned off at runtime, the ScalableBufferManager would leak state and not unset DRS state.</p></li>
<li><p>Graphics: Fixed an issue that the depthSlice is not set for depth attachement when using depth only NativeRenderPass. (1381464)</p></li>
<li><p>Graphics: Fixed an issue were asserts were triggered upon creating uninitialized textures. (1342524)</p></li>
<li><p>Graphics: Fixed an issue were errors related to .raytrace shader (RayTracingShader) setup were not removed from the Console Window in the Editor after they were fixed. (1362269)</p></li>
<li><p>Graphics: Fixed an issue where preview objects were being drawn in an unexpected layer. They are now drawn using layer 0 (Default) instead of layer 1 (TransparentFX). (<a href="https://issuetracker.unity3d.com/issues/material-slash-prefab-preview-window-view-is-black-slash-gray-when-using-a-custom-lit-shader-where-ztest-is-changed-from-lequel-to-equel">1361557</a>)</p></li>
<li><p>Graphics: Fixed an issue where RayTracingAccelerationStructure.CullInstances was not accepting a Renderer into the RTAS that uses a mix of Opaque and Transparent Materials while RayTracingInstanceCullingTest.allowTransparentMaterials was false. (<a href="https://issuetracker.unity3d.com/issues/hdrp-dxr-multimat-opaque-materials-are-not-included-in-the-rtas-when-there-at-least-one-transparent-in-the-mat-list">1381388</a>)</p></li>
<li><p>Graphics: Fixed an issue where Texture.CreateExternalTexture was not detecting the native texture format on DirectX12. (1343696)</p></li>
<li><p>Graphics: Fixed an issue where Texture2D.UpdateExternalTexture did not work on vulkan. (1355632)</p></li>
<li><p>Graphics: Fixed an issue where textures were relying on uninitialized sentinel values by making uninitialized data optional. (<a href="https://issuetracker.unity3d.com/issues/certain-object-field-icons-in-editor-are-not-rendered">1342022</a>)</p></li>
<li><p>Graphics: Fixed an issue where TexturesD3D11Base::RegisterNativeTexture ignored format from UnityEngine.Cubemap.CreateExternalTexture when creating the SRV. (1281016)</p></li>
<li><p>Graphics: Fixed an SRP Batcher issue with Integer properties affecting GPU state. (<a href="https://issuetracker.unity3d.com/issues/srp-batcher-batches-materials-together-when-using-different-integer-stencil-ref-and-comp-values">1355311</a>)</p></li>
<li><p>Graphics: Fixed artifacts when calling ReflectionProbe.BlendCubemap(). (<a href="https://issuetracker.unity3d.com/issues/android-opengl-artifacts-appear-on-a-gameobject-using-cubemap-material-when-the-app-is-launched-for-the-first-time">1360030</a>)</p></li>
<li><p>Graphics: Fixed AssetPreviews + texture preview window for ASTCnm/Plain normal maps.</p></li>
<li><p>Graphics: Fixed BatchRendererGroup objects not being pickable.</p></li>
<li><p>Graphics: Fixed binding read-only depth/stencil attachments as texture when using Vulkan.</p></li>
<li><p>Graphics: Fixed black pixel issue in AMD FidelityFX RCAS implementation.</p></li>
<li><p>Graphics: Fixed black RenderTarget/CustomRenderTarget thumbnails when changing Color/Depth formats. (1340733)</p></li>
<li><p>Graphics: Fixed copying between ARGB regular texture and RT on Vulkan. (1371407)</p></li>
<li><p>Graphics: Fixed corrupt mipmap calculations during RG32 and RGB48 texture importing. (1340126)</p></li>
<li><p>Graphics: Fixed crash when creating a RenderTexture with dimensions exceeding the capabilities of the current graphics device. (<a href="https://issuetracker.unity3d.com/issues/macos-crash-on-pthread-kill-when-render-texture-has-no-depth-buffer-and-dimension-is-3d">1313675</a>)</p></li>
<li><p>Graphics: Fixed cropped thumbnail for Image with non-uniform scale and rotation.</p></li>
<li><p>Graphics: Fixed failing CopyTexture in Editor when build target is a mobile platform and the source texture is a normal map or lightmap. (<a href="https://issuetracker.unity3d.com/issues/android-opengl-graphics-dot-copytexture-throws-an-error-when-using-normal-map-texture">1365807</a>)</p></li>
<li><p>Graphics: Fixed GLSL shader compilation error on some OpenGL drivers when using SV_RenderTargetArrayIndex with tessellation shaders. (<a href="https://issuetracker.unity3d.com/issues/shaders-using-sv-rendertargetarrayindex-with-tessellation-stages-fail-to-compile-with-opengl">1261150</a>)</p></li>
<li><p>Graphics: Fixed high CPU/GPU utilization when occlusion window is open. (<a href="https://issuetracker.unity3d.com/issues/cpu-slash-gpu-utilization-goes-up-to-10-40-percent-when-occlusion-culling-window-is-opened-and-mouse-is-over-the-occlusion-window-in-the-scene">1341977</a>)</p></li>
<li><p>Graphics: Fixed high memory usage in Vulkan backend when using many different textures per texture property of a shader. (<a href="https://issuetracker.unity3d.com/issues/vulkan-randomly-assigned-material-texture-or-buffer-properties-can-cause-huge-memory-usage">1372610</a>)</p></li>
<li><p>Graphics: Fixed IES Importer related to new API on core.</p></li>
<li><p>Graphics: Fixed IES profile importer handling of overflow (outside 0-1 range) of attenutation splines values.</p></li>
<li><p>Graphics: Fixed incorrect rendering result when HDR rendering support is disabled in GraphicsSettings but HDR output is enabled in PlayerSettings. (<a href="https://issuetracker.unity3d.com/issues/rendering-using-hdr-output-with-graphicssettings-hdr-disabled-caused-incorrect-rendering">1363703</a>)</p></li>
<li><p>Graphics: Fixed incorrect rendering when having object with negative scale. (<a href="https://issuetracker.unity3d.com/issues/urp-camera-stops-rendering-when-a-certain-object-is-enabled-in-the-scene">1280030</a>)</p></li>
<li><p>Graphics: Fixed incorrect rendering when SRP Batcher skips invalid meshes during BRG rendering. (1383042)</p></li>
<li><p>Graphics: Fixed incorrectly regenerated thumbnails when reimporting sprites with an asset postprocessor. (<a href="https://issuetracker.unity3d.com/issues/thumbnail-in-the-project-window-is-not-updated-when-a-sprites-texture-is-altered">1351651</a>)</p></li>
<li><p>Graphics: Fixed issue in which the camera rendered into the backbuffer instead of a temporary texture. (<a href="https://issuetracker.unity3d.com/issues/metal-hdrp-error-creating-pipeline-state-hidden-slash-hdrp-slash-copydepthbuffer-in-hdrp-graphic-test">1362704</a>)</p></li>
<li><p>Graphics: Fixed issue when changing volume profiles at runtime with a script.</p></li>
<li><p>Graphics: Fixed keyword and float property upgrading in SpeedTree8MaterialUpgrader.</p></li>
<li><p>Graphics: Fixed leaving uncleared screen after changing aspect ratio. (<a href="https://issuetracker.unity3d.com/issues/build-screen-is-not-cleared-when-changing-the-aspect-ratio-on-openglcore-graphics-api">1367899</a>)</p></li>
<li><p>Graphics: Fixed leftover memory when switching scenes when using Vulkan. (<a href="https://issuetracker.unity3d.com/issues/android-vulkan-graphics-memory-is-not-released-when-switching-between-scenes">1293458</a>)</p></li>
<li><p>Graphics: Fixed Lens Flare 'radialScreenAttenuationCurve invisible'.</p></li>
<li><p>Graphics: Fixed Lens Flare rotation for Curve Distribution.</p></li>
<li><p>Graphics: Fixed Lens Flare Thumbnails.</p></li>
<li><p>Graphics: Fixed library function SurfaceGradientFromTriplanarProjection to match the mapping convention used in SampleUVMappingNormalInternal.hlsl and fix its description.</p></li>
<li><p>Graphics: Fixed LightAnchor too much error message, became a HelpBox on the Inspector.</p></li>
<li><p>Graphics: Fixed Mac Metal player so red edges no longer appear when dragging resizable windows. (<a href="https://issuetracker.unity3d.com/issues/mac-metal-red-edges-appear-when-dragging-a-resizable-player-window">1298578</a>)</p></li>
<li><p>Graphics: Fixed memory leak when changing SRP pipeline settings, and having the player in pause mode.</p></li>
<li><p>Graphics: Fixed memory leak when using Vulkan GraphicsJobs. (1333454)</p></li>
<li><p>Graphics: Fixed Mesh.AddBlendShapeFrame not properly updating mesh layout to be compatible with GPU blend shapes. (<a href="https://issuetracker.unity3d.com/issues/blendshapes-added-with-mesh-dot-addblendshapeframe-are-not-updated-correctly-when-modifying-the-offsets">1312251</a>)</p></li>
<li><p>Graphics: Fixed Metal error when copying textures with mismatched data. (<a href="https://issuetracker.unity3d.com/issues/data-size-for-different-pixel-format-textures-error-is-thrown-when-copying-textures-using-commandbuffer-dot-copytexture-method">1374449</a>)</p></li>
<li><p>Graphics: Fixed numerous cases where mini-thumbnails would not match the expected visual look when using linear project color space.</p></li>
<li><p>Graphics: Fixed possible out-of-memory when minimizing a Player that uses Vulkan on Windows. (<a href="https://issuetracker.unity3d.com/issues/out-of-memory-when-minimizing-gpu-bound-vulkan-player-with-run-in-background-enabled">1372535</a>)</p></li>
<li><p>Graphics: Fixed potential for LineRenderer.BakeMesh and TrailRenderer.BakeMesh to fail with invalid AABB error messages. (<a href="https://issuetracker.unity3d.com/issues/linerenderer-dot-bakemesh-fails-when-called-on-instantiated-copy">1349946</a>)</p></li>
<li><p>Graphics: Fixed realoading of VFX Assets while inspecting a Cube Render Texture. (<a href="https://issuetracker.unity3d.com/issues/vfxs-reimport-when-entering-play-mode-if-a-render-texture-of-dimension-cube-is-selected">1340307</a>)</p></li>
<li><p>Graphics: Fixed realtime GI when using OpenGL. (<a href="https://issuetracker.unity3d.com/issues/urp-enlighten-regression-where-not-all-surfaces-are-contributing-to-the-gi-on-mobiles">1339133</a>)</p></li>
<li><p>Graphics: Fixed reported out-of-memory error on Scarlett devices when trying to create 96bpp textures.</p></li>
<li><p>Graphics: Fixed scene being made dirty when creating a new RenderTexture asset. (<a href="https://issuetracker.unity3d.com/issues/scene-becomes-dirty-when-a-new-rendertexture-asset-is-created">1331120</a>)</p></li>
<li><p>Graphics: Fixed serialization of DebugStateFlags, the internal Enum was not being serialized.</p></li>
<li><p>Graphics: Fixed Single Channel Red mini-thumbnails not actually being red-only.</p></li>
<li><p>Graphics: Fixed small inconsistencies between the various ImageConvertion.EncodeArrayToEXR (and overload) functions. (1340476)</p></li>
<li><p>Graphics: Fixed sporadic crashes when using Vulkan. (1386731)</p></li>
<li><p>Graphics: Fixed the issue with the special Turkish i, when looking for the m_IsGlobal property in VolumeEditor.</p></li>
<li><p>Graphics: Fixed truncation of Vulkan descriptor set handles on 32bit platforms, causing validation errors.</p></li>
<li><p>Graphics: Fixed undefined behaviour occurring with AssetPreview for Single Channel Alpha texture types.</p></li>
<li><p>Graphics: Fixed Undo from script refreshing thumbnail.</p></li>
<li><p>Graphics: Fixed use of invalid swapchain handle with AMD GPUs on Windows. (1372538)</p></li>
<li><p>Graphics: Fixed Volume Gizmo size when rescaling parent GameObject.</p></li>
<li><p>Graphics: Fixed Vulkan validation error when creating a 3D RenderTexture with mip maps. (1367999)</p></li>
<li><p>Graphics: Fixed Vulkan validation error when using texelFetch with images that don't support linear filtering. (1367541)</p></li>
<li><p>Graphics: Fixed XR support in CoreUtils.DrawFullscreen function.</p></li>
<li><p>Graphics: GrabIntoRenderTexture uses invalid viewport with UTR on D3D11 when formats not compatible. (1325579)</p></li>
<li><p>Graphics: Help boxes with fix buttons do not crop the label.</p></li>
<li><p>Graphics: LODGroup.lastLODBillboard is now exposed to C# API. (1325954)</p></li>
<li><p>Graphics: Mesh.SetVertexBufferParams prints a warning if input mesh layout has skinning data but is not compatible with Unity in how vertex streams are laid out. (<a href="https://issuetracker.unity3d.com/issues/mesh-is-shaded-as-black-when-setting-boneweights-via-advanced-mesh-api">1320869</a>)</p></li>
<li><p>Graphics: Metal editor on OSX now uses CVDisplayLink to time frame presents; this fixes the unstable frame rate on some Macs in Play Mode. (<a href="https://issuetracker.unity3d.com/issues/macos-high-call-time-on-semaphore-dot-waitforsignal-while-rendering-on-empty-project">1297470</a>)</p></li>
<li><p>Graphics: Methods with DrawGizmo appear can now be disabled by the AnnotationManager. (<a href="https://issuetracker.unity3d.com/issues/unable-to-disable-volume-gizmos-anymore">1354816</a>)</p></li>
<li><p>Graphics: Mipchains with external Texture3D no longer cause a crash in Vulkan. (1344019)</p></li>
<li><p>Graphics: Removed URP and HDRP templates. They are now dynamic templates.</p></li>
<li><p>Graphics: Reset asset now works on RenderTexture and CustomRenderTexture assets. (<a href="https://issuetracker.unity3d.com/issues/imgui-reset-functionality-does-not-work-on-custom-render-texture">1285064</a>)</p></li>
<li><p>Graphics: StoreAndResolve actions are now overridden by Resolve actions if needed on Metal.</p></li>
<li><p>Graphics: Strip unused constant buffer members when using OpenGL (ES). (<a href="https://issuetracker.unity3d.com/issues/unused-constants-in-the-constant-buffer-are-not-stripped-out-when-using-opengles3">1359993</a>)</p></li>
<li><p>Graphics: SUCCEEDED(hr) error is thrown when the project's Shadows Filtering Quality is set to High or Very High. (<a href="https://issuetracker.unity3d.com/issues/hdrp-succeeded-hr-error-is-thrown-when-the-projects-shadows-filtering-quality-is-set-to-high-or-very-high">1340115</a>)</p></li>
<li><p>Graphics: The generated mini-thumbnail of TextureGenerationOutput will now properly set its expected stored color space. (1356076)</p></li>
<li><p>Graphics: Unwrapping.GenerateSecondaryUVSet now returns a bool value indicating success or failure. (<a href="https://issuetracker.unity3d.com/issues/setperindexuvs-failed-because-the-output-has-too-many-vertices-when-calling-unwrapping-dot-generatesecondaryuvset">1289982</a>)</p></li>
<li><p>Graphics: VFX Graph: Use main camera fallback if any expression requires the main camera, not only camera buffers. (<a href="https://issuetracker.unity3d.com/issues/vfxgraph-hdrp-maincamera-to-sceneview-fallback-doesnt-work-anymore">1367413</a>)</p></li>
<li><p>Graphics: Virtual Texturing fallback texture sampling code correctly honors the enableGlobalMipBias when virtual texturing is disabled.</p></li>
<li><p>Graphics: Vulkan no longer uses a secondary command buffer for a single clear call.  We also no longer attempt to execute empty command buffers. (1333723)</p></li>
<li><p>Graphics: When adding Overrides to the Volume Profile, only show Volume Components from the current Pipeline.</p></li>
<li><p>Graphics: Workaround for immediate vertices getting split up. (<a href="https://issuetracker.unity3d.com/issues/gap-in-line-strip-when-drawing-using-gl-dot-line-strip-with-768-lines-or-more">1353549</a>)</p></li>
<li><p>Graphics: [DX12] Fixed a crash when TexturesD3D12::RegisterNativeTexture was called with resource that has *_TYPELESS format. (<a href="https://issuetracker.unity3d.com/issues/dx12-crash-when-texturesd3d12-registernativetexture-is-called-with-resource-that-has-star-typeless-format">1343602</a>)</p></li>
<li><p>Graphics: [FrameDebugger] Fix incorrect ColorMask shown. (1360825)</p></li>
<li><p>Graphics: [Vulkan] Fixed an issue where the texture memory in Memory Profiler Module was not updated when profiling a Vulkan build. (<a href="https://issuetracker.unity3d.com/issues/vulkan-texture-memory-in-memory-profiler-module-is-not-updated-when-profiling-a-vulkan-build">1320962</a>)</p></li>
<li><p>HDRP: Added support for negative wind speed parameter.</p></li>
<li><p>HDRP: Added Undo Support for HDRP Global Settings asset assignation.</p></li>
<li><p>HDRP: Fixed a compilation issue for AxF carpaints on Vulkan.</p></li>
<li><p>HDRP: Fixed a crash issue when adding an area light on its own.</p></li>
<li><p>HDRP: Fixed a crash with render graph viewer when render graph is not provided with an execution name.</p></li>
<li><p>HDRP: Fixed a divide-by-zero warning for anisotropic shaders (Fabric, Lit).</p></li>
<li><p>HDRP: Fixed a lack of syncronization between the camera and the planar camera for volumetric cloud animation data.</p></li>
<li><p>HDRP: Fixed a memory leak related to not disposing of the RTAS at the end HDRP's lifecycle.</p></li>
<li><p>HDRP: Fixed a null ref exception in Volume Explorer.</p></li>
<li><p>HDRP: Fixed a null ref exception when adding a new environment to the Look Dev library.</p></li>
<li><p>HDRP: Fixed a null ref exception when no opaque objects are rendered.</p></li>
<li><p>HDRP: Fixed a nullref exception when creating a new scene while LightExplorer is open.</p></li>
<li><p>HDRP: Fixed a nullref when binding a RTHandle allocated from a RenderTextureIdentifier with CoreUtils.SetRenderTarget.</p></li>
<li><p>HDRP: Fixed a nullref when enabling raycount without ray tracing.</p></li>
<li><p>HDRP: Fixed a regression that was introduced in the diffuse denoiser in a previous PR.</p></li>
<li><p>HDRP: Fixed a shader warning in UnityInstancing.hlsl.</p></li>
<li><p>HDRP: Fixed a warning because of a null texture in the lens flare pass.</p></li>
<li><p>HDRP: Fixed a warning because of a null texture in the lens flare pass.</p></li>
<li><p>HDRP: Fixed a warning to Rendering Debugger Runtime UI when debug shaders are stripped.</p></li>
<li><p>HDRP: Fixed a warning when enabling tile/cluster debug.</p></li>
<li><p>HDRP: Fixed access to main directional light from script.</p></li>
<li><p>HDRP: Fixed Additional Velocity for Alembic not taking correctly into account vertex animation.</p></li>
<li><p>HDRP: Fixed ambient occlusion strenght incorrectly using GTAOMultiBounce.</p></li>
<li><p>HDRP: Fixed an incompatibility between MSAA and Volumetric Clouds.</p></li>
<li><p>HDRP: Fixed an inconsistency between perf mode and quality mode for material simplification in RTGI.</p></li>
<li><p>HDRP: Fixed an inconsistency between perf mode and quality mode for sky lighting.</p></li>
<li><p>HDRP: Fixed an infinite import loop of materials when there is no HDMetaData generated by the ShaderGraph.</p></li>
<li><p>HDRP: Fixed an issue that made camera motion vectors unavailable in custom passes.</p></li>
<li><p>HDRP: Fixed an issue that made Custom Pass buffers inaccessible in ShaderGraph.</p></li>
<li><p>HDRP: Fixed an issue where disabled reflection probes were still sent into the ray tracing light cluster.</p></li>
<li><p>HDRP: Fixed an issue where forced sky update (like PBR sky amortized updated) would not update ambient probe.</p></li>
<li><p>HDRP: Fixed an issue where Shadow Matte does not appear in ray tracing effects. (<a href="https://issuetracker.unity3d.com/issues/shadow-of-unlit-shadow-matte-not-captured-in-raytraced-reflections">1364005</a>)</p></li>
<li><p>HDRP: Fixed an issue where sometimes full screen debug would cause render graph errors.</p></li>
<li><p>HDRP: Fixed an issue with reflection probe normalization via APV when no probes are in scene.</p></li>
<li><p>HDRP: Fixed an issue with resolution dependence for physically based depth of field.</p></li>
<li><p>HDRP: Fixed an issue with surface gradient based normal blending for decals (volume gradients weren't converted to SG before resolving in some cases).</p></li>
<li><p>HDRP: Fixed an issue with TAA causing objects not to render at extremely high far flip plane values.</p></li>
<li><p>HDRP: Fixed and optimize distance shadowmask fade.</p></li>
<li><p>HDRP: Fixed API warnings in Matcap mode on Metal.</p></li>
<li><p>HDRP: Fixed area light cookie field to use the same style as the other cookie fields.</p></li>
<li><p>HDRP: Fixed artifacts in volumetric cloud shadows.</p></li>
<li><p>HDRP: Fixed assert failure when enabling the probe volume system for the first time.</p></li>
<li><p>HDRP: Fixed atmospheric scattering being incorrectly enabled when scene lighting is disabled.</p></li>
<li><p>HDRP: Fixed bad feedback loop occuring when auto exposure adaptation time was too small.</p></li>
<li><p>HDRP: Fixed broken rendering when duplicating a camera while the Rendering Debugger is opened.</p></li>
<li><p>HDRP: Fixed cached directional light shadows disappearing without reappearing when the going outside of the range of shadow validity.</p></li>
<li><p>HDRP: Fixed camera motion vector pass reading last frame depth texture.</p></li>
<li><p>HDRP: Fixed cases in which object and camera motion vectors would cancel out, but didn't.</p></li>
<li><p>HDRP: Fixed CoC size computation when dynamic resolution is enabled.</p></li>
<li><p>HDRP: Fixed compatibility message not displayed correctly when switching platforms.</p></li>
<li><p>HDRP: Fixed conflicting runtime debug menu command with an option to disable runtime debug window hotkey.</p></li>
<li><p>HDRP: Fixed contact shadow debug views not displaying correctly upon resizing of view.</p></li>
<li><p>HDRP: Fixed contact shadow disappearing when shadowmask is used and no non-static object is available.</p></li>
<li><p>HDRP: Fixed controls for clouds fade in.</p></li>
<li><p>HDRP: Fixed CPU performance on DLSS, avoiding to recreate state whenever a target can fall into the safe min/max resolution specified by the system.</p></li>
<li><p>HDRP: Fixed crash on SubSurfaceScattering Editor when the selected pipeline is not HDRP.</p></li>
<li><p>HDRP: Fixed crossfade not working on the HD ST8 ShaderGraph.</p></li>
<li><p>HDRP: Fixed custom pass injection point not visible in the UI when using the Camera mode.</p></li>
<li><p>HDRP: Fixed custom pass name being cut when too long in the inspector.</p></li>
<li><p>HDRP: Fixed custom pass utils Blur and Copy functions in XR.</p></li>
<li><p>HDRP: Fixed custom pass volume not executed in scene view because of the volume culling mask.</p></li>
<li><p>HDRP: Fixed custom pass workflow for single camera effects.</p></li>
<li><p>HDRP: Fixed custom post process name not displayed correctly in GPU markers.</p></li>
<li><p>HDRP: Fixed custom post process template not working with Blit method.</p></li>
<li><p>HDRP: Fixed custom shader GUI for material inspector.</p></li>
<li><p>HDRP: Fixed CustomPassUtils.Copy function not working on depth buffers.</p></li>
<li><p>HDRP: Fixed D3D validation layer errors w.r.t shadow textures when an atlas is not used.</p></li>
<li><p>HDRP: Fixed debug window reset.</p></li>
<li><p>HDRP: Fixed decal performances when they use different material and the same draw order.</p></li>
<li><p>HDRP: Fixed depth pyramid being incorrect when having multiple cameras (scene view and gameview) and when hardware DRS was activated.</p></li>
<li><p>HDRP: Fixed diffusion profile being reset to default on SpeedTree8 materials with subsurface scattering enabled during import.</p></li>
<li><p>HDRP: Fixed diffusion profile displayed in the inspector.</p></li>
<li><p>HDRP: Fixed disabled menu item for volume additional properties.</p></li>
<li><p>HDRP: Fixed double camera preview.</p></li>
<li><p>HDRP: Fixed edge bleeding when rendering volumetric clouds.</p></li>
<li><p>HDRP: Fixed EmissiveLighting Debug Light mode not managing correctly emissive for unlit.</p></li>
<li><p>HDRP: Fixed enabling a lensflare in playmode.</p></li>
<li><p>HDRP: Fixed error messages when trying to use HDSceneColor, NormalFromHeight, DDX, DDY or DDXY shader graph nodes in ray tracing.</p></li>
<li><p>HDRP: Fixed error when disabling opaque objects on a camera with MSAA.</p></li>
<li><p>HDRP: Fixed error with motion blur and small render targets.</p></li>
<li><p>HDRP: Fixed errors about incorrect color spaces in the console when using the Wizzard to fix the project setup. (1388222)</p></li>
<li><p>HDRP: Fixed exposure issues with volumetric clouds on planar reflection.</p></li>
<li><p>HDRP: Fixed fabric IBL (Charlie) pre-convolution performance and accuracy (uses 1000x less samples and is closer match with the ground truth).</p></li>
<li><p>HDRP: Fixed failures on platforms that do not support ray tracing due to an engine behavior change.</p></li>
<li><p>HDRP: Fixed film grain &amp; dithering when using spatial upscaling methods for DRS.</p></li>
<li><p>HDRP: Fixed flickering / edge aliasing issue when DoF and TAAU or DLSS are enabled.</p></li>
<li><p>HDRP: Fixed Focus distance in path traced depth of field now takes into account the focus mode setting (volume vs camera).</p></li>
<li><p>HDRP: Fixed for allowing to change dynamic resolution upscale filter via script.</p></li>
<li><p>HDRP: Fixed for changes of color curves not being applied immediately.</p></li>
<li><p>HDRP: Fixed for discrepancies in intensity and saturation between screen space refraction and probe refraction.</p></li>
<li><p>HDRP: Fixed for screen space overlay rendered by camera when HDR is disabled.</p></li>
<li><p>HDRP: Fixed for wrong cached area light initialization.</p></li>
<li><p>HDRP: Fixed FOV change when enabling physical camera.</p></li>
<li><p>HDRP: Fixed gbuffer depth debug mode for materials not rendered during the prepass.</p></li>
<li><p>HDRP: Fixed geometry scale issue with the Eye Shader.</p></li>
<li><p>HDRP: Fixed ghosting issues if the exposure changed too much (RTGI).</p></li>
<li><p>HDRP: Fixed HDRP build issues with DOTS_INSTANCING_ON shader variant.</p></li>
<li><p>HDRP: Fixed HDRP camera debug panel rendering foldout.</p></li>
<li><p>HDRP: Fixed HDRP's ShaderGraphVersion migration management which was broken.</p></li>
<li><p>HDRP: Fixed impossibility to release the cursor in the template.</p></li>
<li><p>HDRP: Fixed incorrect RTHandle scale in DoF when TAA is enabled.</p></li>
<li><p>HDRP: Fixed invalid pass index 1 in DrawProcedural error.</p></li>
<li><p>HDRP: Fixed issue at edge of screen on some platforms when SSAO is on.</p></li>
<li><p>HDRP: Fixed issue that caused the uber post process to run even if nothing is to be done, leading to different results when disabling every post process manually vs disabling the whole post-processing pipeline.</p></li>
<li><p>HDRP: Fixed issue that placed an OnDemand shadow in the atlas before it was ever rendered.</p></li>
<li><p>HDRP: Fixed issue that would always save Decal Materials when saving the scene.</p></li>
<li><p>HDRP: Fixed issue where scene list was not refreshed upon deleting an APV baking set.</p></li>
<li><p>HDRP: Fixed issue with a compute dispatch being with 0 threads on extremely small resolutions.</p></li>
<li><p>HDRP: Fixed issue with accumulation motion blur and depth of field when path tracing is enabled.</p></li>
<li><p>HDRP: Fixed issue with automatic RendererList culling option getting ignored. (1388854)</p></li>
<li><p>HDRP: Fixed issue with change in lens model (perfect or imperfect) wouldn't be taken into account unless the HDRP asset was rebuilt.</p></li>
<li><p>HDRP: Fixed issue with depth slope scale depth bias when a material uses depth offset.</p></li>
<li><p>HDRP: Fixed issue with dynamic resolution and low res transparency sampling garbage outside of the render target.</p></li>
<li><p>HDRP: Fixed issue with fading in SSR applying fade factor twice, resulting in darkening of the image in the transition areas.</p></li>
<li><p>HDRP: Fixed issue with Final Image Histogram displaying a flat histogram on certain GPUs and APIs.</p></li>
<li><p>HDRP: Fixed issue with HDRI Sky and shadow filtering quality set to high.</p></li>
<li><p>HDRP: Fixed issue with hierarchy object filtering.</p></li>
<li><p>HDRP: Fixed issue with on-demand directional shadow maps looking broken when a reflection probe is updated at the same time.</p></li>
<li><p>HDRP: Fixed issue with path traced shadows and layer masks. (1375638)</p></li>
<li><p>HDRP: Fixed issue with Stacklit raytrace reflection.</p></li>
<li><p>HDRP: Fixed issue with typed loads on RGBA16F in Volumetric Lighting Filtering.</p></li>
<li><p>HDRP: Fixed issue with vertex color defaulting to 0.0 when not defined, in ray/path tracing.</p></li>
<li><p>HDRP: Fixed layer lit shader UI.</p></li>
<li><p>HDRP: Fixed lens flare not rendering correctly with TAAU or DLSS.</p></li>
<li><p>HDRP: Fixed light unit conversion after changing mid gray value.</p></li>
<li><p>HDRP: Fixed material inspector that allowed setting intensity to an infinite value.</p></li>
<li><p>HDRP: Fixed memory leak with XR combined occlusion meshes.</p></li>
<li><p>HDRP: Fixed minor performance issues in SSGI.</p></li>
<li><p>HDRP: Fixed misc TAA issue: Slightly improved TAA flickering, Reduced ringing of TAA sharpening, tweak TAA High quality central color filtering.</p></li>
<li><p>HDRP: Fixed missing API documentation for LTC area light code.</p></li>
<li><p>HDRP: Fixed missing global wind parameters in the visual environment.</p></li>
<li><p>HDRP: Fixed motion vector buffer not accessible from custom passes in the BeforeTransparent, BeforePreRefraction and AfterDepthAndNormal injection points.</p></li>
<li><p>HDRP: Fixed motion vector for custom meshes loaded from compute buffer in shader graph (like Hair).</p></li>
<li><p>HDRP: Fixed NeedMotionVectorForTransparent checking the wrong flag.</p></li>
<li><p>HDRP: Fixed Normal Map assiignation when importing FBX Materials.</p></li>
<li><p>HDRP: Fixed nullref when enabling fullscreen passthrough in HDRP Camera.</p></li>
<li><p>HDRP: Fixed NullReferenceException when opening a Volume Component with a Diffusion Profile with any inspector.</p></li>
<li><p>HDRP: Fixed object outline flickering with TAA.</p></li>
<li><p>HDRP: Fixed off by 1 error when calculating the depth pyramid texture size when DRS is on.</p></li>
<li><p>HDRP: Fixed options to trigger cached shadows updates on light transform changes.</p></li>
<li><p>HDRP: Fixed outdated documentation about recursie ray tracing effects support.</p></li>
<li><p>HDRP: Fixed outdated documentation about supported GPUs for ray tracing.</p></li>
<li><p>HDRP: Fixed override camera rendering custom pass API aspect ratio issue when rendering to a render texture.</p></li>
<li><p>HDRP: Fixed overwriting of preview camera background color. (<a href="https://issuetracker.unity3d.com/issues/previewrenderutility-is-not-respecting-the-background-when-previewing-a-3d-gameobject-from-2021-dot-1">1357004</a>)</p></li>
<li><p>HDRP: Fixed parameter ranges in HDRP Asset settings.</p></li>
<li><p>HDRP: Fixed performance penalty when hardware DRS was used between multiple views like editor or other gameviews.</p></li>
<li><p>HDRP: Fixed Pixel Displacement that could be set on tessellation shader while it's not supported.</p></li>
<li><p>HDRP: Fixed possible QNANS during first frame of SSGI, caused by uninitialized first frame data.</p></li>
<li><p>HDRP: Fixed Post Process not editable in the default frame settings.</p></li>
<li><p>HDRP: Fixed potential asymmetrical resource release in the volumetric clouds. (1388218)</p></li>
<li><p>HDRP: Fixed precision issues with the scene voxelization for APV, especially with geometry at the origin.</p></li>
<li><p>HDRP: Fixed Probe volume debug exposure compensation to match the Lighting debug one.</p></li>
<li><p>HDRP: Fixed public API for Diffusion Profile Override volume Component.</p></li>
<li><p>HDRP: Fixed range compression factor being clamped. (<a href="https://issuetracker.unity3d.com/issues/hdrp-planar-reflection-probe-range-compression-factor">1365707</a>)</p></li>
<li><p>HDRP: Fixed Realtime lightmap not working correctly in player with various lit shader.</p></li>
<li><p>HDRP: Fixed regression in the ambient probe intensity for volumetric clouds.</p></li>
<li><p>HDRP: Fixed regression in the clouds presets.</p></li>
<li><p>HDRP: Fixed remapping of depth pyramid debug view.</p></li>
<li><p>HDRP: Fixed remove of the Additional Camera Data when removing the Camera Component.</p></li>
<li><p>HDRP: Fixed remove of the Additional Light Data when removing the Light Component.</p></li>
<li><p>HDRP: Fixed Render Graph Debug UI not refreshing correctly in the Rendering Debugger.</p></li>
<li><p>HDRP: Fixed rendering of objects just after the TAA pass (before post process injection point).</p></li>
<li><p>HDRP: Fixed rendertarget ColorMask in Forward with virtual texturing and transparent motion vectors.</p></li>
<li><p>HDRP: Fixed robustness issues with the stacklit material in path tracing. (<a href="https://issuetracker.unity3d.com/issues/hdrp-dxr-pathtracer-stacklit-supports-breaks-when-coat-mask-parameter-is-exposed-and-equals-zero">1373971</a>)</p></li>
<li><p>HDRP: Fixed rounding issue when accessing the color buffer in the DoF shader.</p></li>
<li><p>HDRP: Fixed scaling issues with dynamic resolution and the CustomPassSampleCameraColor function.</p></li>
<li><p>HDRP: Fixed sceneview debug mode rendering.</p></li>
<li><p>HDRP: Fixed screen space shadow debug view not showing when no shadows is available.</p></li>
<li><p>HDRP: Fixed screen space shadow when multiple lights cast shadows.</p></li>
<li><p>HDRP: Fixed selection of light types (point, area, directional) for path-traced Unlit shadow mattes.</p></li>
<li><p>HDRP: Fixed Shader advanced options for lit shaders.</p></li>
<li><p>HDRP: Fixed shader graph errors when disabling the bias on texture samplers.</p></li>
<li><p>HDRP: Fixed shadow cascade transition not working properly with bias.</p></li>
<li><p>HDRP: Fixed shadow sampling artifact when using the spot light shadow option 'custom spot angle'.</p></li>
<li><p>HDRP: Fixed shadowmask editable when not supported.</p></li>
<li><p>HDRP: Fixed sky jittering when TAA is enabled.</p></li>
<li><p>HDRP: Fixed sky override layer mask having no effect.</p></li>
<li><p>HDRP: Fixed some aliasing ussues with the volumetric clouds.</p></li>
<li><p>HDRP: Fixed some depth comparison instabilities with volumetric clouds.</p></li>
<li><p>HDRP: Fixed some of the extreme ghosting in DLSS by using a bit mask to bias the color of particles. VFX tagged as Exclude from TAA will be on this pass.</p></li>
<li><p>HDRP: Fixed some XR devices: Pulling camera world space position from mainViewConstants instead of transform.</p></li>
<li><p>HDRP: Fixed sorting for mesh decals.</p></li>
<li><p>HDRP: Fixed specular anti aliasing for layeredlit shader.</p></li>
<li><p>HDRP: Fixed specular occlusion sharpness and over darkening at grazing angles.</p></li>
<li><p>HDRP: Fixed SpeedTree graph compatibility by removing custom interpolators.</p></li>
<li><p>HDRP: Fixed spot light shadows near plane.</p></li>
<li><p>HDRP: Fixed stackLit coat screen space reflection and raytrace reflection light hierarchy and IBL fallback.</p></li>
<li><p>HDRP: Fixed static lighting sky update when using an HDRI sky with a render texture in parameter.</p></li>
<li><p>HDRP: Fixed stencil buffer resolve when MSAA is enabled so that OR operator is used instead of picking the last sample.</p></li>
<li><p>HDRP: Fixed support for instanced motion vector rendering.</p></li>
<li><p>HDRP: Fixed support for interleaved tiling in path tracing.</p></li>
<li><p>HDRP: Fixed support for light/shadow dimmers (volumetric or not) in path tracing.</p></li>
<li><p>HDRP: Fixed support of directional light coloring from physical sky in path tracing.</p></li>
<li><p>HDRP: Fixed support of Distortion with MSAA.</p></li>
<li><p>HDRP: Fixed support of multi-editing on custom pass volumes.</p></li>
<li><p>HDRP: Fixed TAA upsampling algorithm, now work properly.</p></li>
<li><p>HDRP: Fixed TAA upsampling algorithm, now work properly.</p></li>
<li><p>HDRP: Fixed tessellation displacement with planar mapping.</p></li>
<li><p>HDRP: Fixed texture fields for volume parameters accepting textures with wrong dimensions.</p></li>
<li><p>HDRP: Fixed the APV UI loosing focus when the helpbox about baking appears in the probe volume.</p></li>
<li><p>HDRP: Fixed the auto-exposure mismatch between sky background and scene objects in path tracing.</p></li>
<li><p>HDRP: Fixed the behavior the max ray length for recursive rendering to match RTR and rasterization.</p></li>
<li><p>HDRP: Fixed the cloudlayer not using depth buffer.</p></li>
<li><p>HDRP: Fixed the clouds missing in the ambient probe and in the static and dynamic sky.</p></li>
<li><p>HDRP: Fixed the clouds not taking properly into account the fog when in distant mode and with a close far plane. (<a href="https://issuetracker.unity3d.com/issues/volumetric-clouds-very-low-camera-far-plane-results-in-fog-not-being-rendered-properly-in-front-of-non-local-clouds">1367993</a>)</p></li>
<li><p>HDRP: Fixed the default custom pass buffer format from R8G8B8A8_SNorm to R8G8B8A8_UNorm. Additionally, an option in the custom pass buffer format settings is available to use the old format.</p></li>
<li><p>HDRP: Fixed the default number of physically based sky bounce to be 3.</p></li>
<li><p>HDRP: Fixed the default value of "Distortion Blur" from 1 to 0 according to the doc.</p></li>
<li><p>HDRP: Fixed the dependency between transparent SSR and transparent depth prepass being implicit. (1365915)</p></li>
<li><p>HDRP: Fixed the emissive being overriden by ray traced sub-surface scattering.</p></li>
<li><p>HDRP: Fixed the error thrown when layered lit material has an invalid material type.</p></li>
<li><p>HDRP: Fixed the incorrect value written to the VT feedback buffer when VT is not used.</p></li>
<li><p>HDRP: Fixed the issue where an attempt to build and run a HDRP project for the first time, caused an error. (<a href="https://issuetracker.unity3d.com/issues/hdrp-editor-crashes-when-building-project-using-build-and-run-for-the-second-time">1417508</a>)</p></li>
<li><p>HDRP: Fixed the option to force motion blur off when in XR.</p></li>
<li><p>HDRP: Fixed the performance of the volumetric clouds in non-local mode when large occluders are on screen.</p></li>
<li><p>HDRP: Fixed the point distribution for the diffuse denoiser sometimes not being properly intialized.</p></li>
<li><p>HDRP: Fixed the possibility to hide custom pass from the create menu with the HideInInspector attribute.</p></li>
<li><p>HDRP: Fixed the ray tracing acceleration structure build marker not being included in the ray tracing stats.</p></li>
<li><p>HDRP: Fixed the ray tracing fallbacks being broken since an Nvidia Driver Update.</p></li>
<li><p>HDRP: Fixed the rendering order of decals that have a similar draw order value.</p></li>
<li><p>HDRP: Fixed the rt screen space shadows not using the correct asset for allocating the history buffers.</p></li>
<li><p>HDRP: Fixed the RTAO debug view being broken.</p></li>
<li><p>HDRP: Fixed the sun leaking from behind fully opaque clouds.</p></li>
<li><p>HDRP: Fixed the volume not being assigned on some scene templates.</p></li>
<li><p>HDRP: Fixed the volumetric clouds cloud map not being centered over the world origin.</p></li>
<li><p>HDRP: Fixed the volumetric clouds debug view not taking into account the exposure and leading to Nans. (1365054)</p></li>
<li><p>HDRP: Fixed the volumetric clouds for the indoor template scenes by disabling them (normal and DXR).</p></li>
<li><p>HDRP: Fixed the way we are handling emissive for SSGI/RTGI/Mixed and APV and remove ForceForwardEmissive code.</p></li>
<li><p>HDRP: Fixed Tile/Cluster Debug in the Rendering Debugger for Decal and Local Volumetric Fog.</p></li>
<li><p>HDRP: Fixed tiled artifacts in refraction at borders between two reflection probes.</p></li>
<li><p>HDRP: Fixed tooltip not showing on labels in ShaderGraphs. (1358483)</p></li>
<li><p>HDRP: Fixed Transparent Depth Pre/Post pass by default for the built-in HDRP Hair shader graph.</p></li>
<li><p>HDRP: Fixed undo on light anchor.</p></li>
<li><p>HDRP: Fixed unsupported material properties show when rendering pass is Low Resolution.</p></li>
<li><p>HDRP: Fixed using the wrong coordinate to compute the sampling direction for the screen space global illumination.</p></li>
<li><p>HDRP: Fixed using the wrong directional light data for clouds and the definition of current Sun when the shadow pass is culled.</p></li>
<li><p>HDRP: Fixed various issues with render graph viewer when entering playmode.</p></li>
<li><p>HDRP: Fixed vertex color mode Add name whicgh was misleading, renamed to AddSubstract.</p></li>
<li><p>HDRP: Fixed Vertex Color Mode documentation for layered lit shader.</p></li>
<li><p>HDRP: Fixed VFX flag "Exclude From TAA" not working for some particle types.</p></li>
<li><p>HDRP: Fixed VfX lit particle AOV output color space.</p></li>
<li><p>HDRP: Fixed volume interpolation issue with ScalableSettingLevelParameter.</p></li>
<li><p>HDRP: Fixed volumetric clouds in lens flares sample indoor scene by disabling it.</p></li>
<li><p>HDRP: Fixed Volumetric Clouds not updated when using RenderTexture as input for cloud maps.</p></li>
<li><p>HDRP: Fixed volumetric fog in planar reflections.</p></li>
<li><p>HDRP: Fixed warning "Releasing render texture that is set to be RenderTexture.active!" on pipeline disposal / hdrp live editing.</p></li>
<li><p>HDRP: Fixed warning when an APV baking set is renamed.</p></li>
<li><p>HDRP: Fixed white flash when camera is reset and SSR Accumulation mode is on.</p></li>
<li><p>HDRP: Fixed white flashes when history is reset due to changes on type of upsampler.</p></li>
<li><p>HDRP: Fixed wobbling/tearing-like artifacts with SSAO.</p></li>
<li><p>HDRP: Fixed write to VT feedback in debug modes.</p></li>
<li><p>HDRP: Fixed wrong LUT initialization in Wireframe mode.</p></li>
<li><p>HDRP: Fixed wrong ordering in FrameSettings (Normalize Reflection Probes).</p></li>
<li><p>HDRP: Fixed Z axis orientation when sampling 3D textures in local volumetric fog.</p></li>
<li><p>HDRP: HDRP Wizard can still be opened from Windows &gt; Rendering, if the project is not using a Render Pipeline.</p></li>
<li><p>HDRP: Indentation of the HDRenderPipelineAsset inspector UI for quality.</p></li>
<li><p>HDRP: Maximum light count per fine prunned tile (opaque deferred) is now 63 instead of 23.</p></li>
<li><p>HDRP: Prevent user from spamming and corrupting installation of nvidia package.</p></li>
<li><p>HDRP: Reduced the number shader variants for the volumetric clouds.</p></li>
<li><p>HDRP: Render Graph object pools are now cleared with render graph cleanup.</p></li>
<li><p>HDRP: Significantly improved performance of APV probe debug.</p></li>
<li><p>HDRP: The HDRP Wizard is only opened when a SRP in use is of type HDRenderPipeline.</p></li>
<li><p>HDRP: When the HDProjectSettings was being loaded on some cases the load of the ScriptableObject was calling the method <code>Reset</code> from the HDProjectSettings, simply rename the method to avoid an error log from the loading.</p></li>
<li><p>IL2CPP: Added missing facade dlls (System.Memory System.Buffers...) to the Unity 4.8 reference profile.</p></li>
<li><p>IL2CPP: Android will now properly build when Windows Language is set to Turkish.</p></li>
<li><p>IL2CPP: Fixed exported Android project failure. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-android-build-fails-when-building-an-exported-project-on-android-studio-with-script-debugging-enabled">1373278</a>)</p></li>
<li><p>IMGUI: Added rounding to get pixels to align better when the scale is not 1 to 1. (1309132)</p></li>
<li><p>IMGUI: Fixed an issue where FoldoutHeader group does not show error when they are nested. (<a href="https://issuetracker.unity3d.com/issues/first-list-in-a-foldoutheadergroup-errors">1344968</a>)</p></li>
<li><p>IMGUI: Fixed an issue where the gradient color fields gets dark in Playmode. (<a href="https://issuetracker.unity3d.com/issues/playmode-tint-some-colors-in-gradient-editor-are-affected-by-playmode-tint-some-not">803349</a>)</p></li>
<li><p>IMGUI: Fixed GameObject and Folder icons become pixelated when Quality Levels are deleted and Texture Quality is set to Eight Res. (<a href="https://issuetracker.unity3d.com/issues/gameobject-and-folder-icons-become-pixelated-when-quality-levels-are-deleted-and-texture-quality-is-set-to-eight-res">1249745</a>)</p></li>
<li><p>IMGUI: Fixed incorrect calculation of Handles when drawn in the Editor Window. (<a href="https://issuetracker.unity3d.com/issues/handles-dot-slider2d-does-not-respond-to-mouse-input-when-dragged-in-the-editor-window">1338039</a>)</p></li>
<li><p>IMGUI: Fixed Lighting window label is clipped when there is plenty space. (1342233)</p></li>
<li><p>IMGUI: Fixed memory leak when continuously calling Repaint inside OnGUI after GUI.Window. (<a href="https://issuetracker.unity3d.com/issues/memory-leak-when-continuously-calling-repaint-inside-ongui-after-gui-dot-window">1347653</a>)</p></li>
<li><p>IMGUI: Fixed the Preview window does not open when Ctrl+Clicked on object field icon. (<a href="https://issuetracker.unity3d.com/issues/the-preview-window-does-not-open-when-ctrl-plus-clicked-on-parameter-icon">1353928</a>)</p></li>
<li><p>IMGUI: When reordering an item in a ReorderableList, keep the expanded state of the item and its children. (<a href="https://issuetracker.unity3d.com/issues/items-change-expanded-slash-collapsed-states-when-changing-the-order-of-them-in-a-reorderable-list">1335323</a>)</p></li>
<li><p>Input: Fixed InputSystem.QueueStateEvent throwing exceptions when called from non-main thread. (<a href="https://issuetracker.unity3d.com/issues/inputsystem-new-inputsystem-queuestateevent-cannot-be-called-from-another-thread">1348778</a>)</p></li>
<li><p>Input: Fixed PrintScreen key reported as pressed when pressing Insert/Home/Del/etc with NumLock being off with Input System package on Windows (also modified UWP and GDK). (<a href="https://issuetracker.unity3d.com/issues/certain-input-system-keys-trigger-prtscn-with-either-numlock-on-or-off">1359217</a>)</p></li>
<li><p>Input System: Any unhandled exception in <code>InputManager.OnUpdate</code> failing latter updates with <code>InvalidOperationException: Already have an event buffer set! Was OnUpdate() called recursively?</code>. Instead the system will try to handle the exception and recover into a working state.</p></li>
<li><p>Input System: Fixed a problem where only using runtimes that are not XR supported causes a compile error. This fix adds back in ENABLE_VR checks to prevent this issue.</p></li>
<li><p>Installer: Removed unnecessary data from templates installed by the editor installer, making Unity installs smaller by over 800MB.</p></li>
<li><p>iOS: Changed the default audio output frequency to 48KHz, instead of 24KHz. (<a href="https://issuetracker.unity3d.com/issues/ios-audio-audiosource-dot-getspectrumdata-returns-incorrect-data">1354046</a>)</p></li>
<li><p>iOS: Fixed a crash when the iPhone 12 family were forced to portrait upside down. (<a href="https://issuetracker.unity3d.com/issues/ios-application-crashes-when-switching-orientation-to-reverse-portrait-after-switching-it-to-non-default-app-orientation">1357577</a>)</p></li>
<li><p>iOS: Fixed an issue that the iOS Simulator crashing an app when the <code>Strip Engine Code</code> is turned on. (1190185)</p></li>
<li><p>iOS: Fixed graphics memory not being freed on unity unload. (<a href="https://issuetracker.unity3d.com/issues/uaal-metal-graphic-resources-allocated-in-the-scene-are-not-released-upon-unloading-the-scene-when-using-metal">1348481</a>)</p></li>
<li><p>iOS: Metal: fixed disabling stencil completely in case of Comparison Function being Disabled, as the "write only" is perfectly valid stencil state (case 1345523). (<a href="https://issuetracker.unity3d.com/issues/stencil-compare-operation-disabled-behaves-as-always-when-not-using-metal-as-the-graphics-api">1345523</a>)</p></li>
<li><p>Kernel: Fixed an issue where Boot.config was not written when there was no data in the file.</p></li>
<li><p>Kernel: Registering undo operations that don't affect the scene will no longer mark the scene as dirty. (<a href="https://issuetracker.unity3d.com/issues/undo-dot-registerobject-or-undo-dot-createobject-dirties-the-scene-but-no-actual-changes-to-scene-are-made">1306519</a>)</p></li>
<li><p>License: Extend IPC channel name maximum length.</p></li>
<li><p>License: Fixed a bug on Windows where the operating system was not detected properly<br> License: Fixed a bug where duplicate configurations would not allow Licensing Client to start properly<br>
License: Fixed a bug where remote configuration was not getting downloaded<br>
License: Ensuring ULF license directory exists on MacOS and Linux<br>
License: Improve performance for updating local configuration on Linux.</p></li>
<li><p>License: Fixed Licensing Client signature check in the Editor.</p></li>
<li><p>License: Forced a relaunch of the license client if a connection is refused on pipe.</p></li>
<li><p>Linux: Editor: Fix GLX context creation when using nvidia prime render offloading.</p></li>
<li><p>Linux: Fixed an issue where the Assets menu might be disabled after using the right-click context menu.</p></li>
<li><p>Linux: Fixed exception caused by EmbeddedLinuxPreProcessor, by only executing checks when EmbeddedLinux platform is selected<br> Fixes the removal of unneeded EmbeddedLinux support files (e.g. unstripped debug symbols), to minimize the resulting archive size.</p></li>
<li><p>Linux: Fixed not being able to drag undocked window tabs across monitor boundaries. (<a href="https://issuetracker.unity3d.com/issues/linux-cant-drag-tabs-across-window-boundaries-from-one-container-window-to-another">1333992</a>)</p></li>
<li><p>Linux: Fixed versioned Linux libraries are ignored by the Editor when they are imported. (<a href="https://issuetracker.unity3d.com/issues/versioned-linux-libraries-are-ignored-by-the-editor-when-they-are-imported">1345105</a>)</p></li>
<li><p>Linux: Like on Windows, mouse movement will now wrap around the screen edges for certain GUI elements that rely on mouse deltas (i.e. Rotate tool). (<a href="https://issuetracker.unity3d.com/issues/linux-cursor-movement-limited-to-screen-edges">1156952</a>)</p></li>
<li><p>Linux: Prevent crash when closing the standalone profiler on Linux. (1343811)</p></li>
<li><p>Linux: Removed Ctrl+Q as a shortcut to close the Linux editor. (1367175)</p></li>
<li><p>macOS: Fixed a bug where Mac standalone player builds would fail if using a custom icon and building an Xcode project.</p></li>
<li><p>macOS: Fixed InputFields share composition string on macOS builds when using IME. (<a href="https://issuetracker.unity3d.com/issues/input-fields-share-input-on-macos-builds-when-using-the-kana-japanese-keyboard-layout">1345917</a>)</p></li>
<li><p>macOS: Fixed invalid generated xcode projects when the product name has non-ascii characters. (<a href="https://issuetracker.unity3d.com/issues/ios-xcode-project-generated-with-product-name-containing-chinese-characters-cannot-be-opened-due-to-parse-errors">1347730</a>)</p></li>
<li><p>macOS: Fixed mouse delta values are generated after mouse click while the cursor is motionless. (<a href="https://issuetracker.unity3d.com/issues/mac-mouse-delta-values-are-generated-after-mouse-click-while-the-cursor-is-motionless">1194673</a>)</p></li>
<li><p>macOS: Maintain previous window position when reopening player on MacOS. (1333806)</p></li>
<li><p>Mobile: Fixed an issue with web scripting ANRs when C# callbacks take long to execute. (<a href="https://issuetracker.unity3d.com/issues/android-app-becomes-unresponsive-and-crashes-with-anr-errors">1374426</a>)</p></li>
<li><p>Mobile: Updated the Xcode version used to build the PhysX libraries in order to fix the "Ignoring invalid debug info" warnings when archiving a Unity project in Xcode. (<a href="https://issuetracker.unity3d.com/issues/xcode-11-dot-4-linker-emits-ignoring-invalid-debug-info-warnings-when-archiving-a-unity-project">1233645</a>)</p></li>
<li><p>Mono: Fixed crash that would occur after calling Marshal.GetCCW. (<a href="https://issuetracker.unity3d.com/issues/freeze-slash-crash-on-dllcanunloadnow-when-compiling-while-reading-a-file">1351182</a>)</p></li>
<li><p>Mono: Fixed the root cause behind "The type initializer for 'Sys' threw an exception." when running the editor on Apple silicon devices. (<a href="https://issuetracker.unity3d.com/issues/m1-webgl-editor-throws-errors-when-building-for-webgl-on-native-apple-silicon-editor">1399524</a>)</p></li>
<li><p>Mono: Raise exception rather than crashing when calling Marshal.GetFunctionPointerForDelegate with a delegate that cannot be marshalled. (<a href="https://issuetracker.unity3d.com/issues/burstcompile-attribute-causes-crash-on-compile">1343949</a>)</p></li>
<li><p>Mono: Safely interrupt the GC finalize thread on shutdown. (<a href="https://issuetracker.unity3d.com/issues/quitting-the-player-that-has-a-lot-of-alive-objects-with-finalizers-results-in-a-crash">1363998</a>)</p></li>
<li><p>Multiplayer: Marked uNET HLAPI as deprecated.</p></li>
<li><p>N/A (internal): Fixed build for embeddedlinnux<br> Port fixes from 2020.3 for embedded linux to trunk.</p></li>
<li><p>N/A (internal): Re-enabled ShaderImporterTest ImportShader_FromEmbeddedPackage_WithInclude_InRelativeDirectory_IsImported. (1278035)</p></li>
<li><p>N/A (internal): Test no longer rely on ordering of merging prefabs when loading a scene. (1349135)</p></li>
<li><p>Networking: Fixed crash when a dedicated server tries to load an audio clip on startup. (<a href="https://issuetracker.unity3d.com/issues/dedicated-server-player-crashes-on-complex-hdrp-project">1354359</a>)</p></li>
<li><p>Package: (Recorder) Do not perform the color space conversion from linear to sRGB for RenderTextures that are already sRGB.</p></li>
<li><p>Package: (Recorder) Ensure that the color space conversion from sRGB to linear is performed when required for EXR files.</p></li>
<li><p>Package: (Recorder) Fixed an exception that occurred when sending a RenderTexture to a Recorder before creating this RenderTexture.</p></li>
<li><p>Package: (Recorder) Fixed issues with the Recorder samples about synchronizing multiple recordings and resetting the Game view resolution.</p></li>
<li><p>Package: [Recorder] Fix vertically flipped outputs on OpenGL hardware.</p></li>
<li><p>Package: [Recorder] Perform the appropriate color space conversion for Texture Sampling sources when required.</p></li>
<li><p>Package: [Visual Scripting] Fixed an issue where uncaught exceptions were thrown in Debug builds of the Windows editor.  Fixed custom units not appearing in the finder.</p></li>
<li><p>Package Manager: Added a limit to the description for Asset store packages in the editor. (1346719)</p></li>
<li><p>Package Manager: Added info box informing users that an Asset is hidden when viewing it in My Assets.</p></li>
<li><p>Package Manager: Added missing filters capability to My Registries view. (1409395)</p></li>
<li><p>Package Manager: Added Sample Descriptions to the Package Details UI.</p></li>
<li><p>Package Manager: Added tooltip on unlock icon. (1375779)</p></li>
<li><p>Package Manager: An info icon will warn users when the package version they are using is not recommended for their Unity version.</p></li>
<li><p>Package Manager: Asset Store package release details are not cleaned-up. (<a href="https://issuetracker.unity3d.com/issues/asset-description-doesnt-match-manifest-when-opened-in-package-manager">1354850</a>)</p></li>
<li><p>Package Manager: Confusing package type in the inspector must be removed. (<a href="https://issuetracker.unity3d.com/issues/remove-confusing-message-from-pcakage-inspector-window-this-package-and-all-its-assets-will-be-dot-dot-dot">1298092</a>)</p></li>
<li><p>Package Manager: Dependency packages are no longer missing from the Feature dependencies list. (<a href="https://issuetracker.unity3d.com/issues/feature-sets-adaptive-performance-is-invisible-in-the-mobile-feature-set">1341060</a>)</p></li>
<li><p>Package Manager: Dragging and dropping Assets in projects that reference the package that they are part of (i.e. most projects that are used to test packages within Unity) will now move the Assets instead of copying them.</p></li>
<li><p>Package Manager: Embedded packages are not shown as installed in the Package Manager. (<a href="https://issuetracker.unity3d.com/issues/embedded-packages-are-not-shown-as-installed-in-the-package-manager">1352772</a>)</p></li>
<li><p>Package Manager: Errors are now automatically refreshed once packages are updated to fix the issue. (1342141)</p></li>
<li><p>Package Manager: Export package window does not update with new content. (<a href="https://issuetracker.unity3d.com/issues/exporting-package-window-doesnt-update-when-trying-to-open-it-again-after-selecting-a-different-asset">1337283</a>)</p></li>
<li><p>Package Manager: Features labeled as released should not contain pre-release packages. (<a href="https://issuetracker.unity3d.com/issues/package-manager-feature-sets-are-marked-as-release-even-when-they-contain-pre-release-packages">1344818</a>)</p></li>
<li><p>Package Manager: Fixed a bug where the manifest edit button did not work on a newly embedded package when Asset Pipeline Auto Refresh is off. (1396392)</p></li>
<li><p>Package Manager: Fixed a NullReferenceException thrown when user selects a feature set that contains a package, not discoverable in Editor manifest, in the list of included packages. (1381677)</p></li>
<li><p>Package Manager: Fixed a small memory leak. (<a href="https://issuetracker.unity3d.com/issues/tls-allocator-alloc-temp-tls-after-opening-asset-store-window">1396779</a>)</p></li>
<li><p>Package Manager: Fixed an issue in multi-selection mode where it was previously impossible to remove custom packages. (1382259)</p></li>
<li><p>Package Manager: Fixed an issue where having package folders without a package manifest in the project's Library folder would fail resolving <code>local-tarball</code> or <code>git</code> packages.</p></li>
<li><p>Package Manager: Fixed an issue where in "My Assets" tab, some package thumbnails lead to wrong target URLs.</p></li>
<li><p>Package Manager: Fixed an issue where JSON files encoded using UTF-8 with BOM could not be parsed.</p></li>
<li><p>Package Manager: Fixed an issue where package metadata would be fetched even though the locally cached metadata was up-to-date.</p></li>
<li><p>Package Manager: Fixed an issue where <code>local-tarball</code> dependencies would become unresolved if the source tarball was removed.</p></li>
<li><p>Package Manager: Fixed backslashes not always being displayed correctly. (1384378)</p></li>
<li><p>Package Manager: Fixed bug where having a package which can't be found shows it as a Unity Technologies package available in the Unity Registry. (1348573)</p></li>
<li><p>Package Manager: Fixed issue where Enter key is not working when user tries to add a package by name or by GIT url in Package Manager window. (<a href="https://issuetracker.unity3d.com/issues/a-package-cant-be-added-by-git-url-and-by-name-when-clicking-enter">1393395</a>)</p></li>
<li><p>Package Manager: Fixed issue where package actions remain disabled if installing a package and going to play mode right after. (1341873)</p></li>
<li><p>Package Manager: Fixed issue where Package Manager GIT URL entry does not strip leading/trailing spaces. (1322420)</p></li>
<li><p>Package Manager: Fixed issue where Package Manager UI goes all black for a brief moment after an UPM resolve operation,. (1365389)</p></li>
<li><p>Package Manager: Fixed spacing in Package Manager from "Dev Ops" to "DevOps".</p></li>
<li><p>Package Manager: Fixed Test_Serializable_Objects_SurviveDomainReload test. (1306124)</p></li>
<li><p>Package Manager: Fixed the issue where assets don't refresh properly when user signs out and sign back in. (1376327)</p></li>
<li><p>Package Manager: Fixed the issue where CheckUpdate calls does not end for disabled packages. (1394243)</p></li>
<li><p>Package Manager: Fixed the issue where copy paste keyboard shortcut does not work in the search box on <code>My Assets</code> tab. (1357462)</p></li>
<li><p>Package Manager: Fixed the issue where the search bar in the Package Manager window gets out of focus frequently when user type slowly. (1348902)</p></li>
<li><p>Package Manager: Fixed the issue where <code>subscription based</code> filter shows when there are not packages with entitlements. (1399520)</p></li>
<li><p>Package Manager: Fixed the package state icon not changing correctly after a download from the Asset Store. (<a href="https://issuetracker.unity3d.com/issues/packman-my-assets-icons-are-not-updated-upon-downloading-the-assets">1384683</a>)</p></li>
<li><p>Package Manager: Fixed the target version of the update button not suggesting the correct version. (1410189)</p></li>
<li><p>Package Manager: Fixed UnityPackageManager process leaving dangling IPC socket file after it exited.</p></li>
<li><p>Package Manager: Null Exception thrown when an Asset had an update available is fixed. (1357085)</p></li>
<li><p>Package Manager: Package installed checkmark hardly noticeable in Light theme. (1348248)</p></li>
<li><p>Package Manager: Packages in error no longer disappear from list on resolve. (1343734)</p></li>
<li><p>Package Manager: Refreshed package version list when enabling pre-release packages in use or when updating package version.</p></li>
<li><p>Package Manager: Removed 'Recommended' label from packages in scoped registries. Users will now see 'Latest update' on the latest version for those packages instead.</p></li>
<li><p>Package Manager: Removed extra fetch calls after Package Manager resolve. Should fix some Package Manager unit test instabilities.</p></li>
<li><p>Package Manager: Removed update button to the Unity Registry version of a package if this package is embedded or locally installed. (1354198)</p></li>
<li><p>Package Manager: The list of Samples in Package Details is expanded by default.</p></li>
<li><p>Particles: A warning will now be shown when attempting to assign a ParticleSystem as a sub-emitter when it is not a child and is part of a Prefab hierarchy. (<a href="https://issuetracker.unity3d.com/issues/errors-are-thrown-and-sub-emitter-is-not-reparented-when-trying-to-reparent-sub-emitters-of-prefabs">1306311</a>)</p></li>
<li><p>Particles: Added sub-frame emission precision for Bursts. (<a href="https://issuetracker.unity3d.com/issues/particle-system-does-not-emit-until-a-fixed-timestep-has-passed">1352736</a>)</p></li>
<li><p>Particles: Fixed crashes if accessing specific properties in uninitialized Collision and Trigger modules from script.</p></li>
<li><p>Particles: Fixed cycles and frame over time to work together correctly in the Texture Sheet Animation module. (<a href="https://issuetracker.unity3d.com/issues/texturesheetanimation-loops-through-all-frames-when-cycles-is-set-to-2-or-more-and-frameovertime-upper-frame-limit-is-not-max">1338814</a>)</p></li>
<li><p>Particles: Fixed errors when viewing a Force Field Preset inspector whilst entering Playmode. (<a href="https://issuetracker.unity3d.com/issues/particlesystemforce-errors-are-thrown-on-accessing-preset-when-particlesystemforce-is-deleted">1318951</a>)</p></li>
<li><p>Particles: Fixed prefab override tooltip for Particle Systems. (1267018)</p></li>
<li><p>Physics: Anchored prismatic limit handles in screen space to avoid them occluding small Articulation Body links.</p></li>
<li><p>Physics: Character controller will no longer snap downwards when hitting a step wall that is just outside of the step offset reach. (<a href="https://issuetracker.unity3d.com/issues/character-controller-snaps-downwards-when-the-height-needed-to-step-on-a-gameobject-is-bigger-than-the-step-offset-value">1256900</a>)</p></li>
<li><p>Physics: Clamped the Articulation body drive lower and upper limits to each other. (<a href="https://issuetracker.unity3d.com/issues/articulation-body-joint-motion-lower-limit-and-upper-limit-are-not-clamped">1310004</a>)</p></li>
<li><p>Physics: Enabled loading the baked physx meshes from disk while running in Editor (before this change an expensive bake operation was required). (<a href="https://issuetracker.unity3d.com/issues/excessive-editor-load-time-for-scenes-using-asset-bundles-which-contain-high-poly-mesh-colliders">1104237</a>)</p></li>
<li><p>Physics: Ensure that when resetting the 2D Physics Project settings, the setting "Reuse Collision Callbacks" is reset to ON. (1378927)</p></li>
<li><p>Physics: Fixed a crash that happened when resetting the mass properties of a disabled articulation body. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-resetting-center-of-mass-of-disabled-articulationbody-in-runtime">1346489</a>)</p></li>
<li><p>Physics: Fixed a crash when visualising contacts of a scene that's being unloaded. (<a href="https://issuetracker.unity3d.com/issues/physics-debugger-sometimes-crashes-when-visualising-contacts-of-a-scene-thats-being-unloaded">1390350</a>)</p></li>
<li><p>Physics: Fixed a race condition which could ultimately cause random crashes inside cloth, due to data cleanup overlapping with cloth simulation. (1275123)</p></li>
<li><p>Physics: Fixed a rare issue where multithreaded 2D physics processes some contacts twice. (<a href="https://issuetracker.unity3d.com/issues/spriteshape-with-buoyancy-effector-react-differently-in-build-and-editor">1369087</a>)</p></li>
<li><p>Physics: Fixed capsule overlaps missing low resolution heightmaps. (<a href="https://issuetracker.unity3d.com/issues/physics-dot-overlapcapsule-doesnt-detect-terrain-collider-when-terrain-heightmap-resolution-is-513x513-or-lower">1263649</a>)</p></li>
<li><p>Physics: Fixed ClosesetPointCommand throwing an assert when executing jobs. (1377908)</p></li>
<li><p>Physics: Fixed Hinge Joint ignoring break force and break torque after using useSpring or useMotor. (<a href="https://issuetracker.unity3d.com/issues/hinge-joint-becomes-unbreakable-when-break-force-and-break-torque-are-set-up-before-the-spring">1364352</a>)</p></li>
<li><p>Physics: Fixed Hinge Joints not breaking after calling useSpring or useMotor on the Joint. (<a href="https://issuetracker.unity3d.com/issues/hinge-joint-is-not-destroyed-when-the-joint-breaks">1361452</a>)</p></li>
<li><p>Physics: Fixed invalid Collider parameters causing crashes in PhysX. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-physx-gu-persistentcontactmanifold-reducebatchcontacts-when-entering-play-mode">1340746</a>)</p></li>
<li><p>Physics: Fixed Reset not resetting connected bodies in Joint Inspector.</p></li>
<li><p>Physics: Fixed undefined behaviour when calling Physics.OverlapCapsule over Terrain holes.</p></li>
<li><p>Physics: Unity will no longer crash when multiple overlapping rigidbodies are creating over 65 thousand interaction elements. (<a href="https://issuetracker.unity3d.com/issues/crash-on-physx-sc-elementinteractionmarker-elementinteractionmarker-when-exiting-playmode-with-continous-collision-detection">1328426</a>)</p></li>
<li><p>Physics: Updated documentation on maxLinearVelocity and maxJointVelocity properties. (<a href="https://issuetracker.unity3d.com/issues/articulationbody-dot-maxlinearvelocity-doesnt-limit-velocity-when-forces-are-applied-to-the-articulation-body">1375711</a>)</p></li>
<li><p>Player: Fixed the player outputing "CreateDirectory '' failed: The system cannot find the path specified." error to stdout when using "-logfile" command line parameter with a relative path. (<a href="https://issuetracker.unity3d.com/issues/passing-logfile-argument-to-a-standalone-build-results-in-an-error-message">1343466</a>)</p></li>
<li><p>Prefabs: "Prefab Import Error: Assertion failed on expression: 'm_InstanceID != InstanceID_None'" caused by dangling pointers in broken scenes. (1340955)</p></li>
<li><p>Prefabs: Catch and handle exception if creating a prefab from Asset Menu fails. (<a href="https://issuetracker.unity3d.com/issues/prefab-is-added-to-the-opened-scene-whenever-you-rmb-create-prefab-in-a-folder">1333618</a>)</p></li>
<li><p>Prefabs: Fixed an issue where all descendants on the Prefab Variant would get destroyed after adding the 'Rect Transform' component to the Prefab root. (<a href="https://issuetracker.unity3d.com/issues/all-descendants-on-the-prefab-variant-get-destroyed-after-adding-the-rect-transform-component-to-the-prefab-root">1340595</a>)</p></li>
<li><p>Prefabs: Fixed an issue where Null manager errors were no prevented if GlobalObjectIdentifierToObjectSlow() was called for objects in unloaded scenes. (<a href="https://issuetracker.unity3d.com/issues/error-is-thrown-when-converting-a-globalobjectid-to-an-object-reference-and-the-object-is-in-an-unloaded-scene">1371478</a>)</p></li>
<li><p>Prefabs: Fixed Base Prefab is referenced in Unity Event when making specific revert on Prefab Variant. (<a href="https://issuetracker.unity3d.com/issues/base-prefab-is-referenced-in-unity-event-when-making-specific-revert-on-prefab-variant">1287926</a>)</p></li>
<li><p>Prefabs: Fixed broken scene paths in EditorBuildSettings. (<a href="https://issuetracker.unity3d.com/issues/scenemanager-dot-scenecountinbuildsettings-reports-a-different-numbers-of-scenes-than-there-actually-is-is-the-build-settings">1035848</a>)</p></li>
<li><p>Prefabs: Fixed crash when upgrading scene with nested prefabs. (1389277)</p></li>
<li><p>Prefabs: Fixed DisallowMultipleComponent attribute is ignored in Prefab variants. (<a href="https://issuetracker.unity3d.com/issues/disallowmultiplecomponent-ignored-in-prefab-variants">1370600</a>)</p></li>
<li><p>Prefabs: Fixed exception appears while Prefab Asset replaced by its child. (<a href="https://issuetracker.unity3d.com/issues/improved-prefabs-exception-appears-while-prefab-asset-replaced-by-its-child">1055879</a>)</p></li>
<li><p>Prefabs: Fixed Prefab mode saving too many objects if there are missing nested prefabs. (1339328)</p></li>
<li><p>Prefabs: Fixed Rect tool is enabled for root Prefab in Context mode. Now it behaves similar to the other Transform tools. (<a href="https://issuetracker.unity3d.com/issues/rect-tool-enables-to-move-root-prefab-in-context-mode">1367665</a>)</p></li>
<li><p>Prefabs: Fixed Revert option is not available when right-clicking on the component's 'Enable' checkmark. (<a href="https://issuetracker.unity3d.com/issues/revert-option-is-not-available-when-right-clicked-on-the-prefab-components-enable-checkmark">1364181</a>)</p></li>
<li><p>Prefabs: Fixed RootGameObject detection for missing Prefab instances to avoid creating placeholders.</p></li>
<li><p>Prefabs: Fixed so Prefab Mode have a 'Discard Changes' option like Scenes do in the Hierarchy. (<a href="https://issuetracker.unity3d.com/issues/prefab-mode-does-not-have-discard-changes-like-scenes-do">1369841</a>)</p></li>
<li><p>Prefabs: Fixed that HideFlags are not preserved on dynamically created GameObjects from legacy Prefabs when opened in Prefab Mode. (<a href="https://issuetracker.unity3d.com/issues/hideflags-are-not-respected-on-the-old-prefabs-when-editing-them-on-the-versions-where-old-prefabs-are-deprecated">1151418</a>)</p></li>
<li><p>Prefabs: Fixed undo across Prefab Mode : Child GameObject turned into a prefab on completely unpacking the root prefab. (<a href="https://issuetracker.unity3d.com/issues/prefab-child-gameobject-turns-into-a-prefab-on-completely-unpacking-the-root-prefab">1150192</a>)</p></li>
<li><p>Prefabs: GameObjects added to a prefab instance, which are added after the prefab's children, will remain after the prefab's children even after new children are added to the prefab. (<a href="https://issuetracker.unity3d.com/issues/child-gameobjects-are-added-as-last-in-order-in-a-variant-when-adding-child-gameobjects-to-the-base-prefab">1095995</a>, <a href="https://issuetracker.unity3d.com/issues/prefab-variant-child-has-a-lower-index-than-a-prefab-child-when-editing-a-prefab-while-prefab-variant-is-not-in-the-project">1127653</a>, <a href="https://issuetracker.unity3d.com/issues/adding-children-in-prefab-mode-when-there-are-unapplied-new-gameobject-overrides-causes-the-prefab-to-have-incorrect-structure">1180518</a>)</p></li>
<li><p>Prefabs: Improved performance when entering Prefab Mode in Context for large instances with many overrides. (1370904)</p></li>
<li><p>Prefabs: Make PrefabUtility.GetOriginalSourceRootWhereGameObjectIsAdded() public API. (1367291)</p></li>
<li><p>Prefabs: M_RootOrder is no longer used to determine the sibling order of non-root objects. (<a href="https://issuetracker.unity3d.com/issues/m-rootorder-values-change-in-the-prefab-when-editorutility-dot-setdirty-is-called-on-it">1271887</a>)</p></li>
<li><p>Prefabs: Prefab errors are thrown deleting Prefab instance after making prefab variant and another instance. (<a href="https://issuetracker.unity3d.com/issues/prefab-errors-are-thrown-deleting-prefab-instance-after-making-prefab-variant-and-another-instance">1365373</a>)</p></li>
<li><p>Prefabs: Prefab restructuring rule has been relaxed. It is now possible to add a game object to a prefab instance and position the added objects between the prefabs objects.<br> Objects added to the end of the child list, will now remain at the end, even if children are added to tge prefab.
(<a href="https://issuetracker.unity3d.com/issues/prefab-variant-restructure-rule-is-violated-when-editing-original-prefab">1152758</a>)</p></li>
<li><p>Prefabs: Prevent AddComponent to replace the transform object when called in a callback fired within SetParent. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-adding-a-recttransform-during-the-ontransformparentchanged-callback">1135408</a>)</p></li>
<li><p>Prefabs: Reverting prefab overrides results in "Dangling components have unfulfilled dependencies" error. (<a href="https://issuetracker.unity3d.com/issues/reverting-prefab-overrides-results-in-dangling-components-have-unfulfilled-dependencies-error">1156260</a>)</p></li>
<li><p>Prefabs: The prefab overrides window now has hover effect on items in the TreeView. Also, all items that doesn't have any overrides are now rendered greyed out in order for the items that have have overrides to stand out. (1365985)</p></li>
<li><p>Prefabs: Users can now remove unused non-default overrides on selected Prefab Instances from context menus in the Scene Hierarchy and from a popup in the Prefab Overrides Window. Details are logged to the Console for small numbers of removals. The operation also removes any invalid overrides caused by removed components. (<a href="https://issuetracker.unity3d.com/issues/unused-prefab-data-not-being-cleaned-when-removing-script-through-override">1282612</a>, <a href="https://issuetracker.unity3d.com/issues/old-versions-prefabs-have-transforms-overrides-shown-after-upgrade-to-a-new-version">1339099</a>)</p></li>
<li><p>Profiler: Fixed Asset Loading profiler module not sorting correctly. (1369190)</p></li>
<li><p>Profiler: Fixed Command line diagnostic switch configurations are not passed on to Profiler (Standalone Process) started from the Editor. (1348776)</p></li>
<li><p>Profiler: Fixed fade for non-current samples on Timeline view. (1350111)</p></li>
<li><p>Profiler: Fixed failing ProfilerRecorder test on Android. (1320036)</p></li>
<li><p>Profiler: Fixed incorrect DrawProcedural stat recording. (1327657)</p></li>
<li><p>Profiler: Fixed invalid Main Thread time in Frame Timing Manager on WebGL. (1377253)</p></li>
<li><p>Profiler: Fixed invalid time reported by ProlfierRecorder for Main Thread root marker. (<a href="https://issuetracker.unity3d.com/issues/incorrect-main-thread-marker-time-reported-to-profilerrecorder-whilst-profiler-is-recording">1337020</a>)</p></li>
<li><p>Profiler: Fixed issue where the CPU chart tooltips could be incorrectly calculated. (<a href="https://issuetracker.unity3d.com/issues/profiler-animator-dot-writejob-time-in-cpu-usage-chart-is-two-times-longer-than-shown-in-timelines-main-threads-total">1341423</a>)</p></li>
<li><p>Profiler: Fixed Mesh buffers debug markup availability on vulkan.</p></li>
<li><p>Profiler: Fixed native plugins API create category function to return a new category. (1338385)</p></li>
<li><p>Profiler: Fixed player name label width in Player Connection dropdown to accommodate long strings. Fixed player name reported in Console window on connection to be consistent with Player Connection dropdown. Values in columns will now truncate with elipses if they are too large too fit in the column. When a player is selected the dropdown will now close to mimic the old dropdown behaviour.</p></li>
<li><p>Profiler: Fixed ProfilerRecorder GPU capture on DirectX 12 always returns zeroes. (1345021)</p></li>
<li><p>Profiler: Periodic update of counter values now display correctly in Profiler charts. (1373263)</p></li>
<li><p>Profiler: The profiler will no longer disconnect when the last connected IP is clicked on a second time. (<a href="https://issuetracker.unity3d.com/issues/profiler-clicking-on-the-ip-address-in-the-attach-to-player-menu-for-a-2nd-time-closes-the-connection">1322548</a>)</p></li>
<li><p>Profiler: Toolbar buttons will now no longer be hidden when the profiler window is made too small while undocked. (<a href="https://issuetracker.unity3d.com/issues/standalone-profiler-window-can-be-shrunk-to-the-point-where-some-top-menu-options-become-hidden">1365575</a>)</p></li>
<li><p>Project Browser: Added support to drag and drop package root folders onto an ObjectField. (<a href="https://issuetracker.unity3d.com/issues/folders-in-packages-folder-cannot-be-added-to-object-fields-since-they-cannot-be-dragged">1335319</a>)</p></li>
<li><p>Project Browser: Fixed an issue where sort order of assets in Project Browser is different from Asset picker. (<a href="https://issuetracker.unity3d.com/issues/object-picker-order-is-from-file-order-in-project-window">1328148</a>)</p></li>
<li><p>Project Browser: Fixed empty folder icon in Project Browser is smaller on a 4k display. (<a href="https://issuetracker.unity3d.com/issues/empty-folder-icon-in-project-browser-is-smaller-on-a-4k-display">1375981</a>)</p></li>
<li><p>Project Browser: Fixed text alignment in Delete assets dialog. (1296099)</p></li>
<li><p>Project Browser: Shader subassets thumbnails are not displayed. (1372478)</p></li>
<li><p>Scene Manager: Fixed an issue where -openscene command line argument didn't open scenes when using -batchmode. (<a href="https://issuetracker.unity3d.com/issues/no-scenes-are-opening-when-using-batchmode">1249100</a>)</p></li>
<li><p>Scene Manager: Fixed argument exception is thrown when double-clicking on the DontDestroyOnLoad scene. (<a href="https://issuetracker.unity3d.com/issues/scene-management-argument-exception-is-thrown-when-double-clicking-on-the-dontdestroyonload-scene">1283407</a>)</p></li>
<li><p>Scene Manager: Fixed parenting isn't displayed in the Hierarchy after loading a specific custom layout. (<a href="https://issuetracker.unity3d.com/issues/no-parenting-displayed-in-hierarchy-when-loading-a-custom-layout">1346524</a>)</p></li>
<li><p>Scene Manager: Fixed performance regression in SetByInstanceID. (1353323)</p></li>
<li><p>Scene Manager: Fixed that loading multiple scenes additively via "Assets/Open Scene Additive" menu item loaded them in random order than as seen in the Project Window. (<a href="https://issuetracker.unity3d.com/issues/loading-multiple-scenes-additively-loads-them-in-random-order-than-as-seen-in-the-project-window">1323868</a>)</p></li>
<li><p>Scene Manager: Fixed that moving a GameObject to a unloading scene on the 'sceneUnloaded' event is possible, and leaves the object without valid scene. An exception is now thrown. (<a href="https://issuetracker.unity3d.com/issues/move-game-object-to-unloaded-scene-on-scene-unloaded-callback-is-possible-and-leaves-the-object-without-valid-scene">923322</a>)</p></li>
<li><p>Scene Manager: OpenScene invoked within a SceneClosed or SceneClosing callback, on the same scene that is being closed, will return error. (<a href="https://issuetracker.unity3d.com/issues/opening-same-scene-on-sceneclosed-callback-does-not-add-it-to-scene-manager">902638</a>)</p></li>
<li><p>Scene Manager: Removed duplicate adjacent separators in scene paths before building player. (<a href="https://issuetracker.unity3d.com/issues/using-double-forward-slashes-in-paths-when-building-player-causes-loadscene-and-unloadscene-to-fail-with-correct-paths">1250807</a>)</p></li>
<li><p>Scene/Game View: Fixed a case where gizmo enabled state could potentially get out of sync with Inspector foldout state. (<a href="https://issuetracker.unity3d.com/issues/ondrawgizmos-is-called-from-a-collapsed-script-after-restarting-the-editor">1331034</a>)</p></li>
<li><p>Scene/Game View: Fixed deprecates current <code>Handles.FreeMoveHandle</code> signatures and introduces new ones that do not take a <code>Quaternion rotation</code> parameter. (<a href="https://issuetracker.unity3d.com/issues/handles-dont-rotate-when-using-handles-dot-freemovehandle">1370210</a>)</p></li>
<li><p>Scene/Game View: Fixed errors when exiting play mode with a tool for a non-serialized component active. (<a href="https://issuetracker.unity3d.com/issues/missingreferenceexception-when-exiting-play-mode-while-bound-editing-gizmo-is-active-for-a-collider-that-was-added-at-runtime">1322944</a>)</p></li>
<li><p>Scene/Game View: Fixed extraneous <code>EditorApplication.playModeStateChanged</code> callbacks when setting <code>EditorApplication.isPlaying</code> to false in an <code>ExitEditMode</code> state change callback. (<a href="https://issuetracker.unity3d.com/issues/if-condition-in-editorapplication-dot-playmodestatechanged-callback-is-ignored-for-a-loop-when-entering-play-mode">1348250</a>)</p></li>
<li><p>Scene/Game View: Fixed GameView update with HideFlags.DontSave objects. (<a href="https://issuetracker.unity3d.com/issues/game-view-does-not-update-when-camera-is-flagged-as-hideflag-dot-dontsave">1351075</a>)</p></li>
<li><p>Scene/Game View: Fixed gizmos not rendering in scenes that are loaded during play mode from user code. (<a href="https://issuetracker.unity3d.com/issues/ondrawgizmos-is-not-called-if-game-object-is-in-an-additive-scene-and-draw-gizmos-is-enabled-on-the-game-view">1327723</a>)</p></li>
<li><p>Scene/Game View: Fixed horizontal toolbar elements not displaying text. (<a href="https://issuetracker.unity3d.com/issues/overlays-toolbar-ui-elements-show-their-text-only-in-panel-mode">1379547</a>)</p></li>
<li><p>Scene/Game View: Fixed issue where expanding a collapsed search overlay would result in stack overflow and crash the editor. (1382216)</p></li>
<li><p>Scene/Game View: Fixed locked Inspector causing duplicate tool buttons to appear in component tool toolbars. (<a href="https://issuetracker.unity3d.com/issues/duplicate-buttons-appear-in-a-hinge-joint-component-when-having-two-inspectors-open">1338708</a>)</p></li>
<li><p>Scene/Game View: Fixed MonoBehaviour icons not rendering in Scene View when selected. (<a href="https://issuetracker.unity3d.com/issues/hdrp-decal-gizmo-flickers-when-rectangle-selected">1293266</a>)</p></li>
<li><p>Scene/Game View: Fixed Scene View FX toggle not accurately representing the enabled state of FX. (<a href="https://issuetracker.unity3d.com/issues/scene-effects-toggle-keeps-being-disabled-upon-entering-play-mode">1379441</a>)</p></li>
<li><p>Scene/Game View: Fixed tool gizmos clipping in cases where adjacent objects are separated by large distances on the z axis. (<a href="https://issuetracker.unity3d.com/issues/gizmos-on-the-objects-fade-away-when-zooming-out-in-2d-mode">1353387</a>)</p></li>
<li><p>Scene/Game View: Fixed tool settings overlay not updating contents when active tool editor does not support current container layout. (1348529)</p></li>
<li><p>Scene/Game View: Fixed Tools Overlay not respecting EditorTool.IsAvailable() value. (1373145)</p></li>
<li><p>Scene/Game View: Fixed Tools Overlay showing invalid tools for the active context. (1373147)</p></li>
<li><p>Scripting: Fixed an issue causing Editor to lock-up or crash when creating a ScriptableObject that instantiates a new ScriptableObject in OnEnable method. (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-and-crashes-when-creating-a-scriptableobject-that-instantiates-a-new-scriptableobject-in-onenable-method">1332971</a>)</p></li>
<li><p>Scripting: Fixed an issue that caused a performance regression which was due to a race condition fix when accessing the mono wrapper of a native object. (1353355)</p></li>
<li><p>Scripting: Fixed case where Define Constraints did not work properly for precompiled assemblies. (<a href="https://issuetracker.unity3d.com/issues/runtimeinitializeonload-methods-are-called-multiple-times-when-using-define-constraints-for-precompiled-assemblies">1327988</a>)</p></li>
<li><p>Scripting: Fixed issue where precompiled DLL with define constraints was not being included in a build when passing extra define constraints. (<a href="https://issuetracker.unity3d.com/issues/android-dll-with-define-constraint-included-in-buildplayeroptions-dot-extrascriptingdefines-is-not-included-in-build">1330363</a>)</p></li>
<li><p>Scripting: Fixed newline in namespaces. (<a href="https://issuetracker.unity3d.com/issues/monobehaviour-scripts-cause-compilation-errors-when-the-namespace-contains-a-line-break">1407718</a>)</p></li>
<li><p>Scripting: Fixed Plane.SetNormalAndPosition behaviour when passing a non-normalized normal vector. (1346589)</p></li>
<li><p>Scripting: Fixed Quaternion.ToAngleAxis() returning NaN for quaternion(0,0,0,-1). (<a href="https://issuetracker.unity3d.com/issues/quaternion-toangleaxis-does-not-deal-with-singularity-at-0-0-0-1">1348545</a>)</p></li>
<li><p>Scripting: Fixed race condition in TextWriterLogger which may lead to exceptions in ApiUpdater.</p></li>
<li><p>Scripting: Project generation will get updated PlayerSettings for writing csproj files. (1336737)</p></li>
<li><p>Scripting: SemVersionParser.TryParse and UnityVersionParser.TryParse don't throw first chance exceptions anymore. (1340457)</p></li>
<li><p>Scripting: When switching to UWP it doesn't add NET_STANDARD_2_0 define, it adds NET_4_6 instead. (<a href="https://issuetracker.unity3d.com/issues/uwp-not-adding-net-standard-2-0-define">1334636</a>)</p></li>
<li><p>Scripting: <code>[InitializeOnLoad]</code> classes are now initialized in a defined order based on assembly references, such that if Assembly B depends on Assembly A, all <code>[InitializeOnLoad]</code> classes in Assembly A are guaranteed to be initialized prior to any <code>[InitializeOnLoad]</code> classes in Assembly B. (1344815)</p></li>
<li><p>Search: Delay search engines initialization after user code is compiled.</p></li>
<li><p>Search: Fixed bug that causes searcher window to be offset too far when accounting for host window boundaries.</p></li>
<li><p>Search: Fixed deleting text in QueryBuilder can delete block by mistake. (1376664)</p></li>
<li><p>Search: Fixed double click on store search results opens Package Manager instead of Asset Store. (<a href="https://issuetracker.unity3d.com/issues/double-click-at-search-results-opens-package-manager-instead-of-asset-store">1362492</a>)</p></li>
<li><p>Search: Fixed fail to drag subasset from search window to ObjectField. (<a href="https://issuetracker.unity3d.com/issues/search-fail-to-drag-subasset-from-search-window-to-objectfield">1374002</a>)</p></li>
<li><p>Search: Fixed Out of memory crash when using the search picker to pick a large set of texture and/or sprites View on Crashes HQ. (<a href="https://issuetracker.unity3d.com/issues/search-out-of-memory-crash-when-using-the-search-picker-to-pick-a-large-set-of-texture-and-slash-or-sprites">1362804</a>)</p></li>
<li><p>Search: Fixed possible null reference exception in Search. (<a href="https://issuetracker.unity3d.com/issues/static-analysis-defect-672865-in-modules-slash-quicksearch-slash-editor-slash-queryengine-slash-querytoken-dot-cs">1372840</a>)</p></li>
<li><p>Search: Fixed query block editor popup position and size on OSX. (1376679)</p></li>
<li><p>Search: Fixed search by type tags are not adapted for use with the Quick Search engine. (<a href="https://issuetracker.unity3d.com/issues/search-by-type-tags-are-not-adapted-for-use-with-the-quick-search-engine">1334338</a>)</p></li>
<li><p>Search: Fixed search indexer get document lock while an incremental update.</p></li>
<li><p>Search: Fixed text in the search field of the Search window doesn't get selected after focusing the window and clicking on the field once. (<a href="https://issuetracker.unity3d.com/issues/text-in-the-search-field-of-the-search-window-doesnt-get-selected-after-focusing-the-window-and-clicking-on-the-field-once">1338063</a>)</p></li>
<li><p>Serialization: Avoid out-of-memory crash when corrupt meta file contains a certain sequence of characters. (<a href="https://issuetracker.unity3d.com/issues/crash-on-memorymanager-outofmemoryerror-when-opening-a-project-with-corrupted-meta-files">1332514</a>)</p></li>
<li><p>Serialization: Changed the internal behavior of the SerializedProperty.propertyPath eliminating unnecessary string allocations on every call.</p></li>
<li><p>Serialization: Fixed an issue where Unity could crash when recursively calling methods that invoke serialization. (<a href="https://issuetracker.unity3d.com/issues/crash-on-memorymanager-allocate-when-calling-assetdatabase-dot-createasset-in-onprocessshader">1227302</a>)</p></li>
<li><p>Serialization: Fixed cancel case when deleting an array element with multiple objects selected. (<a href="https://issuetracker.unity3d.com/issues/both-elements-are-set-to-none-in-reorderables-when-cancel-is-clicked-in-the-remove-element-dialog-if-multiple-gos-are-selected">1305941</a>)</p></li>
<li><p>Serialization: Fixed for SerializedObject to retain individual object array content, when multiple objects selected and the last element is added or removed. (<a href="https://issuetracker.unity3d.com/issues/serializedproperty-array-values-get-copied-from-one-asset-to-another-when-modifying-the-array-while-having-two-assets-selected">1277419</a>)</p></li>
<li><p>Serialization: Fixed NullReferenceException is thrown when a MonoBehaviour script that was attached to a GameObject is deleted. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-is-throw-when-a-monobehaviour-script-that-was-attached-to-a-gameobject-is-deleted">1355905</a>)</p></li>
<li><p>Serialization: Fixed SerializeReference object missing in certain situation.</p></li>
<li><p>Serialization: Fixed wrong values get copied when copying long values in the Inspector. (<a href="https://issuetracker.unity3d.com/issues/wrong-values-get-copied-when-copying-long-values-in-the-inspector">1372674</a>)</p></li>
<li><p>Serialization: Improved performance of GetArrayElementAtIndex.</p></li>
<li><p>Serialization: Prevent serialization of fields by-value if the field's type is derived from the class being serialized. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-opening-project-due-to-serialization-memory-leak">1317343</a>)</p></li>
<li><p>Services: Fixed bug in the way usymtool handles inlined lines in DWARF data. (1393336)</p></li>
<li><p>Services: Fixed issue with Usymtool failing to read some PDB files. (1412493)</p></li>
<li><p>Services: Fixed usymtool sometimes failing to process symbol files correctly. (1375841)</p></li>
<li><p>Services: Reduced processing time and memory use of usymtool. (1396931)</p></li>
<li><p>Services: Usymtool will process public symbols correctly again. (1403471)</p></li>
<li><p>Shadergraph: Fixed a bug that Parallax Mapping and Parallax Occlusion Mapping nodes don't use the same channel to sample heightmap by adding drop-downs for channel selecting to both of the nodes. (1347270)</p></li>
<li><p>Shadergraph: Fixed a bug where node preview doesn't update when a texture is changed in the explorer. (<a href="https://issuetracker.unity3d.com/issues/texture-in-the-shader-graph-did-not-get-updated-when-the-texture-file-is-changed">1363784</a>)</p></li>
<li><p>Shadergraph: Fixed a recent regression in ShaderGraph Screen Position behavior on some platforms in Built-in, Universal and HDRP.</p></li>
<li><p>Shadergraph: Fixed a serialization bug wrt PVT property flags when using subgraphs. This fixes SRP batcher compatibility.</p></li>
<li><p>Shadergraph: Fixed a ShaderGraph issue where a material inspector could contain an extra set of render queue, GPU instancing, and double-sided GI controls.</p></li>
<li><p>Shadergraph: Fixed a usability issue where in some cases searcher would suggest one collapsed category of results that user would have to manually expand anyway.</p></li>
<li><p>Shadergraph: Fixed a warning in ShaderGraph about BuiltIn Shader Library assembly having no scripts.</p></li>
<li><p>Shadergraph: Fixed an issue where ShaderGraph 'view shader' commands were opening in individual windows, and blocking Unity from closing.</p></li>
<li><p>Shadergraph: Fixed compilation problems on preview shader when using hybrid renderer v2 and property desc override Hybrid Per Instance.</p></li>
<li><p>Shadergraph: Fixed errors in the ShaderGraph Transform node. (1368082)</p></li>
<li><p>Shadergraph: Fixed incorrect warning while using VFXTarget.</p></li>
<li><p>Shadergraph: Fixed loading all materials from project when saving a ShaderGraph.</p></li>
<li><p>Shadergraph: Fixed missing shader keyword stage during keyword copying.</p></li>
<li><p>Shadergraph: Fixed noise nodes to use a deterministic integer hash, instead of platform dependent floating point hashes. (1156544)</p></li>
<li><p>Shadergraph: Fixed ShaderGraph BuiltIn target shader GUI to allow the same render queue control available on URP with the changes for case.</p></li>
<li><p>Shadergraph: Fixed ShaderGraph HDRP master preview disappearing for a few seconds when graph is modified.</p></li>
<li><p>Shadergraph: Fixed ShaderGraph isNaN node, which was always returning false on Vulkan and Metal platforms.</p></li>
<li><p>Shadergraph: Fixed the behavior of checkerboard node with raytracing.</p></li>
<li><p>Shadergraph: Fixed the incorrect value written to the VT feedback buffer when VT is not used.</p></li>
<li><p>Shadergraph: Fixed the Scene Depth node so it returns proper results in Eye space when using an orthographic camera.</p></li>
<li><p>Shadergraph: Fixed the sticky-note editable title text size in shader graph not matching the set font size. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-sticky-notes-title-is-always-rendered-in-small-font-while-editing-regardless-of-the-set-font-size">1357657</a>)</p></li>
<li><p>Shadergraph: Fixed the wrong scaling of the main preview window. (<a href="https://issuetracker.unity3d.com/issues/main-preview-window-is-rendered-with-blank-vertical-lines-at-the-sides-when-shader-graph-window-is-open">1356719</a>)</p></li>
<li><p>Shadergraph: Fixed Triplanar ShaderGraph node to handle arbitrary input and output coordinate spaces. (<a href="https://issuetracker.unity3d.com/issues/shader-graph-rotating-gameobject-get-material-stretched-when-using-triplanar-node">1346477</a>)</p></li>
<li><p>Shadergraph: Fixed upgrade warnings on SpeedTree8 subgraphs.</p></li>
<li><p>Shadergraph: Gradient field doesn't support HDR values. (<a href="https://issuetracker.unity3d.com/issues/vfx-gradients-no-longer-support-hdr-values">1381867</a>)</p></li>
<li><p>Shadergraph: Improved screenspace position accuracy in the fragment shader by using VPOS. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-dither-node-results-in-artifacts-when-far-from-origin-caused-by-screen-position-breaking-down">1352662</a>)</p></li>
<li><p>Shaders: Added human readable clarification when hitting undeclared keywords on some shader passes. (<a href="https://issuetracker.unity3d.com/issues/missing-keyword-declarations-when-using-dynamic-branching-is-not-obvious-to-user">1390142</a>)</p></li>
<li><p>Shaders: Bumped material property blocks array size limit from 1023 to 1048575. (<a href="https://issuetracker.unity3d.com/issues/materialpropertyblock-arrays-are-limited-to-1023-elements">1358444</a>)</p></li>
<li><p>Shaders: Clean up old shader cache entries from the disk.</p></li>
<li><p>Shaders: Fixed a bug with SHADER_AVAILABLED_XXX macros not being defined in compute shaders. (<a href="https://issuetracker.unity3d.com/issues/shader-available-xxx-defines-are-not-set-in-compute-shaders">1364139</a>)</p></li>
<li><p>Shaders: Fixed an issue whereby the built-in shaders zip package no longer contains a bunch of empty folders.</p></li>
<li><p>Shaders: Fixed incorrect casts in Metal shaders when a reinterpret cast was intended. (<a href="https://issuetracker.unity3d.com/issues/ios-set-attribute-from-map-blocks-dont-work-in-initialize-when-using-runtime-shaders">1331056</a>)</p></li>
<li><p>Shaders: Fixed multi_compile_particles to work together with built-in lighting variants. Requires shader re-import. (<a href="https://issuetracker.unity3d.com/issues/multi-compile-particles-changes-shader-appearance">1346626</a>)</p></li>
<li><p>Shaders: Fixed recent rendering performance regression caused by dynamic branching feature. (1380277)</p></li>
<li><p>Shaders: Fixed ShaderPropertySheet native tests on some setups. (<a href="https://issuetracker.unity3d.com/issues/shaderpropertysheet-native-tests-failing-unity-2022-when-minconstantbufferoffsetalignment-unsupported">1402368</a>)</p></li>
<li><p>Shaders: Fixed strict shader variant matching not picking up correct variants when using stage-specific keywords. (1368999)</p></li>
<li><p>Shaders: Fixed surface shaders compilation failures when using #pragma dynamic_branch. (1380291)</p></li>
<li><p>Shaders: Metal shaders that use 'pragma only_renderers framebufferfetch' are now correctly reported as unsupported on MacOS. Shaders that use 'pragma require framebufferfetch' are no longer reported as unsupported on platforms that support framebuffer fetch. (<a href="https://issuetracker.unity3d.com/issues/macos-unexpected-color-data-is-stored-when-using-number-pragma-only-renderers-framebufferfetch-in-shader">1288056</a>)</p></li>
<li><p>Shaders: Prevented toggles and user properties from overriding dynamic branching keyword state in the shaders. (1377683)</p></li>
<li><p>Shaders: Updated DXC libraries to fix a regression with DXIL validation for shaders that use barycentrics and possibly other newer features. (<a href="https://issuetracker.unity3d.com/issues/dxc-compiler-shader-error-in-unlit-slash-newunlitshader-program-frag-error-flags-must-match-us-when-using-barycentrics">1349629</a>)</p></li>
<li><p>Terrain: [Static Analysis] Defect 672727 in Modules/Terrain/Public/PaintContext.cs. (1367368)</p></li>
<li><p>Tests: Fixed instability with test FrontEndApiInitializationFromThread [INSTABILITY:1474884]. (1396899)</p></li>
<li><p>Tests: Updated JobTests_JobDebugger unit test to reflect fixed NativeArray behavior.<br> be updated accordingly).</p></li>
<li><p>Text: Fixed an issue where Sprite Asset sprite glyph scale was not affecting the scale of sprites in UI Toolkit. (1364241)</p></li>
<li><p>Text: Fixed unwanted UTF-16/UTF-32 escaped sequence. (<a href="https://issuetracker.unity3d.com/issues/ui-builder-label-text-displays-invalid-characters-when-certain-special-characters-are-used">1367695</a>)</p></li>
<li><p>Timeline: Fixed an issue where Timeline preview would be interrupted when a scene was saved. (<a href="https://issuetracker.unity3d.com/issues/the-timeline-doesnt-set-back-the-state-of-game-objects-after-saving-a-scene">1360485</a>)</p></li>
<li><p>uGUI: Added a new data unavailable message to the UI Profiler for when this is not attached to the editor. (<a href="https://issuetracker.unity3d.com/issues/profiler-ui-module-details-pane-section-is-empty-when-capturing-from-a-built-player">1251139</a>)</p></li>
<li><p>uGUI: Added a NullReferenceException when selecting a Dropdown Component override in the prefab overrides menu for the second time. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-when-selecting-a-dropdown-component-override-in-the-prefab-overrides-menu-for-the-second-time">1308539</a>)</p></li>
<li><p>uGUI: Added a switch to Canvas to allow the user to determine if the canvas should resize on manual Camera.Render calls.</p></li>
<li><p>uGUI: Changed the calculations to take in consideration images that may be smaller than their RecTransform. Fixes the raycasting on those images. (<a href="https://issuetracker.unity3d.com/issues/hovering-over-the-sprite-is-offset-when-alphahittestminimumthreshold-is-higher-than-0-and-sprite-meshtype-is-set-to-tight">1341107</a>)</p></li>
<li><p>uGUI: Fixed an issue to force update the Canvas RectTransform on load from disk, so that Override nested Canvas can still get a proper world transform for rendering. (<a href="https://issuetracker.unity3d.com/issues/a-child-canvas-with-override-sorting-is-not-rendered-on-editor-start-if-the-parent-canvas-is-disabled">1322784</a>)</p></li>
<li><p>uGUI: Fixed the canvas size not having the correct values when reopening the project. (<a href="https://issuetracker.unity3d.com/issues/canvas-gets-shrunk-in-the-scene-view-after-reopening-the-project">1342677</a>)</p></li>
<li><p>uGUI: Fixed the formula in GridLayout to make sure the constraint column/row amount is always respected. (<a href="https://issuetracker.unity3d.com/issues/grid-layout-group-constraint-count-set-to-4-not-working-when-constraint-is-set-to-fixed-row-count-and-start-axis-to-horizontal">1345471</a>)</p></li>
<li><p>uGUI: Fixed the game view's aspect ratio distortion on static aspect ratios and when resizing the window. (<a href="https://issuetracker.unity3d.com/issues/gameview-dimensions-distorted-when-resizing">1373961</a>)</p></li>
<li><p>uGUI: Fixed the InputField layout recalculation by forcing a rebuild before calculating how many characters can fit inside. (<a href="https://issuetracker.unity3d.com/issues/input-fields-width-doesnt-change-after-entering-specific-combinations-of-text-when-the-content-size-fitter-is-used">1320719</a>)</p></li>
<li><p>uGUI: Fixed the ScrollRect content position upon reloading a scene when either one or both of the horizontal and vertical properties are not applied. (<a href="https://issuetracker.unity3d.com/issues/scrollrect-contents-recttransform-bound-go-crazy-when-overriding-a-prefab">1088655</a>)</p></li>
<li><p>uGUI: Fixed the SliderEditor's slider handler disappearing when setting a min value greater than the value on a Slider preset. (<a href="https://issuetracker.unity3d.com/issues/ui-minmaxslider-disappears-when-enable-slash-disable-whole-numbers-checkbox-for-ui-slider-preset">1337860</a>)</p></li>
<li><p>uGUI: Fixed the way the raycast 2D is calculated to take in account the Z position of the sprite. (<a href="https://issuetracker.unity3d.com/issues/physics2draycaster-distance-results-ignore-sprite-z-position">1340417</a>)</p></li>
<li><p>uGUI: Fixed UI Components causing GC Allocation when enabled. (<a href="https://issuetracker.unity3d.com/issues/ui-components-cause-gc-allocation-when-enabled">1299752</a>)</p></li>
<li><p>uGUI: Makes sure no call to the ReadPixels is made while using a crunch compression on an image. (<a href="https://issuetracker.unity3d.com/issues/ugui-image-with-crunch-compression-can-still-have-a-modified-alphahittestminimumthreshold">1341100</a>)</p></li>
<li><p>uGUI: Removed the allocation caused by the GetComponent in the layout when scrolling. (<a href="https://issuetracker.unity3d.com/issues/scrollrect-layout-recalculation-causes-unnecessary-allocation">1343656</a>)</p></li>
<li><p>uGUI: Updated the Raycast Target property at runtime even if started as disabled. (<a href="https://issuetracker.unity3d.com/issues/animated-image-property-raycast-target-does-not-function-when-disabled-before-entering-play-mode">1341044</a>)</p></li>
<li><p>UI Toolkit: Added support for using a numeric value for enum fields in uxml.<br> Added support for using a flags enum in uxml (multiple flags may now be set by joining them with a comma).<br>
Added support for flags enum in the UI Builder for UxmlEnumAttributeDescription.<br>
Fixed an issue in the UI Builder where using an invalid enum value in uxml would break the attribute section of the inspector.<br>
Fixed an issue where the uxml importer and the UI Builder would parse an enum differently, leading to valid cases being reported as errors and invalid cases reported as working.<br>
Fixed an issue where the EnumField would not update the display text when setting an invalid value (the actual value would be changed, but the display text would not).
(1375227)</p></li>
<li><p>UI Toolkit: Ensured that invalid uxml and uss files cannot be opened nor can be added to an existing document. (<a href="https://issuetracker.unity3d.com/issues/uibuilder-edit-setup-is-corrupted-when-malformed-uxml-is-loaded">1333514</a>)</p></li>
<li><p>UI Toolkit: Fixed 1357249: Editor freezes when decreasing the VisualElement size of a Dropdown. (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-when-decreasing-the-visualelement-size-of-a-dropdown">1357249</a>)</p></li>
<li><p>UI Toolkit: Fixed 1413448: [UIToolkit] Clicking on a ListView throws errors.</p></li>
<li><p>UI Toolkit: Fixed a couple of issues with the UI of Transform in UI Builder. (<a href="https://issuetracker.unity3d.com/issues/issues-with-the-transform-ui-in-the-builder">1342227</a>)</p></li>
<li><p>UI Toolkit: Fixed a few USS style settings to match IMGUI inspectors and a wrong check for property fields in inspector elements. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-objectfield-doesnt-line-up">1320031</a>)</p></li>
<li><p>UI Toolkit: Fixed absolute child element ignore padding of the parent. (<a href="https://issuetracker.unity3d.com/issues/yoga-absolute-child-with-percentage-width-slash-height-ignore-padding-of-the-parent">1348644</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue in the UI Builder where editing a style property would edit the wrong one when a style rule contained the same style property multiple times. (1373706)</p></li>
<li><p>UI Toolkit: Fixed an issue that pressing Enter on a focused ListView element when its SelectionType is set to None will no longer scroll to the last item. (<a href="https://issuetracker.unity3d.com/issues/customeditor-list-scrolls-down-when-pressing-enter-and-listview-dot-selectiontype-is-set-to-none">1372675</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue when a modal window is opened, the UI Elements property animations, as well as scheduled items, asynchronous tasks and Update() callbacks are now updated as expected. (<a href="https://issuetracker.unity3d.com/issues/scheduled-items-asynchronous-tasks-and-update-are-not-run-when-editorwindow-is-opened-using-showmodalutility">1333331</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where externally editing a UI document would open the UI Builder window. (<a href="https://issuetracker.unity3d.com/issues/ui-builder-editing-uxml-file-externally-opens-the-ui-builder">1365403</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where MinMaxSlider's value would be wrongly clamped when loaded from uxml.<br> Fixed an issue where constructing a MinMaxSlider with valid values would throw an exception.
(1368242)</p></li>
<li><p>UI Toolkit: Fixed an issue where setting the same StyleKeyword to a style property would dirty the panel. (1356202)</p></li>
<li><p>UI Toolkit: Fixed an issue where the theme style sheet icon would not be shown when creating the asset. (<a href="https://issuetracker.unity3d.com/issues/tss-theme-files-icon-is-invisible-until-the-name-is-set-when-creating-a-new-tss-theme-file">1365364</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue with the search completion where a variable set to color name was treated as an enum variable rather than a color variable. (<a href="https://issuetracker.unity3d.com/issues/uibuilder-color-variables-set-to-color-names-are-not-recognized-as-colors-by-the-auto-complete">1359230</a>)</p></li>
<li><p>UI Toolkit: Fixed checker pattern background no longer visible. (1340240)</p></li>
<li><p>UI Toolkit: Fixed default.tss.asset failing to load while the UI Toolkit package is being imported. (<a href="https://issuetracker.unity3d.com/issues/runtime-theme-default-dot-tss-dot-asset-failed-to-be-loaded-from-uitk-package-while-the-package-is-being-imported">1362005</a>)</p></li>
<li><p>UI Toolkit: Fixed DynamicTransform elements disappearing when assigning a Vector2 scale factor. (<a href="https://issuetracker.unity3d.com/issues/using-usagehints-dot-dynamictransform-disables-rendering-of-visualelement-in-the-play-mode">1341601</a>)</p></li>
<li><p>UI Toolkit: Fixed editor window creation menu references. Now created files can be renamed. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-editor-window-does-not-open-when-changing-the-uss-file-name-and-renaming-it-back">1347331</a>)</p></li>
<li><p>UI Toolkit: Fixed exceptions being thrown when setting the value of an EnumField inside the UI Builder. (1331021)</p></li>
<li><p>UI Toolkit: Fixed failing DoubleField round-trip conversion when value is set to double.MinValue or double.MaxValue, resulting in the DoubleField text being "0". (1367534)</p></li>
<li><p>UI Toolkit: Fixed focus in the list view when navigating with arrow keys or scrolling. (<a href="https://issuetracker.unity3d.com/issues/listview-becomes-unselected-when-scrolling-with-up-down-home-or-end-keys">1372673</a>)</p></li>
<li><p>UI Toolkit: Fixed hardcoded paths in editor window creation menu. (1317521)</p></li>
<li><p>UI Toolkit: Fixed Image class alignment issue on non-standard DPIs. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-image-content-is-off-by-one-pixel-when-the-scalling-in-the-os-display-settings-is-set-to-150-percent">1330817</a>)</p></li>
<li><p>UI Toolkit: Fixed label FieldMouseDragger in sliders. (<a href="https://issuetracker.unity3d.com/issues/2d-input-value-of-all-properties-are-not-changing-when-a-mouse-is-dragged-over-it-in-the-skinning-editor">1294945</a>)</p></li>
<li><p>UI Toolkit: Fixed list view animated reordering when clicking on a TextField. (1371166)</p></li>
<li><p>UI Toolkit: Fixed missing Length conversions for style transitions between px and % units. (1348296)</p></li>
<li><p>UI Toolkit: Fixed NullReferenceException thrown when calling GetWindow&lt;&gt;() inside ShowWindow() when called from [InitializeOnLoad] class. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-calling-getwindow-inside-showwindow-when-called-from-initializeonload-class">1325267</a>)</p></li>
<li><p>UI Toolkit: Fixed NullReferenceException when clicking the Settings button in the UI Builder window. (1340230)</p></li>
<li><p>UI Toolkit: Fixed object selection not working when clicking on the object in a disabled UI Toolkit ObjectField. (1355709)</p></li>
<li><p>UI Toolkit: Fixed polyline fills with only three edges. (1388225)</p></li>
<li><p>UI Toolkit: Fixed possible NullReferenceException in BaseTreeView.OnViewDataReady. (1401264)</p></li>
<li><p>UI Toolkit: Fixed rendering on Adreno3XX GPUs. (<a href="https://issuetracker.unity3d.com/issues/opengles3-android-uitoolkit-is-not-rendered-properly-on-some-devices">1361189</a>)</p></li>
<li><p>UI Toolkit: Fixed ScrollView's scroll type persistance in the builder and elastic mode will not act like unrestricted mode in editor. (1362816)</p></li>
<li><p>UI Toolkit: Fixed shader inspector configuration options sometimes not responding to clicks in the Editor. (<a href="https://issuetracker.unity3d.com/issues/shader-preprocess-only-option-and-compile-and-show-code-do-nothing-when-clicked-if-shader-is-in-packages-folder">1376549</a>)</p></li>
<li><p>UI Toolkit: Fixed slow color changes on labels. (1337368)</p></li>
<li><p>UI Toolkit: Fixed SVG 9-slice visual artefact. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-9-slice-scaling-is-wrong-on-vector-images">1354273</a>)</p></li>
<li><p>UI Toolkit: Fixed Test [Instability][trunk] StyleSheetPaneTests.SelectorRenameWithEmptyStringRevertsToOriginalText (UI Builder). (1355533)</p></li>
<li><p>UI Toolkit: Fixed TextCore outline/shadow color in editor. (1341868)</p></li>
<li><p>UI Toolkit: Fixed the color and style of the title text in the UI Toolkit debugger. (1344018)</p></li>
<li><p>UI Toolkit: Fixed the EnumField's type and value incorrectly fetching data from the UXML document inside the UI Builder.<br> Improved the EnumField and ObjectField type input to display an auto-complete popup inside the UI Builder.<br>
Fixed the value input of an EnumField to use an EnumField instead of TextField inside the UI Builder.<br>
Fixed the value input of an TagField to use an TagField instead of TextField inside the UI Builder.<br>
Fixed the value input of an LayerField to use an LayerField instead of TextField inside the UI Builder.<br>
Fixed the value input of an LayerMaskField to use an LayerMaskField instead of LayerMaskField inside the UI Builder.
(1330804)</p></li>
<li><p>UI Toolkit: Fixed the EnumField's value from being cleared while saving a UXML document inside the UI Builder. (1330802)</p></li>
<li><p>UI Toolkit: Fixed the issue that Text Settings can not be created in a local package when right-clicking the local package folder. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-cant-create-textsettings-asset-file-in-packages-local-package-folder">1327812</a>)</p></li>
<li><p>UI Toolkit: Fixed the issue that UI Document created in a local package appeared in the Assets folder, with incorrect default file name. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-ui-document-is-created-in-assets-instead-of-packages-folder">1327810</a>)</p></li>
<li><p>UI Toolkit: Fixed the UI Builder and the UI Toolkit Debugger displaying duplicates in the matching selector sections. (<a href="https://issuetracker.unity3d.com/issues/ui-builder-there-are-duplicate-matching-selectors-under-the-stylesheet-matching-selectors-tab-in-the-ui-builder-inspector">1347536</a>)</p></li>
<li><p>UI Toolkit: Fixed the UI Toolkit PropertyField not tracking the underlying value properly when [SerializeReference] is used on a field. (<a href="https://issuetracker.unity3d.com/issues/propertyfields-dont-work-properly-with-serializereference-fields">1216937</a>)</p></li>
<li><p>UI Toolkit: Fixed tooltips not shown in children of a BaseField. (1355200)</p></li>
<li><p>UI Toolkit: Fixed UI Toolkit events not working after script recompilation during Play mode when using the EventSystem component as the source of events. (<a href="https://issuetracker.unity3d.com/issues/uitoolkit-package-breaks-after-assembly-reload-when-using-the-input-system-package-for-input">1324337</a>)</p></li>
<li><p>UI Toolkit: Fixed UI Toolkit Live Reload errors on Editor Window after modifying uxml file and returning to Editor and the window is docked. (<a href="https://issuetracker.unity3d.com/issues/ui-toolkit-live-reload-errors-on-editor-window-after-modifying-uxml-file-and-returning-to-editor-and-the-window-is-docked">1329767</a>)</p></li>
<li><p>UI Toolkit: Fixed UI Toolkit throwing InvalidOperationExceptions when Input Manager isn't accessible. (<a href="https://issuetracker.unity3d.com/issues/invalidoperationexception-gets-thrown-in-the-console-when-using-the-new-input-system">1336180</a>)</p></li>
<li><p>UI Toolkit: Fixed uxml files not being re-imported after changes in the uxml importer. (1343398)</p></li>
<li><p>UI Toolkit: Fixed Vector API polyline fill antialiasing. (1393886)</p></li>
<li><p>UI Toolkit: Fixed wrong parent used by a VisualElement for rendering when added to a contentContainer, such as a ScrollView. (1374976)</p></li>
<li><p>UI Toolkit: In the UI Builder, the user can no longer use the inspector on a style selector and rename the selector to an empty name (UI Builder). (1342352)</p></li>
<li><p>UI Toolkit: Make sure ChangeEvent&lt;float&gt; isn't leaked by the TextField. (<a href="https://issuetracker.unity3d.com/issues/incremental-snap-move-y-and-z-fields-values-become-different-than-x-field-value-when-using-small-numbers">1389410</a>)</p></li>
<li><p>UI Toolkit: Make sure maxLength is respected by all inner components of the InputField. (1390038)</p></li>
<li><p>UI Toolkit: Make sure TextSetting's default sprite asset is cleared when changing from PlayMode to Editor. (1291771)</p></li>
<li><p>UI Toolkit: Removed any (UI Toolkit-based) UI Builder package-specific code from the editor as well as prevents the use of the UI Builder package, in favour of the built-in version.</p></li>
<li><p>UI Toolkit: Removed duplicated internal functionality to resolve style variables. (1374879)</p></li>
<li><p>UI Toolkit: Selecting another editable TextField doesn't close SoftKeyboard. (1350228)</p></li>
<li><p>UI Toolkit: Slider dragger-container height/width are now properly set when not showing the input field and setting align-items to something else than stretch. (<a href="https://issuetracker.unity3d.com/issues/scrollbar-in-slider-is-not-in-the-same-position-as-mouse-cursor-when-using-ui-toolkit">1362979</a>)</p></li>
<li><p>UI Toolkit: TemplateContainer has its own icon and no longer shows the custom control icon when is nested in another template (UI Builder). (1340837)</p></li>
<li><p>UI Toolkit: The IMGUIContainer control will now be available as an editor-only control from the UI Builder. (1354419)</p></li>
<li><p>UI Toolkit: UI Toolkit: Fixes the content of the transition properties dropdown being appended instead of recreated when opening the UI Builder window. (1343063)</p></li>
<li><p>Undo System: Added warning for large actions which overflow the undo stack. (<a href="https://issuetracker.unity3d.com/issues/undo-is-not-restoring-all-of-the-deleted-gameobjects-when-deleting-a-large-number-of-gameobjects">1204737</a>)</p></li>
<li><p>Undo System: Fixed an issue where script's icon does not change back on Undo in the Project window. (<a href="https://issuetracker.unity3d.com/issues/scripts-icon-does-not-change-back-to-the-default-on-undo-in-the-project-window">1331877</a>)</p></li>
<li><p>Undo System: Fixed regression bug (crash) when performing SetTransformParent followed by deletion of target object, then undo. (1380419)</p></li>
<li><p>Undo System: Fixed undo/redo of adding objects to scriptable objects. (<a href="https://issuetracker.unity3d.com/issues/crash-occurs-on-memorymanager-getallocator-or-an-error-changetype-equals-destroy-is-thrown-when-performing-undo-slash-redo">1294434</a>)</p></li>
<li><p>Undo System: Improved performance when overwriting the redo stack.</p></li>
<li><p>Undo System: Redo stack is now restored upon exiting playmode. (<a href="https://issuetracker.unity3d.com/issues/undo-stack-is-desynchronised-when-undoing-changes-in-play-mode-and-resetting-the-scene-by-exiting-it">1336257</a>)</p></li>
<li><p>Universal Windows Platform: Fixed Application.identifier returning an empty string. It will now return the identity name specified in the application manifest. (<a href="https://issuetracker.unity3d.com/issues/unityengine-dot-application-dot-identifier-returns-an-empty-string-when-called-in-uwp-build">1399538</a>)</p></li>
<li><p>Universal Windows Platform: Fixed Application.targetFrameRate rendering at significantly lower frame rate than specified.</p></li>
<li><p>Universal Windows Platform: Fixed development builds not starting up on Windows 10 versions prior to build 15063.</p></li>
<li><p>Universal Windows Platform: Fixed incorrect WSATestCertificate error message after moving project's folder. (<a href="https://issuetracker.unity3d.com/issues/uwp-wsatestcertificate-causes-errors-in-console-window-when-changing-the-projects-folder-directory">1361792</a>)</p></li>
<li><p>Universal Windows Platform: Fixed touch events causing incorrect UI behavior when using Windows touch Simulator. (1371807)</p></li>
<li><p>Universal Windows Platform: Fixed TouchScreenKeyboard.active returning true when the keyboard isn't visible. (<a href="https://issuetracker.unity3d.com/issues/hololens-touchscreenkeyboard-doesnt-report-correct-status-or-active-values">1141591</a>)</p></li>
<li><p>URP: Added Undo support for URP Global Settings asset assignation.</p></li>
<li><p>URP: Added warning for lit shader detailed abledo, if texture is not linear. (<a href="https://issuetracker.unity3d.com/issues/detail-maps-packed-differently-in-built-in-vs-urp">1342011</a>)</p></li>
<li><p>URP: Fixed "Add Renderer Feature" filtering in menu.</p></li>
<li><p>URP: Fixed a depth non-clear in XR due to wrong depth slice being checked.</p></li>
<li><p>URP: Fixed a regression where filtering the scene view yielded incorrect visual results.</p></li>
<li><p>URP: Fixed a regression where ShaderGraph screen position was not correct in game view and when using XR.</p></li>
<li><p>URP: Fixed an issue in where the Convert Renderering Settings would cause a freeze.</p></li>
<li><p>URP: Fixed an issue in where the current open scene didn't load after running the converters. (1365101)</p></li>
<li><p>URP: Fixed an issue where shadow artefacts appeared between cascades on Terrain Detail objects.</p></li>
<li><p>URP: Fixed an issue where ShadowCasters were sometimes being rendered twice in the editor while in playmode.</p></li>
<li><p>URP: Fixed an issue where Sprite type Light2Ds were missing a default sprite.</p></li>
<li><p>URP: Fixed an issue where Sprite type Light2Ds would throw an exeception if missing a sprite.</p></li>
<li><p>URP: Fixed an issue where SSAO would throw a "RenderingCommandBuffer: invalid pass index" errors. (<a href="https://issuetracker.unity3d.com/issues/urp-renderingcommandbuffer-invalid-pass-index-errors-when-opening-urp-sample-scenes">1374215</a>)</p></li>
<li><p>URP: Fixed an issue where the "Skip Iterations" option on Bloom could cause the effect to not run at all, which would cause flickering due to the Bloom texture being uninitialized. (<a href="https://issuetracker.unity3d.com/issues/particle-effect-causes-bloom-post-effect-deactivation-at-mouse-hover-if-not-selected">1382991</a>)</p></li>
<li><p>URP: Fixed an issue where the 2D Renderer was not rendering depth and stencil in the normal rendering pass.</p></li>
<li><p>URP: Fixed an issue where _AfterPostProcessTexture was no longer being assigned in UniversalRenderer.</p></li>
<li><p>URP: Fixed an issue with MSAA falling back to the incorrect value when sample count 2 is not supported on some Android GPUs.</p></li>
<li><p>URP: Fixed an issue with too many variants being included in ShaderGraph shaders used in URP.</p></li>
<li><p>URP: Fixed camera sorting layer render target not being allocated in the 2d renderer.</p></li>
<li><p>URP: Fixed CopyDepthPass incorrectly always enqueued when deferred rendering mode was enabled when it should depends on the pipeline asset settings.</p></li>
<li><p>URP: Fixed decal compilation issue on mac.</p></li>
<li><p>URP: Fixed decals to work with native render pass. (<a href="https://issuetracker.unity3d.com/issues/urp-decals-are-not-visible-in-game-view-after-modifying-urp-asset-properties">1353141</a>)</p></li>
<li><p>URP: Fixed disabled debug lighting modes on Vulkan and OpenGL following a shader compiler fix.</p></li>
<li><p>URP: Fixed for rendering thumbnails.</p></li>
<li><p>URP: Fixed graphical artefact when terrain height map is used with rendering layer mask for lighting.</p></li>
<li><p>URP: Fixed incorrect behavior of Reflections with Smoothness lighting debug mode.</p></li>
<li><p>URP: Fixed incorrect shadow batching and shadow length.</p></li>
<li><p>URP: Fixed indentation of Emission map on material editor.</p></li>
<li><p>URP: Fixed inspector documentation URLs for the URP asset and Universal Renderer asset.</p></li>
<li><p>URP: Fixed inspector documentation URLs to the SSAO, Decal, and Render Objects renderer features.</p></li>
<li><p>URP: Fixed lit detail correctly upgraded from standard shader. (<a href="https://issuetracker.unity3d.com/issues/urp-detail-map-tiling-is-tied-to-base-texture-tiling">1323725</a>)</p></li>
<li><p>URP: Fixed memory leak with XR combined occlusion meshes.</p></li>
<li><p>URP: Fixed property wrappers around material properties.</p></li>
<li><p>URP: Fixed sceneview debug mode rendering.</p></li>
<li><p>URP: Fixed ScreenSpaceShadows target which was not bound during draw. (<a href="https://issuetracker.unity3d.com/issues/directional-light-shadows-are-not-displayed-if-screen-space-shadows-are-on">1388353</a>)</p></li>
<li><p>URP: Fixed shaderGraph shaders to render into correct depthNormals passes when deferred rendering mode and SSAO are enabled.</p></li>
<li><p>URP: Fixed ShadowCaster now requires varying normalWS to include changed normals from vertex shader in shader graph.</p></li>
<li><p>URP: Fixed soft shadows shader variants not set to multi_compile_fragment on some shaders (gbuffer pass, speedtree shaders, WavingGrass shader).</p></li>
<li><p>URP: Fixed some rendering inconsistencies when using Decals.</p></li>
<li><p>URP: Fixed typo in numIterationsEnclosingSphere api name.</p></li>
<li><p>URP: MotionVector fix when using Native RenderPass. (1348528)</p></li>
<li><p>URP: Removed the name input for the SSAO and Screen Space Shadows renderer features.</p></li>
<li><p>Version Control: Fixed a bug where the Texture2D error would pop up after downloading a project<br> Fixed a bug when context menu would sometimes disappear<br>
Fixed small textbox on checkin dialog when launched from context menu<br>
Fixed a workspace NullReferenceException bug<br>
Fixed notification icon not showing on Plastic window<br>
Fixed auto login errors not showing up for users<br>
Fixed unexpected error message after user switched workspace to a label.</p></li>
<li><p>Version Control: Fixed a console error when selecting object in Scene view hierarchy or creating a new asset.</p></li>
<li><p>Version Control: Fixed capitalization of Pending Changes and File History tab names<br> Fixed the amount of spacing after the Item column title in the Pending Changes tab<br>
Removed pin striping from line items in File History tab<br>
Fixed project view context menu and icons missing after Collaborate project migration<br>
Fixed migrated projects not downloading correctly from Unity Hub.</p></li>
<li><p>Version Control: Fixed contextual menu not showing up in project view.</p></li>
<li><p>Version Control: Fixed inverted text for the force checkout option<br> Fixed typing capital O in checkin comment would open the selected item<br>
Fixed loading indicator not centered on Plastic SCM installation window<br>
Fixed installing Plastic SCM would sign out user from the plugin<br>
Removed extra refresh button on Gluon's Incoming Changes tab<br>
Fixed loading indicator not centered on Plastic SCM installation window<br>
Fixed missing Plastic SCM window option when user is not signed in on Unity Hub<br>
Removed meta file warning message for the deleted Beta folder<br>
Fixed Plastic SCM menu missing from Project view context menu.</p></li>
<li><p>Version Control: Fixed light theme icons used in dark theme after pulling incoming changes<br> Fixed "Input string was not in a correct format" error.</p></li>
<li><p>Version Control: Fixed Newtonsoft.Json.dll conflicts with other external packages<br> Fixed editor objects count increasing when hovering over Plastic window or toolbar button<br>
Fixed ArgumentOutOfRange exception when creating a branch<br>
Fixed scene reloading not happening after creating a new branch.</p></li>
<li><p>Version Control: Fixed NullReferenceException after closing the Plastic SCM window.</p></li>
<li><p>Version Control: Fixed performance regression in large projects due to FindObjectsOfTypeAll calls<br> Fixed working mode error after migration from Unity Collaborate.</p></li>
<li><p>Version Control: Fixed Plastic X not opening from plugin menu<br> Fixed error when trying to invite members to proect<br>
Fixed editor unhandled errors being hijacked by the plugin<br>
Fixed toolbar icon not displaying incoming changes notification when Plastic window is closed<br>
Fixed VCCache::instance != NULL error when opening a project with Plastic window opened.</p></li>
<li><p>Version Control: Fixed some namespace collisions with Antlr3.</p></li>
<li><p>Version Control: Fixed SSO renew token after password change.</p></li>
<li><p>Version Control: Fixed UI overlays in Project view missing on changed assets when force checkout is disabled.</p></li>
<li><p>Version Control: Fixed view not switching to workspace after creating an Enterprise Gluon workspace.</p></li>
<li><p>Version Control: Renamed the CoreServices namespace so it doesn't conflict<br> Fixed some situations where the history window would be blank<br>
Fixed missing Enterprise login link<br>
Fixed low resolution icons in light theme.</p></li>
<li><p>Version Control: The problem to display Checkout button for package.json files is solved. (<a href="https://issuetracker.unity3d.com/issues/perforce-when-editing-a-package-dot-json-the-editor-checks-out-the-meta-file-not-the-asset-file">1332659</a>)</p></li>
<li><p>VFX Graph: Added a missing paste option in the context menu for VFX contexts. Also the paste options is now disabled when uneffective.</p></li>
<li><p>VFX Graph: Allows for attribute-less systems. (1341789)</p></li>
<li><p>VFX Graph: Automatically offset contexts when a new node is inserted to avoid overlapping.</p></li>
<li><p>VFX Graph: Better node position when created by dragging an edge.</p></li>
<li><p>VFX Graph: Blackboard fields can now be duplicated either with a shortcut (Ctrl+D) or with a contextual menu option.</p></li>
<li><p>VFX Graph: Context labels where not displayed in the inspector except for outputs where it was always a letter, even if the user had given a custom label.</p></li>
<li><p>VFX Graph: Creating a new VFX of the same name as an already opened VFX will reuse the existing window. (<a href="https://issuetracker.unity3d.com/issues/vfx-window-can-not-be-opened-and-errors-are-thrown-when-graph-is-created-using-empty-vfx-graph-window">1382841</a>)</p></li>
<li><p>VFX Graph: Disabled text inputs were unreadable. (<a href="https://issuetracker.unity3d.com/issues/uielements-the-font-color-for-read-only-values-has-changed-making-them-unreadable">1387237</a>)</p></li>
<li><p>VFX Graph: Enabled an optimization for motion vectors, storing projected positions for vertices instead of the transform matrix.</p></li>
<li><p>VFX Graph: Enabled state of VFX blocks and operators are preserved after copy/paste.</p></li>
<li><p>VFX Graph: Exposed Parameter placement can now be moved after sanitize.</p></li>
<li><p>VFX Graph: Fixed a compilation issue when a normal is used in shadergraph for opacity with unlit output.</p></li>
<li><p>VFX Graph: Fixed a GPU hang on some initialize dispatch during dichotomy (platform specific).</p></li>
<li><p>VFX Graph: Fixed a vector truncation error in HDRP Decal template.</p></li>
<li><p>VFX Graph: Fixed an exception thrown when using WorldToLocal/LocalToWorld operators. (<a href="https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-lhs-equals-rhs-and-and-lhs-equals-res-and-and-rhs-equals-res-errors-when-using-a-worldtolocal-matrix">1335940</a>)</p></li>
<li><p>VFX Graph: Fixed an issue in the Gradient editor, Undo will now properly refresh the gradient preview (color swatches).</p></li>
<li><p>VFX Graph: Fixed an issue that attribute-less systems does not run. (1341789)</p></li>
<li><p>VFX Graph: Fixed an issue where the Eye dropper in the color fields kept updating after pressing the Esc key.</p></li>
<li><p>VFX Graph: Fixed an issue where Zoom and warning icons were blurry in the "Play Controls" and "Visual Effect Model" scene overlays.</p></li>
<li><p>VFX Graph: Fixed an issue with Eye dropper in the color fields updating after pressing the Esc key.</p></li>
<li><p>VFX Graph: Fixed bounds helper tool (automatic systems culling, world bounds computation, ...).</p></li>
<li><p>VFX Graph: Fixed Collision with Depth Buffer when using Orthographic camera.</p></li>
<li><p>VFX Graph: Fixed Collision with Depth when using a physical camera.</p></li>
<li><p>VFX Graph: Fixed incorrect buffer type for strips.</p></li>
<li><p>VFX Graph: Fixed IsFrontFace shader graph node for VFX.</p></li>
<li><p>VFX Graph: Fixed Motion vectors in XR.</p></li>
<li><p>VFX Graph: Fixed out of sync serialization of VFX assets that could cause the asset to be dirtied for no reason.</p></li>
<li><p>VFX Graph: Fixed potentially invalid value for pixel dimensions in HDRPCameraBinder.</p></li>
<li><p>VFX Graph: Fixed unexpected Spawn context execution ordering.</p></li>
<li><p>VFX Graph: Folder named with a ".vfx" extension could lead to an error on macOS. (<a href="https://issuetracker.unity3d.com/issues/errors-appear-when-reimporting-the-folder-with-dot-vfx-in-name-when-visual-effect-graph-is-installed">1385206</a>)</p></li>
<li><p>VFX Graph: HDRP Decals are not in experimental.</p></li>
<li><p>VFX Graph: In <code>Output Particle</code> blocks, shader graph exposed properties order is consistent with shader graph blackboard.</p></li>
<li><p>VFX Graph: Inspector group headers now have a better indentation and alignment.</p></li>
<li><p>VFX Graph: Minor : Static Analysis issue. (1336647)</p></li>
<li><p>VFX Graph: Particles were rendered pink with some debug modes. (<a href="https://issuetracker.unity3d.com/issues/vfx-graph-lit-output-particles-are-rendered-as-pink-textures-when-show-cascades-of-global-volume-is-enabled">1342276</a>)</p></li>
<li><p>VFX Graph: Prevent VFX Graph compilation each time a property's min/max value is changed.</p></li>
<li><p>VFX Graph: Prevent VFX re-compilation in some cases when a value has not changed.</p></li>
<li><p>VFX Graph: Properties labels do not overlap anymore.</p></li>
<li><p>VFX Graph: Removed bool from the built-in list of blittable types for GraphicsBuffer. (<a href="https://issuetracker.unity3d.com/issues/vfx-graph-graphicsbuffer-throws-error-while-processing-vfxtype-when-using-bool-in-struct">1351830</a>)</p></li>
<li><p>VFX Graph: Resize custom operator (multiply, add...) to the minimum size when changing input types.</p></li>
<li><p>VFX Graph: ShaderGraph made with new VFX SG integration where not listed when searching for a shader graph output. (<a href="https://issuetracker.unity3d.com/issues/searcher-the-new-searcher-does-not-display-shadergraphs-using-the-new-vfx-slash-sg-integration">1379523</a>)</p></li>
<li><p>VFX Graph: Show opened VFX asset in inspector when clicking in a void area and unselect node when VFX graph loose focus.</p></li>
<li><p>VFX Graph: Some operators were missing in node search window (gradient for instance).</p></li>
<li><p>VFX Graph: Sticky note title keeps the selected font size when being edited.</p></li>
<li><p>VFX Graph: Sticky notes can now be deleted through contextual manual menu.</p></li>
<li><p>VFX Graph: Texture picker lists only textures with expected dimensions (2D, 3D, Cubemap).</p></li>
<li><p>VFX Graph: VFX Graph operators keep the same width when expanded or collpased so that the button does not change position.</p></li>
<li><p>VFX Graph: VFX Subgraph operator and block windows now have dedicated icons.</p></li>
<li><p>VFX Graph: Visual Effect inspector input fields no longer lose focus anymore while typing (Random seed).</p></li>
<li><p>VFX Graph: When adding a new node/operator in the graph editor and using the search field, the search results are sorted in a smarter way.</p></li>
<li><p>Video: Fixed an exploit found in the libvpx. (1345217)</p></li>
<li><p>Video: Fixed an issue where VideoPlayer.width and height returned 0 instead of expected values. (<a href="https://issuetracker.unity3d.com/issues/macos-videoplayer-dot-width-and-height-returns-0-when-videoplayer-dot-texture-dot-width-and-height-returns-expected-values">1339883</a>)</p></li>
<li><p>Video: Fixed getting buffer overflow warning when increasing playback speed on the VideoPlayer. (<a href="https://issuetracker.unity3d.com/issues/videoplayer-buffer-overflow-warnings-when-we-start-playing-vp8-video-with-increased-playback-speed">1325295</a>)</p></li>
<li><p>Video: Material's Main Maps Tiling/Offset controls are locked when VideoPlayer is targetting the material. (<a href="https://issuetracker.unity3d.com/issues/materials-main-maps-tiling-slash-offset-controls-are-locked-when-videoplayer-is-targetting-the-material">1378047</a>)</p></li>
<li><p>Video: Reenabled VideoPlaybackPlayAllFramesWithLooping test case on UWP. (1171545)</p></li>
<li><p>Video: Video player no longer suffers performance issues in windowed mode with external monitor. (<a href="https://issuetracker.unity3d.com/issues/macos-video-loading-performance-degrades-when-app-is-in-windowed-mode-and-an-external-monitor-is-connected">1350851</a>)</p></li>
<li><p>Video: VideoPlayer throws errors when VideoClip loaded from AssetBundle nears the end. (<a href="https://issuetracker.unity3d.com/issues/videoplayer-throws-errors-when-videoclip-loaded-from-assetbundle-nears-the-end">1358843</a>)</p></li>
<li><p>Virtual Texturing: Completed requests now won't be incorrectly canceled if the last <code>InvalidateRegion</code> call is made before <code>PopRequests</code>.</p></li>
<li><p>Visual Scripting: 1.8.0 pre-release version is no longer available.</p></li>
<li><p>Visual Scripting: AOT prebuild works properly when building a project in batchmode.</p></li>
<li><p>Visual Scripting: No more il2cpp crash caused by infinite recursion when generating AotStubs.</p></li>
<li><p>Visual Scripting: No more jitter on fuzzy finder.</p></li>
<li><p>Visual Scripting: No more missing icons when the "Transition End Arrow" is on.</p></li>
<li><p>Visual Scripting: No more missing textures after switching platform.</p></li>
<li><p>Visual Scripting: Restoring the public icon set api.</p></li>
<li><p>Visual Scripting: Variable duplication working properly.</p></li>
<li><p>Visual Scripting: Welcome Screen opens the proper graph.</p></li>
<li><p>WebGL: Added workarounds for various Safari Web Audio bugs playing back compressed and looping audio clips. Fixed a regression in Unity audio backend that could cause an incorrect audio volume to be set for &lt; 1 second duration at audio playback start time. (1360344)</p></li>
<li><p>WebGL: Fixed clearing of user template variables when template is switched. (<a href="https://issuetracker.unity3d.com/issues/webgl-template-custom-user-variables-are-cleared-when-switching-between-templates">1328657</a>)</p></li>
<li><p>WebGL: Fixed errors rendering URP scenes with WebGL. (1385451)</p></li>
<li><p>WebGL: Fixed for URP being washed out when Size Code Optimization is used in the Build Settings. (<a href="https://issuetracker.unity3d.com/issues/urp-scenes-with-post-processing-disabled-or-enabled-and-anti-aliasing-set-to-fxaa-are-over-illuminated-when-built-for-webgl">1309878</a>)</p></li>
<li><p>WebGL: Fixed insecure connection error when using "Build and Run'. (1378580)</p></li>
<li><p>WebGL: Fixed iOS touch events crashing UI Toolkit. (1365436)</p></li>
<li><p>WebGL: Removed 255 character limit for audio file urls. (<a href="https://issuetracker.unity3d.com/issues/webgl-build-crashes-when-requesting-255-character-url-with-unitywebrequestmultimedia-dot-getaudioclip">1327368</a>)</p></li>
<li><p>Windows: Added error messaging when we cannot create an Editor Window and prevented extra background task windows from opening during import. (<a href="https://issuetracker.unity3d.com/issues/background-task-windows-are-opened-when-importing-large-packages">1257717</a>)</p></li>
<li><p>Windows: Fixed mouse position being off-by-1 pixel when rendering at lower than native resolution in certain cases.</p></li>
<li><p>Windows: Fixed resolution resetting to native resolution on primary window when trying to move the secondary window use Display.SetParams.</p></li>
<li><p>Windows: Fixed UnityWebRequest does not respect auto proxy settings.</p></li>
</ul>
