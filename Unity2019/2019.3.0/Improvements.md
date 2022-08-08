# Unity 2019.3.0

https://unity3d.com/unity/whats-new/2019.3.0

## Improvements



*   2D: Add multiple texture support to Sprite Shape Renderer.
    
*   2D: Added multiple texture support to Tilemap Renderer.
    
*   2D: Reduced memory usage of a Tilemap Tile by 16 bytes.
    
*   Android: Android: When "Installed with Unity (recommended)" is selected in Editor Tools Preferences window, display the path where the tool should be located.
    
*   Android: Custom UnityPlayerActivity implementations can now modify the command line arguments passed to Unity during startup.
    
*   Android: Improved stacktrace resolving performance by up to 30% on ARM64 Il2CPP (stacktrace resolving occurs in cases like - exception is thrown, or Debug.Log\* is called, etc)
    
*   Android: Make use of ASTC decode mode OpenGL and Vulkan extension for LDR textures
    
*   Android: Unity now uses cpu\_capacity for big.LITTLE core detection on devices where the Linux kernel supports it.
    
*   Android: You can now install Android OpenJDK via Unity Hub as a separate optional component. This reduces Android support size.
    
*   Animation: Added a sorting order to Animation Playable Output to control how Playable Graphs execute in the Animator.
    
*   Animation: Exposed keyframe reduction options on GameObjectRecorder.SaveToClip().
    
*   Animation: Limited curve dragging in curve editor to only be available when pressing down the Shift key.
    
