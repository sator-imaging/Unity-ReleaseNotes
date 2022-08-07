# Unity 2019.3.0
https://unity3d.com/unity/whats-new/2019.3.0

## Improvements

<ul>
<li><p>2D: Add multiple texture support to Sprite Shape Renderer.</p></li>
<li><p>2D: Added multiple texture support to Tilemap Renderer.</p></li>
<li><p>2D: Reduced memory usage of a Tilemap Tile by 16 bytes.</p></li>
<li><p>Android: Android: When "Installed with Unity (recommended)" is selected in Editor Tools Preferences window, display the path where the tool should be located.</p></li>
<li><p>Android: Custom UnityPlayerActivity implementations can now modify the command line arguments passed to Unity during startup.</p></li>
<li><p>Android: Improved stacktrace resolving performance by up to 30% on ARM64 Il2CPP (stacktrace resolving occurs in cases like - exception is thrown, or Debug.Log* is called, etc)</p></li>
<li><p>Android: Make use of ASTC decode mode OpenGL and Vulkan extension for LDR textures</p></li>
<li><p>Android: Unity now uses cpu_capacity for big.LITTLE core detection on devices where the Linux kernel supports it.</p></li>
<li><p>Android: You can now install Android OpenJDK  via Unity Hub as a separate optional component. This reduces Android support size.</p></li>
<li><p>Animation: Added a sorting order to Animation Playable Output to control how Playable Graphs execute in the Animator.</p></li>
<li><p>Animation: Exposed keyframe reduction options on GameObjectRecorder.SaveToClip().</p></li>
<li><p>Animation: Limited curve dragging in curve editor to only be available when pressing down the Shift key.</p></li>
<li><p>Audio: Better error reporting when audio clips fail to play (<a href="https://issuetracker.unity3d.com/issues/audio-audio-mainthread-check-internal-crashes-when-trying-to-load-corrupted-audioclips">1118840</a>)</p></li>
<li><p>Audio: Faster import of audio files</p></li>
<li><p>Build Pipeline: Added BuildAssetBundleOptions entry that allows stripping the Unity version from built asset bundles.</p></li>
<li><p>Build Pipeline: LZ4 lib version updated to 1.9.1</p></li>
<li><p>Build Pipeline: LZMA lib version updated to 19.00</p></li>
<li><p>Editor: 2D and 3D primitive collider tools are now Editor tools, compatible with the Scene toolbar, and top left toolbar.</p></li>
<li><p>Editor: 3D joint tools are now Editor tools.</p></li>
<li><p>Editor: 3D primitive collider tools are now Editor tools.</p></li>
<li><p>Editor: Added <strong>Enable Code Coverage</strong> option in General Preferences. Added a popup and a console warning to notify users that enabling coverage lowers performance. Enabling coverage displays <strong>[CODE COVERAGE]</strong>  in the window title bar.</p></li>
<li><p>Editor: Added a shortcut for the Scene Visibility <strong>Show All</strong> command.</p></li>
<li><p>Editor: Added shortcus for SceneView Camera modes.</p></li>
<li><p>Editor: Added support for generics to <code>UnityEditor.TypeCache</code> API</p></li>
<li><p>Editor: Added <code>EditorSceneManager.sceneDirtied</code> and <code>PrefabStage.prefabStageDirtied</code> callbacks, that are called when a user modifies a previously unmodified Scene/Prefab.</p></li>
<li><p>Editor: Made terminology for refer to the new and old input systems in Player Settings consistent: "Input System Package" and "Input Manager".</p></li>
<li><p>Editor: Show an info box in the old Input settings suggesting to use the new one (and <em>strongly</em> suggesting so if the old input system backend is turned off).</p></li>
<li><p>Editor: Special Thanks to beta users</p></li>
<li><p>Editor: The context menu <strong>Copy</strong> command now works on disabled Text, Float, and Color fields. (<a href="https://issuetracker.unity3d.com/issues/vcs-material-inspector-header-most-entries-should-be-enabled-for-non-checked-out-materials-same-for-many-other-inspectors">1180207</a>)</p></li>
<li><p>GI: Added extra verification for Experimental.Lightmapping.SetCustomBakeInputs API.</p></li>
<li><p>GI: Added support for scaling Light Probe sample counts with the lightmap sample counts. A multiplier is added to adjust the Light Probe sample counts vs. lightmap sample counts. (<a href="https://issuetracker.unity3d.com/issues/light-probes-are-very-inconsistent-in-indirectly-lit-scenes">1135553</a>)</p></li>
<li><p>GI: GPU lightmapper: Match CPU lightmapper sampling scheme for improved quality.</p></li>
<li><p>GI: Improved performance by making Unity only denoise the Ambient Occlusion buffer when Ambient Occlusion is enabled.</p></li>
<li><p>GI: Increased the responsiveness of the Editor during baking with the Progressive GPU Lightmapper with AMD GPUs.</p></li>
<li><p>GI: ReceiveGI.LightProbes objects no display in the Lightmap indices visualisation view.</p></li>
<li><p>GI: Reduced overhead in compositing when baking lightmaps with the Progressive GPU Lightmapper.</p></li>
<li><p>GI: Rreduced main thread overhead of the baking pipeline.</p></li>
<li><p>Graphics: Bind constant buffer is now supported on OpenGL 4.3+ and OpenGL ES 3.1+.</p></li>
<li><p>Graphics: Exposed hardware-specific device limits for binding compute buffers in different shader stages.</p></li>
<li><p>Graphics: Exposed hardware-specific device limits for compute shader thread group sizes.</p></li>
<li><p>Graphics: Frame debugger now works even if graphics jobs are enabled (except for direct graphics jobs) (1182399)</p></li>
<li><p>Graphics: Graphics: Mesh scripting API improvements. Added non-alloc overload of GetVertexAttributes. Added NativeArray overloads of Mesh.SetFoo. Added T[] and List&lt;T&gt; overloads of SetVertexBufferData and SetIndexBufferData</p></li>
<li><p>Graphics: Improved error logging in case ETC texture compression fails in the Editor</p></li>
<li><p>Graphics: Improved sRGB fallback to unorm format warning to explain how to silent it. (1127043)</p></li>
<li><p>Graphics: Inspector operations like selecting, editing, undo on large assets (Texture3D, Texture2DArray etc.) is much smoother now</p></li>
<li><p>Graphics: Made changes so that <code>EncodeToPNG()</code> supports the 16-bit grayscale format.</p></li>
<li><p>Graphics: Mesh class got HasVertexAttribute and GetVertexAttributeDimension methods.</p></li>
<li><p>Graphics: Mesh class got slice-style setters, e.g. SetVertices(Vector3[] data, int start, int length).</p></li>
<li><p>Graphics: Mesh class SetIndices/GetIndices got 16-bit index format overloads.</p></li>
<li><p>Graphics: Metal: improved debug groups structure</p></li>
<li><p>Graphics: Optimized away a redundant memory copy in Mesh.GetIndices implementation.</p></li>
<li><p>Graphics: Remove (Experimental) tag from Graphics Jobs setting and make it a per platform setting</p></li>
<li><p>Graphics: SetPixelData API was added to Texture2D, Texture2DArray, Texture3D, Cubemap and CubemapArray classes to allow setting raw texture data directly. This works in a similar way to Texture2D. LoadRawTextureData, but instead of having to precalculate data offset and size, the data can be copied directly to a particular miplevel/array element/cubemap face. (<a href="https://issuetracker.unity3d.com/issues/its-not-possible-to-create-texture2darray-with-compression-because-it-doesnt-have-setrawtexturedata-slash-getrawtexturedata">1162624</a>)</p></li>
<li><p>Graphics: Texture mip map streaming system now exposes calculated mipmapLevel via Texture2D.calculatedMipmapLevel (unaffected by requestedMipmapLevel or minimumMipMapLevel)<br> Texture mip map streaming system now supports Texture2D.minimumMipmapLevel for per texture control of the minimum mip that will be selected.<br>
Fixed race condition in mip map streaming calculation that could cause Texture2D.desiredMipmapLevel value to be incorrect if read while the job was still running.
(1153431)</p></li>
<li><p>Graphics: Texture2D.CreateExternalTexture now also accepts ID3D11Texture2D (DX11) and ID3D12Resource (DX12).</p></li>
<li><p>Graphics: Vastly decreases the time taken when a Ray Tracing shader is executed for the first time or a particular shader code or configuration associated to a Ray Tracing dispatch has changed.</p></li>
<li><p>Graphics: Vulkan texture creation during async load optimised to remove hitches for large textures</p></li>
<li><p>Graphics: [metal] iOS native resolution is now same as render resolution int most cases, this way avoiding final blit</p></li>
<li><p>iOS: Minimum supported iOS version is now iOS 10.</p></li>
<li><p>iOS: Unity now warns you if you try to render MeshTopology.Points on Metal with shaders that don't have PSIZE output.</p></li>
<li><p>Kernel: Improve main thread utilisation for IJobParallelFor jobs</p></li>
<li><p>Kernel: Introducing new serialization attribute: SerializeReference</p></li>
<li><p>macOS: [metal] Added initial Graphics Jobs implementation on iOS and macOS platforms</p></li>
<li><p>Package Manager: Added a new <code>git</code> attribute to the <code>PackageManager.PackageInfo</code> C# class<br> (https://docs.unity3d.com/ScriptReference/PackageManager.PackageInfo.html).</p></li>
<li><p>Package Manager: Added conflict resolution information logging in the <code>upm.log</code> during the <code>resolve</code> operation.</p></li>
<li><p>Package Manager: Added menu extension to add new items to the Package Manager UI.</p></li>
<li><p>Package Manager: Added support for the SCP format (for example, <code>git@github.com:user/repo.git</code>) when using Git-based packages.</p></li>
<li><p>Package Manager: Conflicts are no longer reported as errors when the requested dependency of a package is satisfied by a greater major version.</p></li>
<li><p>Package Manager: Deprecated the Package Manager UI as a package.</p></li>
<li><p>Package Manager: Grouped Assets in separate pages for the "My Assets" filter in the Package Manager UI.</p></li>
<li><p>Package Manager: Reduced the Editor's LastLayout file size.</p></li>
<li><p>Package Manager: Warn the user when they try to enter Play mode while downloading Assets from the AssetStore.<br> Warn the user when they try to start downloading a package from the AssetStore while are in Play mode.</p></li>
<li><p>Particles: Expose the "particle" property in the EmitParams, so users can easily override every proeprty of emitted particles.</p></li>
<li><p>Physics: Reduce the number of calls to Transform-Dispatch system (shown as "TransformChangedDispatch" in profiler) per Physics2D.Simulate call. (1185425)</p></li>
<li><p>Profiler: Added a Remember Last Recording State option to the Preferences Window to toggle the Profiler's behavior between remembering the Record button state within a session, or remembering it across sessions on the same machine.</p></li>
<li><p>Profiler: Added Frame Count to the Profiler Preferences to adjust the visible frame count in Profiler Window.</p></li>
<li><p>Profiler: Added thread dropdown to Hierachy View of the Profiler window.</p></li>
<li><p>Profiler: Improved information about Shader compilation in the Profiler.</p></li>
<li><p>Profiler: Reduced the Profiler overhead when flushing data from Job threads.</p></li>
<li><p>Profiler: Reworked Profiler toolbar and rearranged buttons:<br></p> 
<ul>
<li>Profile Editor button has been removed. You can now select Editor as a Target.<br></li>
<li>Record, Save As, Load, and Current are now icon buttons.<br></li>
<li>Allocation Callstacks has been renamed to Call Stacks<br></li>
<li>Added Open Manual and an overflow menu button that contains Color Blind mode and a link to Profiler Preferences.</li>
</ul></li>
<li><p>Scripting: Added project name to the boot.config file for Players. This will enable popular IDE's to display more information about the Player when attaching a debugger.</p></li>
<li><p>Scripting: Added support for the "||" (OR) operator for the define constraints in the .asmdef importer</p></li>
<li><p>Scripting: Improved icons for the validity of Define Constraints in the Asmdef Importer Inspector.</p></li>
<li><p>Scripting: Throw exceptions when calling old Input APIs but the old input system is turned off.</p></li>
<li><p>Shaders: Added an checkbox in Graphics Settings to enable logging information about shader compilation at runtime (development and debug only).</p></li>
<li><p>Shaders: Added warning if duplicated global and local keyword is used</p></li>
<li><p>Shaders: Adding for C# keyword stripping local keywords support. Improving performance for variant shader variant finding</p></li>
<li><p>Terrain: Added support for arbitrarily-sized Terrain Paint Contexts so that they are no longer limited to 2x2 tiles.</p></li>
<li><p>Terrain: Made changes so that painting and setting Terrain height always uses world space coordinates. (<a href="https://issuetracker.unity3d.com/issues/height-of-the-terrain-is-calculated-without-using-y-position-of-the-gameobject-when-setting-height-in-terrain-component">1118605</a>)</p></li>
<li><p>Timeline: Scrolling horizontally with either the mouse wheel or track pad now pans horizontally in Timeline's clips area.</p></li>
<li><p>Timeline: Scrolling with either the mouse wheel or track pad is now context-sensitive in Timeline. It zooms if the pointer is above the clips area, it pans everywhere else.</p></li>
<li><p>UI Elements: Extended the <code>Image</code> class and the <code>background-image</code> property to support SVG image assets.</p></li>
<li><p>UI Elements: Improved performance of picking operations (1194971)</p></li>
<li><p>UI Elements: ListView is now bindable via C# and UXML.</p></li>
<li><p>UI Elements: On SM3.5+, both point and bilinear textures will be elligible to enter the automatic atlas (if the other criterias such as size are fulfilled as well). Below SM3.5, only bilinear sampling is required and using point sampling will break batches.</p></li>
<li><p>Universal Windows Platform: Added 'GazeInput' Capability to UWP Publisher Settings within the Editor (1162038)</p></li>
<li><p>Universal Windows Platform: Added warning in Player Settings inspector for when when selected icons are too large and will fail Windows App Certification Kit tests (<a href="https://issuetracker.unity3d.com/issues/uwp-warring-should-be-thrown-in-the-console-when-adding-large-store-icon">1146113</a>)</p></li>
<li><p>Version Control: Added "-vcsMode" editor command line argument to set VCS mode.</p></li>
<li><p>Version Control: Added a confirmation dialog for moving or renaming folders under version control (1108630)</p></li>
<li><p>Version Control: Added AssetDatabase.MakeEditable to public API.</p></li>
<li><p>Version Control: Asset and Project Settings inspector context menus (e.g. Material "Select/Edit Shader") now work on non-checked out assets (<a href="https://issuetracker.unity3d.com/issues/vcs-material-inspector-header-most-entries-should-be-enabled-for-non-checked-out-materials-same-for-many-other-inspectors">1180207</a>)</p></li>
<li><p>Version Control: If a successful server connection gets lost, the editor tries to automatically reconnect for a while (<a href="https://issuetracker.unity3d.com/issues/vcs-improve-perforce-disconnection-workflow-auto-reconnect-better-work-offline-discovery-etc-dot">1184060</a>)</p></li>
<li><p>Version Control: Inspector object reference fields context menus have "Check Out" entry when they point to an asset that is not checked out (<a href="https://issuetracker.unity3d.com/issues/vcs-a2-object-reference-fields-and-inspector-vcs-status-bar-should-have-version-control-context-menu-on-them">1145194</a>)</p></li>
<li><p>Version Control: Inspector VCS status bar was moved to the top, and in addition to "Checkout" got "Add", "Lock", "Unlock", "Submit" buttons when appropriate.</p></li>
<li><p>Version Control: VCS setting inspector fields have recently used value dropdowns on them</p></li>
<li><p>Video: On WebGL, videos with non-square pixel aspect ratio now displayed correctly.</p></li>
</ul>