*   Audio: Better error reporting when audio clips fail to play ([1118840](https://issuetracker.unity3d.com/issues/audio-audio-mainthread-check-internal-crashes-when-trying-to-load-corrupted-audioclips))
    
*   Audio: Faster import of audio files
    
*   Build Pipeline: Added BuildAssetBundleOptions entry that allows stripping the Unity version from built asset bundles.
    
*   Build Pipeline: LZ4 lib version updated to 1.9.1
    
*   Build Pipeline: LZMA lib version updated to 19.00
    
*   Editor: 2D and 3D primitive collider tools are now Editor tools, compatible with the Scene toolbar, and top left toolbar.
    
*   Editor: 3D joint tools are now Editor tools.
    
*   Editor: 3D primitive collider tools are now Editor tools.
    
*   Editor: Added **Enable Code Coverage** option in General Preferences. Added a popup and a console warning to notify users that enabling coverage lowers performance. Enabling coverage displays **\[CODE COVERAGE\]** in the window title bar.
    
*   Editor: Added a shortcut for the Scene Visibility **Show All** command.
    
*   Editor: Added shortcus for SceneView Camera modes.
    
*   Editor: Added support for generics to `UnityEditor.TypeCache` API
    
*   Editor: Added `EditorSceneManager.sceneDirtied` and `PrefabStage.prefabStageDirtied` callbacks, that are called when a user modifies a previously unmodified Scene/Prefab.
    
*   Editor: Made terminology for refer to the new and old input systems in Player Settings consistent: "Input System Package" and "Input Manager".
    
*   Editor: Show an info box in the old Input settings suggesting to use the new one (and _strongly_ suggesting so if the old input system backend is turned off).
    
*   Editor: Special Thanks to beta users
    
*   Editor: The context menu **Copy** command now works on disabled Text, Float, and Color fields. ([1180207](https://issuetracker.unity3d.com/issues/vcs-material-inspector-header-most-entries-should-be-enabled-for-non-checked-out-materials-same-for-many-other-inspectors))
    
*   GI: Added extra verification for Experimental.Lightmapping.SetCustomBakeInputs API.
    
*   GI: Added support for scaling Light Probe sample counts with the lightmap sample counts. A multiplier is added to adjust the Light Probe sample counts vs. lightmap sample counts. ([1135553](https://issuetracker.unity3d.com/issues/light-probes-are-very-inconsistent-in-indirectly-lit-scenes))
    
*   GI: GPU lightmapper: Match CPU lightmapper sampling scheme for improved quality.
    
*   GI: Improved performance by making Unity only denoise the Ambient Occlusion buffer when Ambient Occlusion is enabled.
    
*   GI: Increased the responsiveness of the Editor during baking with the Progressive GPU Lightmapper with AMD GPUs.
    
*   GI: ReceiveGI.LightProbes objects no display in the Lightmap indices visualisation view.
    
*   GI: Reduced overhead in compositing when baking lightmaps with the Progressive GPU Lightmapper.
    
*   GI: Rreduced main thread overhead of the baking pipeline.
    
*   Graphics: Bind constant buffer is now supported on OpenGL 4.3+ and OpenGL ES 3.1+.
    
*   Graphics: Exposed hardware-specific device limits for binding compute buffers in different shader stages.
    
*   Graphics: Exposed hardware-specific device limits for compute shader thread group sizes.
    
*   Graphics: Frame debugger now works even if graphics jobs are enabled (except for direct graphics jobs) (1182399)
    
*   Graphics: Graphics: Mesh scripting API improvements. Added non-alloc overload of GetVertexAttributes. Added NativeArray overloads of Mesh.SetFoo. Added T\[\] and List<T> overloads of SetVertexBufferData and SetIndexBufferData
    
*   Graphics: Improved error logging in case ETC texture compression fails in the Editor
    
*   Graphics: Improved sRGB fallback to unorm format warning to explain how to silent it. (1127043)
    
*   Graphics: Inspector operations like selecting, editing, undo on large assets (Texture3D, Texture2DArray etc.) is much smoother now
    
*   Graphics: Made changes so that `EncodeToPNG()` supports the 16-bit grayscale format.
    
*   Graphics: Mesh class got HasVertexAttribute and GetVertexAttributeDimension methods.
    
*   Graphics: Mesh class got slice-style setters, e.g. SetVertices(Vector3\[\] data, int start, int length).
    
*   Graphics: Mesh class SetIndices/GetIndices got 16-bit index format overloads.
    
*   Graphics: Metal: improved debug groups structure
    
*   Graphics: Optimized away a redundant memory copy in Mesh.GetIndices implementation.
    
*   Graphics: Remove (Experimental) tag from Graphics Jobs setting and make it a per platform setting
    
*   Graphics: SetPixelData API was added to Texture2D, Texture2DArray, Texture3D, Cubemap and CubemapArray classes to allow setting raw texture data directly. This works in a similar way to Texture2D. LoadRawTextureData, but instead of having to precalculate data offset and size, the data can be copied directly to a particular miplevel/array element/cubemap face. ([1162624](https://issuetracker.unity3d.com/issues/its-not-possible-to-create-texture2darray-with-compression-because-it-doesnt-have-setrawtexturedata-slash-getrawtexturedata))
    
*   Graphics: Texture mip map streaming system now exposes calculated mipmapLevel via Texture2D.calculatedMipmapLevel (unaffected by requestedMipmapLevel or minimumMipMapLevel)  
    Texture mip map streaming system now supports Texture2D.minimumMipmapLevel for per texture control of the minimum mip that will be selected.  
    Fixed race condition in mip map streaming calculation that could cause Texture2D.desiredMipmapLevel value to be incorrect if read while the job was still running. (1153431)
    
*   Graphics: Texture2D.CreateExternalTexture now also accepts ID3D11Texture2D (DX11) and ID3D12Resource (DX12).
    
*   Graphics: Vastly decreases the time taken when a Ray Tracing shader is executed for the first time or a particular shader code or configuration associated to a Ray Tracing dispatch has changed.
    
*   Graphics: Vulkan texture creation during async load optimised to remove hitches for large textures
    
*   Graphics: \[metal\] iOS native resolution is now same as render resolution int most cases, this way avoiding final blit
    
*   iOS: Minimum supported iOS version is now iOS 10.
    
*   iOS: Unity now warns you if you try to render MeshTopology.Points on Metal with shaders that don't have PSIZE output.
    
*   Kernel: Improve main thread utilisation for IJobParallelFor jobs
    
*   Kernel: Introducing new serialization attribute: SerializeReference
    
*   macOS: \[metal\] Added initial Graphics Jobs implementation on iOS and macOS platforms
    
*   Package Manager: Added a new `git` attribute to the `PackageManager.PackageInfo` C# class  
    (https://docs.unity3d.com/ScriptReference/PackageManager.PackageInfo.html).
    
*   Package Manager: Added conflict resolution information logging in the `upm.log` during the `resolve` operation.
    
*   Package Manager: Added menu extension to add new items to the Package Manager UI.
    
*   Package Manager: Added support for the SCP format (for example, `git@github.com:user/repo.git`) when using Git-based packages.
    
*   Package Manager: Conflicts are no longer reported as errors when the requested dependency of a package is satisfied by a greater major version.
    
*   Package Manager: Deprecated the Package Manager UI as a package.
    
*   Package Manager: Grouped Assets in separate pages for the "My Assets" filter in the Package Manager UI.
    
*   Package Manager: Reduced the Editor's LastLayout file size.
    
*   Package Manager: Warn the user when they try to enter Play mode while downloading Assets from the AssetStore.  
    Warn the user when they try to start downloading a package from the AssetStore while are in Play mode.
    
*   Particles: Expose the "particle" property in the EmitParams, so users can easily override every proeprty of emitted particles.
    
*   Physics: Reduce the number of calls to Transform-Dispatch system (shown as "TransformChangedDispatch" in profiler) per Physics2D.Simulate call. (1185425)
    
*   Profiler: Added a Remember Last Recording State option to the Preferences Window to toggle the Profiler's behavior between remembering the Record button state within a session, or remembering it across sessions on the same machine.
    
*   Profiler: Added Frame Count to the Profiler Preferences to adjust the visible frame count in Profiler Window.
    
*   Profiler: Added thread dropdown to Hierachy View of the Profiler window.
    
*   Profiler: Improved information about Shader compilation in the Profiler.
    
*   Profiler: Reduced the Profiler overhead when flushing data from Job threads.
    
*   Profiler: Reworked Profiler toolbar and rearranged buttons:  
    
    *   Profile Editor button has been removed. You can now select Editor as a Target.  
        
    *   Record, Save As, Load, and Current are now icon buttons.  
        
    *   Allocation Callstacks has been renamed to Call Stacks  
        
    *   Added Open Manual and an overflow menu button that contains Color Blind mode and a link to Profiler Preferences.
*   Scripting: Added project name to the boot.config file for Players. This will enable popular IDE's to display more information about the Player when attaching a debugger.
    
*   Scripting: Added support for the "||" (OR) operator for the define constraints in the .asmdef importer
    
*   Scripting: Improved icons for the validity of Define Constraints in the Asmdef Importer Inspector.
    
*   Scripting: Throw exceptions when calling old Input APIs but the old input system is turned off.
    
*   Shaders: Added an checkbox in Graphics Settings to enable logging information about shader compilation at runtime (development and debug only).
    
*   Shaders: Added warning if duplicated global and local keyword is used
    
*   Shaders: Adding for C# keyword stripping local keywords support. Improving performance for variant shader variant finding
    
*   Terrain: Added support for arbitrarily-sized Terrain Paint Contexts so that they are no longer limited to 2x2 tiles.
    
*   Terrain: Made changes so that painting and setting Terrain height always uses world space coordinates. ([1118605](https://issuetracker.unity3d.com/issues/height-of-the-terrain-is-calculated-without-using-y-position-of-the-gameobject-when-setting-height-in-terrain-component))
    
*   Timeline: Scrolling horizontally with either the mouse wheel or track pad now pans horizontally in Timeline's clips area.
    
*   Timeline: Scrolling with either the mouse wheel or track pad is now context-sensitive in Timeline. It zooms if the pointer is above the clips area, it pans everywhere else.
    
*   UI Elements: Extended the `Image` class and the `background-image` property to support SVG image assets.
    
*   UI Elements: Improved performance of picking operations (1194971)
    
*   UI Elements: ListView is now bindable via C# and UXML.
    
*   UI Elements: On SM3.5+, both point and bilinear textures will be elligible to enter the automatic atlas (if the other criterias such as size are fulfilled as well). Below SM3.5, only bilinear sampling is required and using point sampling will break batches.
    
*   Universal Windows Platform: Added 'GazeInput' Capability to UWP Publisher Settings within the Editor (1162038)
    
*   Universal Windows Platform: Added warning in Player Settings inspector for when when selected icons are too large and will fail Windows App Certification Kit tests ([1146113](https://issuetracker.unity3d.com/issues/uwp-warring-should-be-thrown-in-the-console-when-adding-large-store-icon))
    
*   Version Control: Added "-vcsMode" editor command line argument to set VCS mode.
    
*   Version Control: Added a confirmation dialog for moving or renaming folders under version control (1108630)
    
*   Version Control: Added AssetDatabase.MakeEditable to public API.
    
*   Version Control: Asset and Project Settings inspector context menus (e.g. Material "Select/Edit Shader") now work on non-checked out assets ([1180207](https://issuetracker.unity3d.com/issues/vcs-material-inspector-header-most-entries-should-be-enabled-for-non-checked-out-materials-same-for-many-other-inspectors))
    
*   Version Control: If a successful server connection gets lost, the editor tries to automatically reconnect for a while ([1184060](https://issuetracker.unity3d.com/issues/vcs-improve-perforce-disconnection-workflow-auto-reconnect-better-work-offline-discovery-etc-dot))
    
*   Version Control: Inspector object reference fields context menus have "Check Out" entry when they point to an asset that is not checked out ([1145194](https://issuetracker.unity3d.com/issues/vcs-a2-object-reference-fields-and-inspector-vcs-status-bar-should-have-version-control-context-menu-on-them))
    
*   Version Control: Inspector VCS status bar was moved to the top, and in addition to "Checkout" got "Add", "Lock", "Unlock", "Submit" buttons when appropriate.
    
*   Version Control: VCS setting inspector fields have recently used value dropdowns on them
    
*   Video: On WebGL, videos with non-square pixel aspect ratio now displayed correctly.