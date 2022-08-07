# Unity 2019.2.0
https://unity3d.com/unity/whats-new/2019.2.0

## Improvements

<ul>
<li><p>2D: Added a toggle switch to the Grid Brush for a mode to change Z Positions of Tiles.</p></li>
<li><p>2D: Added multitexture support to SpriteShapeRenderer.</p></li>
<li><p>2D: Added multitexture support to TilemapRenderer.</p></li>
<li><p>2D: Added the CreateTileFromPaletteAttribute to allow users to specify how and what Tiles are created when dragging Assets onto the Tile Palette window.</p></li>
<li><p>2D: Exposed GridPaintingState APIs to allow users to programatically change Tile Palette Painting states</p></li>
<li><p>2D: Users can now convert Prefabs to Tile Palettes by dragging a valid Prefab onto the Tile Palette window.</p></li>
<li><p>Android: Enabled Vulkan support for Optimized frame pacing on Android.</p></li>
<li><p>Android: Implemented Screen.Brightness property for Android (read-only).</p></li>
<li><p>Android: Improved performance of string marshaling between C# and Java (up to 50% faster).</p></li>
<li><p>Android: Moved AndroidJava* and AndroidJNI APIs to built-in package AndroidJNI.</p></li>
<li><p>Android: Reduced armv7 code size by 20% by enabling thumb.</p></li>
<li><p>Android: Small reduction in job overhead when few cores are being used.</p></li>
<li><p>Android: The Unity video player can now be used with the Vulkan renderer.</p></li>
<li><p>Android: When set to true, you can mimic TouchScreenKeyboard.hideInput by drawing an input field outside the screen.</p></li>
<li><p>Animation: Added a contextual menu option that jumps to a specific AnimatorController State while liveLinked is enabled.</p></li>
<li><p>Animation: Added a selection filter that shows properties and animation curves for only the selected GameObjects.</p></li>
<li><p>Animation: Added an option to hide read-only clip properties and animation curves in the Animation window, to improve performance.</p></li>
<li><p>Animation: Added visibility feedback to the Animator Inspector.</p></li>
<li><p>Animation: Added visual feedback and keyboard shortcuts for the Ripple option in the Animation window.</p></li>
<li><p>Animation: Updated the Animation window to preview and author Animation C# Jobs constraints.</p></li>
<li><p>Asset Import: Added a new Cancel option for changing the Import Settings for Assets in addition to Apply and Revert. The Cancel option is the default when pressing  or closing the popup. Canceling restores the current selection and keeps the unapplied changes.</p></li>
<li><p>Asset Import: Compressor Quality can now be set in the texture asset import settings for BC6H and BC7 formats allowing compression quality to be traded for import speed.</p></li>
<li><p>Asset Import: Undo and Redo are now available on the Import Settings window while importing Assets.</p></li>
<li><p>Asset Import: Updated Sketchup SDK to version 19.0.</p></li>
<li><p>DX12: Improved performance of async texture loading in DX12 to avoid a rendering stall when 2D textures are created.</p></li>
<li><p>Editor: Added <strong>Enable Code Coverage</strong> option in General Preferences. Added a popup and a Console warning that notifies users that enabling Coverage slows performance. The window title now displays <code>[CODE COVERAGE]</code> when Coverage is enabled.</p></li>
<li><p>Editor: Added a message box whenever the OS fails to delete an asset when deleted from the Project Browser view.</p></li>
<li><p>Editor: Added a proxy icon for the currently open Scene to the title bar in the main Editor window on macOS.</p></li>
<li><p>Editor: Added a toggle to the Scene Camera settings for infinite acceleration when navigating with flying mode.</p></li>
<li><p>Editor: Added Araxis Merge support on Revision Control Diff/Merge tool.</p></li>
<li><p>Editor: Added new options for expanding/collapsing the components in the inspector context menu.</p></li>
<li><p>Editor: Added shortcut for Scene Visibility <strong>Show All</strong>.</p></li>
<li><p>Editor: Exposed ProjectWindowUtil.CreateScriptAssetFromTemplateFile. This function allows Editor scripts to create new text-based assets from template files in a similar way to how the built-in C# Script template is used to create new MonoBehaviour classes.</p></li>
<li><p>Editor: Made ProBuilder a recommended package.</p></li>
<li><p>Editor: Made the RenderDoc capture button in the Scene/Game view work with the Xcode frame debugger in Metal. This requires launching Unity through Xcode with the Metal frame capture enabled.</p></li>
<li><p>Editor: Moved Camera Easing options from Preferences to Camera Settings in the Scene view.</p></li>
<li><p>Editor: Moved Camera Easing options from Preferences to Camera Settings in the Scene view.</p></li>
<li><p>Editor: Optimized Inspector refresh after entering Play mode.</p></li>
<li><p>Editor: Reduced the number of key presses in order to start a rebind in the Shortcut manager.</p></li>
<li><p>GI: Added a 'None' mode for emissive GI contribution in the standard shader GUI.</p></li>
<li><p>GI: Added mixed area lights to culling results, which enable mixed rectangular lights in HDRP.</p></li>
<li><p>GI: Added Rendering.GraphicsSettings.realtimeDirectRectangularAreaLights to enable HDRP to provide direct realtime area lighting.</p></li>
<li><p>GI: Improved baking speed for the Progressive lightmapper in cases with many Light Probe sets in the Scene.</p></li>
<li><p>GI: Improved GPU Lightmapper performance by generating many rays per texel/Light Probe for indirect lighting. Optimized direct lighting by using compaction.</p></li>
<li><p>GI: Improved the GPU Lightmapper performance by generating many rays per texel/Light Probe for direct lighting.</p></li>
<li><p>GI: Optimized time to first lit texel for the progressive lightmappers by multithreading heavy functions.</p></li>
<li><p>GI: Realtime GI now uses correct lightomg falloff for indirect Lights when you use configurable light falloff.</p></li>
<li><p>GI: Reduced GPU memory footprint for the GPU Lightmapper when baking lighting. This is done by compressing normal vectors and albedo.</p></li>
<li><p>GI: The GPU Lightmapper now supports the Optix AI denoiser.</p></li>
<li><p>GI: Upgraded Optix AI Denoiser to version 6. This new version has better performance and a lower memory footprint.</p></li>
<li><p>Graphics: Added profiler markers for the Made with Unity splash screen.</p></li>
<li><p>Graphics: Added sprite Mesh support for custom splash screen logos. You can now use tight mesh mode and Vector sprites.</p></li>
<li><p>Graphics: Added SRP hooks for detail rendering Shaders.</p></li>
<li><p>Graphics: Added support for Dynamic Resolution Scaling to the Lightweight Rendering Pipeline.</p></li>
<li><p>Graphics: Added the ability to disable the blur on the Made with Unity splash screen. background.</p></li>
<li><p>Graphics: Asynchronous Shader compilation: Minimized cyan dummy shader flashes by variant tracking and warmup.</p></li>
<li><p>Graphics: Deferred the creation of command buffers and render encoders until they are needed in Metal.</p></li>
<li><p>Graphics: Improved the performance of asyncronous Texture loading on the PS4 by fixing a rendering stall that occured when you created a 2D Texture.</p></li>
<li><p>Graphics: The SRP Batcher is now supported on Xbox DirectX11.</p></li>
<li><p>Graphics: You can now use the SRP batcher on OpenGL 4.2+ and OpenGL ES 3.1+.</p></li>
<li><p>iOS: Added new iOS device (released in 2018) identification support to the Profiler.</p></li>
<li><p>iOS: Added <code>LowPowerModeEnabled</code> and <code>WantsSoftwareDimming</code> properties to <code>iOS.Device</code> and a <code>Brightness</code> Property to <code>Screen</code> (currently only supported on iOS).</p></li>
<li><p>iOS: Can now select architecture for native plugins on iOS &amp; TvOS.</p></li>
<li><p>iOS: ReplayKit improvements:</p> 
<ul>
<li>For local recordings, we can now capture the local camera, microphone, and screen.</li>
<li>The size of the preview window overlay can now be adjusted.</li>
<li>Added <code>ReplayKit.isPreviewControllerActive</code>, <code>ReplayKit.PauseBroadcasting</code>, and <code>ReplayKit.ResumeBroadcasting</code>.</li>
</ul></li>
<li><p>Kernel: Improveed the performance of the internal Matrix4x4 Invert method that Rendering and Cameras primarily use.</p></li>
<li><p>macOS: Native plugins with the .dylib file extension are now supported.</p></li>
<li><p>Mobile: Improved performance of async texture loading on iOS to remove a rendering stall when 2D textures are created.</p></li>
<li><p>Package Manager: Added support to include built-in packages in the Project as dependencies of other packages.</p></li>
<li><p>Package Manager: Improved package visibility in the Project view and the Object Picker.</p></li>
<li><p>Package Manager: Improved Undo/Redo and Cancel button handling in the Package Manifest Importer window.</p></li>
<li><p>Package Manager: Installed modules now appear in the Dependencies list alongside package dependencies.</p></li>
<li><p>Particles: Made missing External Forces module properties available in scripting API.</p></li>
<li><p>Physics: Upgraded the cloth library to use NVIDIA's NvCloth Library instead of the deprecated PxCloth.</p></li>
<li><p>Plugins: Added Unity Companion license to the Plugin API header.</p></li>
<li><p>Profiler: Added names to Unity-created threads in VTune profiler.</p></li>
<li><p>Profiler: Added reduced profiler overhead when flushing data from Job threads.</p></li>
<li><p>Profiler: Added single threaded platform support to the Memory Profiler.</p></li>
<li><p>Profiler: Made players show up consistently in the profiler list,when there are a lot of players running on the same network.</p></li>
<li><p>Profiler: Provide dynamic code (Mono JIT) information to VTune Amplifier.</p></li>
<li><p>ps4: Improved PS4 Additional content to support multiple products.</p></li>
<li><p>Scripting: Enabled incremental Garbage Collection in the Editor.</p></li>
<li><p>Scripting: The managed debugger now outputs the network port it's listening on to the player log.</p></li>
<li><p>Shaders: Defined <code>UNITY_SEPARATE_TEXTURE_SAMPLER</code> in <code>HlslSupport.cginc</code> for platforms capable of separate texture and sampler objects.</p></li>
<li><p>Shaders: Moved 38 built-in keywords to local keywords. Shaders inspector now shows used global/local keywords by shader.</p></li>
<li><p>Terrain: Made changes such that the system no longer generates basemap Textures if you do not use the basemap shader.</p></li>
<li><p>Terrain: Made changes to allow local keywords, which are defined with <code>multi_compile_local</code> or <code>shader_feature_local</code>, for Terrain shaders.</p></li>
<li><p>Terrain: Removed the Terrain Material enum type, and changed built-in Terrain Materials into selectable Assets.</p></li>
<li><p>Timeline: Added mute to Track groups.</p></li>
<li><p>Timeline: Added new user interface to animate track and clip properties.</p></li>
<li><p>Timeline: Added the ability to override the loop setting on Animation clips. (1140766, 1144743)</p></li>
<li><p>Timeline: Implemented a new read-only mode for when a Timeline asset is not editable. This is caused by either the file readonly flag or source control.</p></li>
<li><p>UI: Added ability to modify the UI Dropdown's Alpha fade when showing and hiding.</p></li>
<li><p>UI: Added the ability to modify the number of pixels per unit used when calculating sliced and tiled sprites.</p></li>
<li><p>UI: Removed the <code>spritePacking</code> tag option from the TextureImporter when not using the legacy packing mode.</p></li>
<li><p>UI Elements: Prevented exceptions thrown by user code from corrupting the UI renderer.</p></li>
<li><p>Video: Improved the documentation for platform strings used  by VideoClipImporter methods.</p></li>
<li><p>Windows: Added a Player Setting for reverting to BltBlt swapchain model which was used before 2019.1. This enables several scenarios like transparent window to be used once again.</p></li>
<li><p>XR: Added GPU Profiler support for Oculus Quest and Oculus Go.</p></li>
<li><p>XR: Added Low Overhead Mode setting to Oculus (Android) to do less driver validation, which can potentially increase performance.</p></li>
<li><p>XR: Moved the Google VR Cardboard and Daydream support to a package and updated to version 1.180.</p></li>
<li><p>XR: Updated Oculus to use the 1.36 plugin.</p></li>
<li><p>XR: Updated Vuforia to version 8.0.10.</p></li>
</ul>

### API Changes
<ul>
<li><p>AI: Added the <code>GetEdgesAndNeighbors()</code> method in the <code>NavMeshQuery</code> class for retrieving the shape of a given node and all the navigation nodes which it connects to. The method can be called in jobs.</p></li>
<li><p>Android: Added support for JNI Weak References (<code>AndroidJNI</code> class).</p></li>
<li><p>Asset Import: Added an API in the Model Importer to prevent GameObjects from being sorted by name in imported GameObject hierarchies.</p></li>
<li><p>Editor: Added API for Scene Visibility.</p></li>
<li><p>Editor: Added more API endpoints for <code>TransformHandle</code> to allow granular control over which handles appear.</p></li>
<li><p>Editor: Added new API to better detect and control async shader compilation in the Editor.</p></li>
<li><p>Editor: Added <code>AssemblyBuilder.referencesOptions</code> to allow building assemblies using UnityEngine module .dlls instead of the default monolithic UnityEngine.dll.</p></li>
<li><p>Editor: Added <code>AssetDatabase.OpenAsset()</code> overloads that take both a line number and column number.</p></li>
<li><p>Editor: Added <code>Editor.DrawFoldoutInspector</code> to draw a nested Inspector with a foldout title bar.</p></li>
<li><p>Editor: Added <code>EditorWindow.CreateWindow</code>, which works like <code>EditorWindow.GetWindow</code>, but always creates a new window.</p></li>
<li><p>Editor: Added <code>GameObjectUtility.GetMonoBehavioursWithMissingScriptCount</code> and <code>GameObjectUtility.RemoveMonoBehavioursWithMissingScript</code>for removing MonoBehaviours with missing scripts from GameObjects.</p></li>
<li><p>Editor: Added <code>MaterialEditor.customShaderGUI</code> property that returns the active ShaderGUI object for the current material.</p></li>
<li><p>Editor: Changing the display name of enum values in the Inspector is now done using the <code>InspectorNameAttribute</code> instead of the <code>DescriptionAttribute</code>. (<a href="https://issuetracker.unity3d.com/issues/drawdefaultinspector-displays-enums-differently-from-editorguilayout-dot-enumpopup-when-using-cusom-inspector">1115381</a>)</p></li>
<li><p>Editor: Renamed <code>SceneView.SceneViewCameraSettings</code> to <code>SceneView.CameraSettings</code>.</p></li>
<li><p>Editor: Replaced <code>EditorTool.OnActivate</code> and <code>OnDeactivate</code> methods with <code>EditorTools</code> events. This addresses callback order problems.</p></li>
<li><p>Editor: <code>OnOpenAsset</code> attribute now supports method signature <code>(int instanceId, int line, int column)</code></p></li>
<li><p>GI: Added <code>Gizmos.exposure</code> texture which, when set, is readback to determine exposure correction for LightProbe gizmos.</p></li>
<li><p>GI: Made it so you can set Lightmap Parameters from scripts on non-prefab objects. (<a href="https://issuetracker.unity3d.com/issues/lightmap-settings-of-game-object-is-not-saved-if-game-object-is-not-prefab">966408</a>)</p></li>
<li><p>Graphics: Added the static function, Inverse3DAffine(), to Matrix4x4 to compute the inverse of an affine matrix.</p></li>
<li><p>Graphics: Changed the SRP signature of <code>BeginCameraRendering</code> and <code>BeginFrameRendering</code> to give access to the <code>ScriptableRenderContext</code>. Added callbacks for end camera and end frame rendering.</p></li>
<li><p>Kernel: The function, UnsafeUtility.MemCpyReplicate(), no longer logs a failed assertion or raises an exception when the size or Count parameters are zero. Instead, it passively exits (like the other UnsafeUtility methods).</p></li>
<li><p>Mobile: Added 'Screen.cutouts' which displays cutout bounding boxes</p></li>
<li><p>Mobile: Added <code>Application.absoluteURL</code> property and <code>Application.deepLinkActivated</code> event which handles application activation via deep link.</p></li>
<li><p>Package Manager: Added an Editor API for retrieving package information based on an Asset path or an assembly:</p> 
<ul>
<li><code>PackageManager.PackageInfo.FindForAssetPath(string assetPath)</code></li>
<li><code>PackageManager.PackageInfo.FindForAssembly(Assembly assembly)</code></li>
</ul></li>
<li><p>Scripting: Added the <code>TryGetComponent</code>API to GameObject and Component classes that do not allocate in the Editor when the component does not exist.</p></li>
<li><p>Scripting: Added <code>UnityEditor.TypeCache</code> API which extracts derived types, methods or classes marked with an attribute quickly.</p></li>
<li><p>Shaders: Added the <code>Shader.FindPassTagValue</code> method for querying pass tag values.</p></li>
<li><p>Shaders: Added the <code>Shader.passCount</code> property for retrieving the number of shader passes of the active SubShader.</p></li>
<li><p>Terrain: Added a non-alloc version overload to the new <code>TerrainData.GetInterpolatedHeights</code> API.</p></li>
<li><p>Terrain: Added new callback APIs to monitor changes to Terrain Textures.</p> 
<ul>
<li><code>TerrainAPI.TerrainCallbacks.heightmapChanged</code></li>
<li><code>TerrainAPI.TerrainCallbacks.textureChanged</code>
These callbacks return both the changed rect region, and whether the change is synchronized to the CPU or is GPU only.</li>
</ul></li>
<li><p>Terrain: Added new TerrainData APIs to modify Terrain Textures more easily.</p> 
<ul>
<li><code>TerrainData.CopyActiveRenderTextureToHeightmap</code></li>
<li><p><code>TerrainData.CopyActiveRenderTextureToTexture</code>
Use the two above functions to copy content of the active RT into Terrain Textures, and optionally delay CPU synchronization, for instance, when a mousemove event occurs in the middle of painting.</p></li>
<li><p><code>TerrainData.DirtyHeightmapRegion</code></p></li>
<li><p><code>TerrainData.DirtyTextureRegion</code>
Use these two functions instead of ones initially listed if the user directly changes the GPU resources through other means.</p></li>
<li><p><code>TerrainData.SyncHeightmap</code></p></li>
<li><code>TerrainData.SyncTexture</code>
Use these two functions to perform a full synchronization from GPU to CPU, for instance, when a mouseup event occurs.</li>
</ul></li>
<li><p>Terrain: Added the <code>TerrainData.GetInterpolatedHeights</code> method for querying interpolated Terrain height values over a grid of samples.</p></li>
<li><p>Terrain: Added <code>TerrainData.SetTerrainLayersRegisterUndo</code> for setting the <code>terrainLayers</code> property. This function also lets undo operations in the Editor correctly handle Textures created or destroyed during the process.</p></li>
<li><p>Terrain: Deprecate TerrainData.UpdateDirtyRegion. Use TerrainData.DirtyHeightmapRegion instead.</p></li>
<li><p>Terrain: Deprecated <code>Terrain.ApplyDelayedHeightmapModification</code>. Use <code>TerrainData.SyncHeightmap</code> instead.</p></li>
<li><p>Terrain: Exposed the <code>TerrainLayerInspector</code> class.</p></li>
<li><p>Timeline: Added FootIK property to Timeline Animation clips. (<a href="https://issuetracker.unity3d.com/issues/the-object-animation-is-clipping-when-adding-animation-in-the-timeline">1115652</a>)</p></li>
<li><p>Timeline: Added the ClipEditor, TrackEditor, and MarkerEditor classes to UnityEditor.Timeline so a user can derive and modify custom clips, tracks, or markers respectively.</p></li>
<li><p>Timeline: Added TimelineEditor.selectedClip and TimelineEditor.selectedClips to get and set the selected clip or clips TimelineClips in the Timeline window.</p></li>
<li><p>Timeline: Added TrackAsset.mutedInHierarchy that indicates that a track is muted when it is in a muted group.</p></li>
<li><p>Video: Added overloads to MediaEncoder.AddFrame to accept timestamps for producing Variable Frame Rate movies. The timestamps are expressed with the new MediaTime struct.</p></li>
<li><p>Video: Added the sRGBClip property to VideoClipImporter and the sRGB property to VideoClip. These properties describe whether the content is sRGB or linear.</p></li>
<li><p>Video: Added Time.captureDeltaTime: a more precise floating point reciprocal of Time.captureFramerate.</p></li>
<li><p>XR: Added the XRSetting property <code>XR.XRSettings.deviceEyeTextureDimension</code> which allows you to determine what the XR platform's swap chain eye texture layout is.</p></li>
<li><p>XR: Added <code>UNITY_INITIALIZE_OUTPUT_STEREO_EYE_INDEX</code> to the built-in shader macros to allow for transfering the unity_StereoEyeIndex from a vertex shader to a geometry shader.</p></li>
<li><p>XR: Added <code>XR.XRDevice.UpdateEyeTextureAntiAliasingSettings</code> to force the hmd swap chain to be reallocated when the MSAA sample count is changed.</p></li>
</ul>

### Fixes
<ul>
<li><p>2D: Changed position of Tile Instantiated GameObject to align with the Tile Anchor position of the Tilemap.</p></li>
<li><p>2D: Cleaned up and updated the Sorting Group status of Renderers whose GameObjects were activated and then deactivated. (<a href="https://issuetracker.unity3d.com/issues/invalid-sortinggroup-index-set-in-renderer-error-when-managing-sortinggroups-children-objects">1141682</a>, 1151999)</p></li>
<li><p>2D: Edge Sprite Material changed when using a fill texture that is already an edge sprite on spriteshape. (<a href="https://issuetracker.unity3d.com/issues/2d-spriteshape-edge-sprite-material-changed-when-using-a-fill-texture-that-is-already-an-edge-sprite-on-spriteshape">1157201</a>, 1163660)</p></li>
<li><p>2D: Fixed an issue where a Particle System's Sorting Fudge value while it is in a Sorting Group caused it to sort correctly. Similar Renderers are now sorted according to their Sorting Group order.</p></li>
<li><p>2D: Fixed an issue where a Sprite Atlas did not change when its associated "Object for Packing" Texture was modified by a custom AssetPostprocessor script. (<a href="https://issuetracker.unity3d.com/issues/spiteatlas-does-not-change-when-its-associated-object-for-packing-texture-is-modified-by-a-custom-assetpostprocessor-script">1135638</a>)</p></li>
<li><p>2D: Fixed clipping of Tilemap selection option for Tilemap Focus Dropdown (<a href="https://issuetracker.unity3d.com/issues/tilemap-focus-on-dropdown-text-gets-clipped-when-tilemap-option-is-selected">1158947</a>, 1163376)</p></li>
<li><p>2D: Fixed crash when rendering a Hexagonal Tilemap with Top Left/Right Sort Order in Individual mode (<a href="https://issuetracker.unity3d.com/issues/rendernodequeue-reset-crash-when-editing-hexagonal-tilemaps-with-top-left-slash-right-sort-order-and-individual-mode">1142429</a>, 1155196)</p></li>
<li><p>2D: Fixed crash when setting SpriteRenderer to tiling draw mode when textureless Sprite is assigned (<a href="https://issuetracker.unity3d.com/issues/unity-crash-when-svg-image-draw-mode-is-set-to-sliced-or-tiled">1156756</a>, 1161725)</p></li>
<li><p>2D: Fixed links to documentation for Tilemap components. (<a href="https://issuetracker.unity3d.com/issues/tilemap-components-are-missing-links-to-docs">972901</a>)</p></li>
<li><p>2D: Fixed recomposite Collider2Ds with CompositeCollider2D when offset and vertex distance changes while in outline generation mode.</p></li>
<li><p>2D: Open ended Spriteshape renders the fill texture instead of the range sprite (<a href="https://issuetracker.unity3d.com/issues/2d-spriteshape-open-ended-spriteshape-renders-the-fill-texture-instead-of-the-range-sprite">1162134</a>, 1163663)</p></li>
<li><p>2D: Updated SortingLayerField and SpriteRendererEditor to correctly handle PrefabOverrides. (<a href="https://issuetracker.unity3d.com/issues/material-and-sorting-layer-fields-of-sprite-renderer-component-do-not-show-prefab-overrides-in-inspector">1109376</a>, 1151997)</p></li>
<li><p>Analytics: Fixed an issue where passing Unity objects to <code>AnalyticsEvent</code> caused allocation leak warnings. (1086690)</p></li>
<li><p>Android: Android now handles an Application.targetFrameRate value of -1 as 30 fps again.</p></li>
<li><p>Android: Fix performance penalty when using Vulkan on Android Q preview 5 (1169046, 1169302)</p></li>
<li><p>Android: Fixed a crash when using Android JNI methods from custom thread. (<a href="https://issuetracker.unity3d.com/issues/androidjava-star-is-crashing-when-used-from-custom-threads">545977</a>)</p></li>
<li><p>Android: Fixed a crash when using Optimized Frame Pacing with Vulkan. (1164435)</p></li>
<li><p>Android: Fixed an issue that caused APK builds to fail because Unity failed to retrieve the version code from the APK. (<a href="https://issuetracker.unity3d.com/issues/android-build-and-run-doesnt-deploy-apk-on-device-when-split-apks-by-target-architecture-is-enabled">1133867</a>)</p></li>
<li><p>Android: Fixed an issue that caused the build to fail when setting a keystore name from script. (<a href="https://issuetracker.unity3d.com/issues/android-build-fails-when-setting-keystore-path-via-script-as-a-string-with-relative-path-value">1158036</a>, 1162258)</p></li>
<li><p>Android: Fixed an issue that caused the Editor to crash when opening Player Settings withough having Android SDK set up. (<a href="https://issuetracker.unity3d.com/issues/crash-macos-editor-crash-when-android-platform-is-selected-no-sdk-installed-and-player-settings-button-was-pressed">1143624</a>, 1144223)</p></li>
<li><p>Android: Fixed an issue where custom Android libraries would not be initialized after launching an app after previously exiting the app via Application.Quit. (<a href="https://issuetracker.unity3d.com/issues/vr-android-application-dot-quit-no-longer-causes-apps-to-fully-terminate-the-process-on-oculus-go">1116123</a>)</p></li>
<li><p>Android: Fixed an issue where only part of a static splash image was visible on load when using a transparent splash image. (<a href="https://issuetracker.unity3d.com/issues/android-only-part-of-static-splash-image-is-visible-on-load-when-splash-image-is-transparent">1136826</a>)</p></li>
<li><p>Android: Fixed error "gradleOut-debug-unsigned.apk does not exist" that would occur while trying to build a signed development build. (<a href="https://issuetracker.unity3d.com/issues/android-development-build-with-signed-keystore-fails-building-because-gradleout-debug-unsigned-dot-apk-does-not-exist">1137971</a>)</p></li>
<li><p>Android: Fixed incomplete reading of large texture files. (1111919)</p></li>
<li><p>Android: Fixed large Unicode character marshaling between C# and Java on Android 4 and 5. (<a href="https://issuetracker.unity3d.com/issues/android-strings-consisted-of-astral-characters-are-corrupted-on-5-or-lower-android-devices">1123693</a>)</p></li>
<li><p>Android: Restored our previous method of managing Android signing keys and keystores. (<a href="https://issuetracker.unity3d.com/issues/android-unable-to-load-or-use-keystore-with-password-due-to-incorrect-storepass-parameter-quoting">1144308</a>, 1153333)</p></li>
<li><p>Android: The Y position for the touch and mouse are now inverted in the native backend instead of managed code using the new input system.</p></li>
<li><p>Animation: Allow deleting curve keys whilst dragging, without throwing errors. (<a href="https://issuetracker.unity3d.com/issues/console-throws-indexoutofrangeexception-when-editing-curves-after-deleting-a-key-and-moving-a-mouse">1129837</a>)</p></li>
<li><p>Animation: Fix live link not showing the right edge (1032879)</p></li>
<li><p>Animation: Fixed a crash when unloading animations that are part of an AnimatorController. (1122054)</p></li>
<li><p>Animation: Fixed an issue where RectTransform properties would show missing curves that were not actually missing (<a href="https://issuetracker.unity3d.com/issues/animation-anchored-position-z-reads-as-missing-in-the-animation-window">1115014</a>)</p></li>
<li><p>Animation: Fixed an issue where the Animation Component would stay ActiveAndEnabled when the GameObject was disabled. (<a href="https://issuetracker.unity3d.com/issues/behaviour-dot-isactiveandenabled-returns-true-when-used-on-a-script-disabled-object-with-an-animation-component">1094567</a>)</p></li>
<li><p>Animation: Fixed an issue where the AnimationEvent "Function" field would accept spaces. (<a href="https://issuetracker.unity3d.com/issues/error-about-animation-event-not-having-a-receiver-when-the-events-function-field-is-ended-with-a-space">1111933</a>)</p></li>
<li><p>Animation: Fixed an issue where the Animator would keep references to temporary strings when using ADBv2. (1137999, 1154360)</p></li>
<li><p>Animation: Fixed an issue where the Avatar preview would not react to ObjectSelector changes. (<a href="https://issuetracker.unity3d.com/issues/animation-preview-model-does-not-appear-in-preview-tab-when-being-selected-through-avatar-tab">1113154</a>)</p></li>
<li><p>Animation: Fixed an issue where the preview of transitions with exitTime == 0 would generate some NaN errors (<a href="https://issuetracker.unity3d.com/issues/preview-window-of-a-transition-shows-nan-when-changing-transition-duration-after-selecting-a-state-in-the-animator-window">1092857</a>)</p></li>
<li><p>Animation: Fixed AnimationUtility.SetAnimationClipSettings not regenerating runtime data. (<a href="https://issuetracker.unity3d.com/issues/root-values-played-by-the-timeline-that-has-a-recorded-track-are-incorrect-when-using-setanimationclipsettings">1091972</a>)</p></li>
<li><p>Animation: Fixed crash when changing controller in Animator Override Controller used in a Playable Graph. (1104518)</p></li>
<li><p>Animation: Fixed FileNotFoundException when double-clicking to open an Animator Controller asset. (<a href="https://issuetracker.unity3d.com/issues/macos-filenotfound-exception-when-trying-to-open-an-animator-controller">1127826</a>)</p></li>
<li><p>Animation: Fixed issue with .NET 4.0 causing issues with System.Single conversion (1057751)</p></li>
<li><p>Animation: Fixed memory leak in AnimationWindow when inspecting animation with large number of keyframes (<a href="https://issuetracker.unity3d.com/issues/animation-window-is-leaking-memory-when-inspecting-animation-with-more-keyframes">1092423</a>)</p></li>
<li><p>Animation: Fixed TransformStreamHandle.GetPosition not returning global position when applyRootMotion is off and user is controlling the root transform. (<a href="https://issuetracker.unity3d.com/issues/transformstreamhandle-dot-getposition-doesnt-get-the-correct-world-space-position-when-the-apply-root-motion-is-disabled">1115701</a>)</p></li>
<li><p>Animation: Properly stop graph when switching to manual update mode (<a href="https://issuetracker.unity3d.com/issues/the-manual-mode-is-stuck-when-changing-directorupdatemode-to-manual-in-play-mode-via-script">1084441</a>)</p></li>
<li><p>Animation: Right clicking on an item in a ReoderableList will select it, but will not trigger dragging logic (<a href="https://issuetracker.unity3d.com/issues/animation-parameter-is-not-selected-properly-when-deleting-it-by-using-lmb">907650</a>)</p></li>
<li><p>Asset Import: An error message now appears in the Texture Import Settings window when assigning an invalid texture format for a given platform and texture type. (<a href="https://issuetracker.unity3d.com/issues/error-when-changing-format-to-bc5-with-textureimporter-and-a-pop-up-for-unapplied-import-settings-when-deselecting-texture">1115190</a>)</p></li>
<li><p>Asset Import: Fixed a crash in the FBX Importer when calculating tangents on a blendshape that has infinite values in vertex positions. (<a href="https://issuetracker.unity3d.com/issues/generatesharedverticesindexlist-crashes-when-importing-a-fbx-file">1152354</a>, 1161614)</p></li>
<li><p>Asset Import: Fixed a problem with the Audio Importer which failed to save changes to platform specific settings when performing a Reset or applying an Audio Preset. (<a href="https://issuetracker.unity3d.com/issues/presets-platform-settings-are-not-saved-for-audio-importer-preset">1150491</a>, 1156484)</p></li>
<li><p>Asset Import: Fixed a regression where the contextual menu items for adding and deleting events were not working on the Animation tab of the Import Settings window. (<a href="https://issuetracker.unity3d.com/issues/fbx-importer-contextual-menu-for-events-not-working-anymore">1136900</a>, 1144451)</p></li>
<li><p>Asset Import: Fixed an issue where imported Assets were reverting to their names at the time of export, if they didn't match the name associated with the GUID. (<a href="https://issuetracker.unity3d.com/issues/importing-unity-package-does-not-keep-track-of-renames">1130301</a>)</p></li>
<li><p>Asset Import: Fixed an issue where re-importing a Shader caused a property size to keep growing even when the Shader failed to compile. (<a href="https://issuetracker.unity3d.com/issues/surface-shader-inspector-ui-keeps-adding-albedo-texture-parameters-when-a-multidimensional-array-is-added-to-the-shader">1127367</a>)</p></li>
<li><p>Asset Import: Fixed an issue with the model importer inspector material remapping section where the remapped materials are not properly updated after an item was added. (<a href="https://issuetracker.unity3d.com/issues/remapped-materials-material-selector-only-works-once">1115556</a>, 1160131)</p></li>
<li><p>Asset Import: Fixed cases where Sketchup files, originating from Sketchup 2019, failed to import successfully.</p></li>
<li><p>Asset Import: Fixed issue where clicking Cancel on the Import Package dialog failed to invoke the importPackageCancelled callback. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-importpackagecancelled-callback-is-not-called-at-all">1037916</a>)</p></li>
<li><p>Asset Import: Fixed issue where Unity returned an error instead of creating an empty package if no Assets can be exported. (<a href="https://issuetracker.unity3d.com/issues/exporting-package-without-exportpackageoptions-dot-recurse-exports-an-empty-package">1105480</a>)</p></li>
<li><p>Asset Import: The Import Settings window now shows a specific error when the Editor is not a valid MonoScript type. (1127110)</p></li>
<li><p>Asset Management: Fixed issue where fbx files are not re-imported when a AssetPostprocessor implementing OnPostprocessAnimation has its version updated. (<a href="https://issuetracker.unity3d.com/issues/asset-postprocessor-doesnt-reimport-fbx-file-with-animations-on-version-change-if-only-onpostprocessanimation-is-used">1153110</a>, 1161616)</p></li>
<li><p>Asset Pipeline: Fix race condition crash when loading asset bundles from managed streams. (<a href="https://issuetracker.unity3d.com/issues/crash-on-assetbundleloadfromasyncoperation-getassetbundleblocking-when-loading-assetbundles-via-loadfromstreamasync">1135251</a>, 1157657)</p></li>
<li><p>Asset Pipeline: Fixed an issue where mutually recursive assets could cause a crash.</p></li>
<li><p>Asset Pipeline: Fixed an issue with Unity crashing when a Material that is highlighted in the Project window is overwritten from a script. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-a-material-that-is-highlighted-in-the-project-window-is-overwritten-from-a-script">1119351</a>)</p></li>
<li><p>Audio: Fixed an issue with AudioClip Get/SetData when the provided offset/length requires wrapping around the end of the clip. (<a href="https://issuetracker.unity3d.com/issues/audioclip-dot-getdata-returns-samples-that-are-missing-parts-of-the-original-clip-when-wrap-around-is-needed">844064</a>, 1162046)</p></li>
<li><p>Audio: Removed "raw speaker mode" option from Project Settings for audio, as it was never usable and made the matching enum value obsolete. (<a href="https://issuetracker.unity3d.com/issues/unified-player-settings-on-changing-the-audio-default-speaker-mode-to-raw-it-sets-as-mono">1062387</a>)</p></li>
<li><p>Build Pipeline: Fix Unity allows to build project via script with not compatible color space and graphics API. (<a href="https://issuetracker.unity3d.com/issues/unity-allows-to-build-project-via-script-with-not-compatible-color-space-and-graphics-api">1076664</a>)</p></li>
<li><p>Build Pipeline: Fixed an issue where BuildPipeline.BuildAssetBundles was not releasing memory frequently enough leading to a out of memory crash</p></li>
<li><p>Build Pipeline: Fixed an issue where sprite atlas Sprites were included in the bundle multiple times. (<a href="https://issuetracker.unity3d.com/issues/android-same-atlas-assets-are-being-included-in-asset-bundle-multiple-times-when-bundle-is-built">1121868</a>)</p></li>
<li><p>Build Pipeline: Fixed SBP out of memory crash. (<a href="https://issuetracker.unity3d.com/issues/building-asset-bundles-with-sbp-may-get-oom-crash">1158643</a>, 1160712)</p></li>
<li><p>Build Pipeline: Fixed sprite sheets in asset bundles built by scriptable build pipeline crash on access. (<a href="https://issuetracker.unity3d.com/issues/sprite-sheets-in-asset-bundles-built-by-scriptable-build-pipeline-crash-on-access">1146568</a>, 1167257)</p></li>
<li><p>Build Pipeline: Made Unity include the splash screen background textures even when the splash screen is disabled, so that the scripting API can draw the splash screen. (<a href="https://issuetracker.unity3d.com/issues/splash-screen-background-is-not-included-when-drawing-with-scripting-api-and-splashscreen-is-disabled-in-player-settings">1114547</a>)</p></li>
<li><p>Deployment Management: Fixed an issue with throwing BuildFailedException from a build callback not failing the build. (<a href="https://issuetracker.unity3d.com/issues/build-does-not-fail-when-using-buildfailedexception">1097286</a>, 1159243)</p></li>
<li><p>DX12: Fix for DX12 heap alignment (1160388, 1162983)</p></li>
<li><p>DX12: Fixed exclusive fullscreen always reverting to windowed fullscreen.</p></li>
<li><p>DX12: Make sure we draw the light probe visualization only if we are inside a frame. (<a href="https://issuetracker.unity3d.com/issues/dx12-selecting-a-light-probe-group-game-object-in-directx12-mode-crashes-the-editor-at-d3d12scratchbuffer-d3d12scratchbuffer">1158553</a>, 1166716)</p></li>
<li><p>Editor: Added an error message to <code>EditorGUI.EndChangeCheck</code> when the stack is empty.</p></li>
<li><p>Editor: Added Material checkout support in the Game Object Inspector. (962080)</p></li>
<li><p>Editor: Added support for a new toolbox format for Rider.</p></li>
<li><p>Editor: Added support for menu trees in EditorTool context menu.</p></li>
<li><p>Editor: Assume calls in UnityTest are now treated as an inconclusive result. (1075663)</p></li>
<li><p>Editor: Checkbox buttons now toggle correctly when users press the <strong>Space</strong> shortcut key. (<a href="https://issuetracker.unity3d.com/issues/imgui-checkboxes-dont-toggle-when-keyboard-shortcut-space-is-pressed">1136216</a>)</p></li>
<li><p>Editor: Creating a material while multiple inspector windows are open no longer triggers <code>IndexOutOfRange</code> errors. (<a href="https://issuetracker.unity3d.com/issues/clicking-on-audio-listener-component-in-inspector-toggles-some-empty-space">1122847</a>)</p></li>
<li><p>Editor: Deleting a Preset Asset in ADB2 no longer causes an error. (<a href="https://issuetracker.unity3d.com/issues/presets-deleting-a-single-preset-from-the-project-generates-an-error-in-the-console">1157112</a>, 1159888)</p></li>
<li><p>Editor: Fix an issue where Panels displayed in the Scene view blocked user input across the width of the viewport. (<a href="https://issuetracker.unity3d.com/issues/panels-displayed-in-scene-view-block-user-input-across-the-width-of-the-viewport">1147144</a>, 1161722)</p></li>
<li><p>Editor: Fix Batchmode build hanging in PackageManager::RunRequestSynchronously. (<a href="https://issuetracker.unity3d.com/issues/osx-batchmode-build-hangs-at-refresh-detecting-if-any-assets-need-to-be-imported-or-removed">1137073</a>, 1154317)</p></li>
<li><p>Editor: Fix the issue with NullReferenceException when previewing assets on Unity Package import (<a href="https://issuetracker.unity3d.com/issues/custom-package-preview-window-goes-gray-when-clicking-on-image-files">1148966</a>, 1159897)</p></li>
<li><p>Editor: Fixed  an issue where gamepad input was not detected when 3 Xbox controllers were connected. (<a href="https://issuetracker.unity3d.com/issues/input-xbox-controller-input-not-detected">1127453</a>)</p></li>
<li><p>Editor: Fixed a crash that occurred when entering or exiting Play mode with certain AssetImporters displayed in the Inspector. (1141570, 1144208)</p></li>
<li><p>Editor: Fixed a crash that sometimes occurred if a sprite that was being drawn was deleted or modified while the splash screen was playing. The splash screen is now cancelled when an asset is modified or deleted. (<a href="https://issuetracker.unity3d.com/issues/splash-image-changing-logo-shown-while-splash-screen-is-on-preview-crashes-the-editor">857060</a>)</p></li>
<li><p>Editor: Fixed a delay when dragging the end cap of an edge in GraphView.</p></li>
<li><p>Editor: Fixed a holdover of the alt modifier in the Editor when gaining focus for Linux editor from alt+tab (1104979)</p></li>
<li><p>Editor: Fixed a NullReferenceException that occurred when changing the order of a reorderable list.</p></li>
<li><p>Editor: Fixed an Editor crash that occurred when switching to DirectX 12. (<a href="https://issuetracker.unity3d.com/issues/directx-12-editor-crashes-on-switching-windows-graphics-apis-to-direct3d12">1127388</a>)</p></li>
<li><p>Editor: Fixed an error that occurred when closing a detached Material preview window belonging to a "second" instance of an Inspector window. (1119612)</p></li>
<li><p>Editor: Fixed an exception that occurred when expanding the Mesh Renderer's Shader section in the Tree Inspector. (<a href="https://issuetracker.unity3d.com/issues/inspector-exception-when-expanding-the-mesh-renderers-shader-section-in-the-tree-inspector">1145010</a>, 1145056)</p></li>
<li><p>Editor: Fixed an issue in Unity Test Runner where tests timed out early when using large Timescale values. (<a href="https://issuetracker.unity3d.com/issues/playmode-tests-timeout-when-time-dot-timescale-is-large">1098090</a>)</p></li>
<li><p>Editor: Fixed an issue where <strong>PropertyAttribute</strong> was not applied on arrays. (<a href="https://issuetracker.unity3d.com/issues/propertyattribute-has-no-effect-on-items-in-an-array">1140241</a>)</p></li>
<li><p>Editor: Fixed an issue where <strong>Shift + Del</strong> did not remove empty elements from arrays in the Inspector window. (<a href="https://issuetracker.unity3d.com/issues/shift-plus-delete-does-not-remove-an-empty-element-from-the-array-in-the-inspector-window">1105084</a>)</p></li>
<li><p>Editor: Fixed an issue where clicking an AudioListener Component in the Inspector window caused empty space to appear. (<a href="https://issuetracker.unity3d.com/issues/clicking-on-audio-listener-component-in-inspector-toggles-some-empty-space">1122847</a>)</p></li>
<li><p>Editor: Fixed an issue where compliation failures caused Play mode tint to affect parts of the Editor after exiting Play mode. (<a href="https://issuetracker.unity3d.com/issues/color-of-the-editor-changes-as-if-it-was-play-mode-when-trying-to-enter-play-mode-before-scripts-are-compiled">1130997</a>)</p></li>
<li><p>Editor: Fixed an issue where Console windows disappear when the Unity Editor does not have focus. (<a href="https://issuetracker.unity3d.com/issues/console-windows-disappear-when-unity-editor-is-not-in-focus">1109182</a>)</p></li>
<li><p>Editor: Fixed an issue where Editor layouts with undocked windows were saved/loaded incorrectly. (<a href="https://issuetracker.unity3d.com/issues/editor-windows-layout-is-being-saved-slash-loaded-incorrectly-when-saving-undocked-or-maximized-tabs">1122565</a>)</p></li>
<li><p>Editor: Fixed an issue where Editor windows responded to mouse events outside their window areas. (<a href="https://issuetracker.unity3d.com/issues/editor-windows-respond-to-mouse-events-outside-the-window">1143721</a>, 1144224)</p></li>
<li><p>Editor: Fixed an issue where invoking <code>ShowObjectPicker</code> right after closing another ObjectPicker freezes the Editor. (<a href="https://issuetracker.unity3d.com/issues/showobjectpicker-freezes-editor-when-its-invoked-right-after-another-objectpicker-is-closed">1113046</a>)</p></li>
<li><p>Editor: Fixed an issue where relaunching the Editor after changing graphics settings returned the user to the Hub rather than the Editor. (<a href="https://issuetracker.unity3d.com/issues/hub-editor-doesnt-restart-instead-hub-opens-up-on-selecting-restart-editor-from-popup-when-changing-graphics-apis">1134314</a>, 1161970)</p></li>
<li><p>Editor: Fixed an issue where the <strong>Reset</strong> option in the Inspector context menu cleared the <strong>Name</strong> property for MonoBehaviour assets. (<a href="https://issuetracker.unity3d.com/issues/using-the-reset-context-menu-option-on-a-scriptable-object-clears-its-name-property-in-the-inspector-window">1092051</a>)</p></li>
<li><p>Editor: Fixed an issue where the <strong>Transform</strong> fields in the AvatarMask Inspector don't show all of a skeleton's transforms. (<a href="https://issuetracker.unity3d.com/issues/avatarmask-inspector-transforms-field-doesnt-show-all-transforms-from-the-skeleton">1123656</a>, 1152129)</p></li>
<li><p>Editor: Fixed an issue where the Camera preview had a fixed size when the Scene view tools panel was displayed. (<a href="https://issuetracker.unity3d.com/issues/camera-preview-has-minimum-width-and-does-not-shrink-when-tools-popup-in-scene-view-is-present">1125006</a>)</p></li>
<li><p>Editor: Fixed an issue where the Edit button became stuck in its enabled state. (<a href="https://issuetracker.unity3d.com/issues/imgui-edit-button-in-components-stays-activated-even-on-disabling-it">1120360</a>)</p></li>
<li><p>Editor: Fixed an issue where the Editor window "cropped" render textures. (<a href="https://issuetracker.unity3d.com/issues/postprocessing-depth-of-field-is-not-applied-to-the-whole-screen-when-resolution-is-fixed-and-is-resized">1127773</a>)</p></li>
<li><p>Editor: Fixed an issue where the Splash Screen Unity logo did not fit inside the <strong>Logos</strong> list in the Player section of the Project Settings window. (<a href="https://issuetracker.unity3d.com/issues/editor-splashscreen-logo-is-too-big-in-playersettings-editor">976154</a>)</p></li>
<li><p>Editor: Fixed an issue where the <code>FilePathAttribute</code> constructor threw an exception if called from a <code>MonoBehaviour</code> constructor or another thread. (<a href="https://issuetracker.unity3d.com/issues/filepathattribute-class-calls-an-api-method-get-unitypreferencesfolder-from-its-constructor-resulting-in-an-exception-error">1077857</a>)</p></li>
<li><p>Editor: Fixed an issue where unassigning a shortcut in the Shortcuts Manager did not update the command entry in the main menu. (<a href="https://issuetracker.unity3d.com/issues/shortcut-label-is-still-being-displayed-when-adding-and-removing-a-shortcut-for-the-command">1109108</a>)</p></li>
<li><p>Editor: Fixed an issue where uniformly scaling a zero-sized PrimitiveBoundsHandle using the <strong>Shift</strong> modifier caused the center point to drift. Uniform scaling now applies to all axes if the bounding volume had zero size at the time the control handle was clicked. (<a href="https://issuetracker.unity3d.com/issues/physics-capsule-collider-center-drifts-away-while-dragging-by-holding-shift-key">1021975</a>, 1152362)</p></li>
<li><p>Editor: Fixed an issue with "Assembly has duplicate references" errors not listing the duplicate references correctly. (1132593, 1148355)</p></li>
<li><p>Editor: Fixed an issue with "Multiple precompiled assemblies with the same name" errors not listing the paths of the precompiled assemblies. (<a href="https://issuetracker.unity3d.com/issues/precompiledassemblyexception-does-not-show-file-paths-in-its-message-when-there-are-few-assemblies-with-the-same-name">1138754</a>, 1148356)</p></li>
<li><p>Editor: Fixed an issue with <strong>Use GUIDs</strong> being enabled in the Assembly Definition File inspector when GUID references are not used. (<a href="https://issuetracker.unity3d.com/issues/assembly-definition-useguids-property-gets-enabled-when-changes-are-applied">1140806</a>, 1148354)</p></li>
<li><p>Editor: Fixed an issue with C# solutions not getting regenerated when changing the <strong>Allow 'unsafe' code</strong> Project setting. (<a href="https://issuetracker.unity3d.com/issues/visual-studio-continues-to-warn-about-unsafe-code-when-unsafe-code-is-enabled-in-project-settings">1105512</a>, 1148358)</p></li>
<li><p>Editor: Fixed an issue with jittery scrolling through large serialized lists in the Inspector. (<a href="https://issuetracker.unity3d.com/issues/inspector-is-stuttering-when-scrolling-through-the-large-serializable-list-on-the-scriptable-object-in-the-inspector">1131250</a>)</p></li>
<li><p>Editor: Fixed an issue with orphan host views that occurred while loading an Editor window layout. (<a href="https://issuetracker.unity3d.com/issues/console-throws-failed-to-destroy-views-number-1-hostview-error-when-changing-layout">1079742</a>)</p></li>
<li><p>Editor: Fixed an issue with <code>CompilationPipeline.GetAssemblies(AssemblyType.Player)</code> not returning test assemblies. (1137205, 1148357)</p></li>
<li><p>Editor: Fixed assertion message 's2 != NULL' in log files.</p></li>
<li><p>Editor: Fixed display of blendshapes count when count is 1 in model preview. (<a href="https://issuetracker.unity3d.com/issues/a-model-with-1-blendshape-does-not-show-blendshapes-count-info-in-previewgui">1162436</a>, 1166909)</p></li>
<li><p>Editor: Fixed incorrect asset icon being shown for assemblies.</p></li>
<li><p>Editor: Fixed resize borders on floating windows to better expose window controls. This also fixes an issue where dragging from other parts of the window triggered resizing. (1116567)</p></li>
<li><p>Editor: Fixed security vulnerability UNITY-SEC-2144.</p></li>
<li><p>Editor: Fixed splitter view layout and resizing rounding issues. (<a href="https://issuetracker.unity3d.com/issues/editor-windows-layout-is-being-saved-slash-loaded-incorrectly-when-saving-undocked-tabs">1099360</a>)</p></li>
<li><p>Editor: Fixed the misalignment by reverting the fadegroup functionality. (<a href="https://issuetracker.unity3d.com/issues/video-aspect-ratio-drop-down-appears-misaligned-on-changing-the-original-dimensions-of-the-video">1111065</a>, 1158313)</p></li>
<li><p>Editor: Fixed the position of the drag area of the preview resizer depending on whether the target preview is in an img container. (<a href="https://issuetracker.unity3d.com/issues/resizing-the-preview-in-the-asset-explorer-window-causes-the-wrong-mouse-icon-to-be-used">1154694</a>, 1160640)</p></li>
<li><p>Editor: Fixed the Preview pane in the Object Selector.</p></li>
<li><p>Editor: Fixed VU meter display on custom audio filter behaviours with custom Editors. (<a href="https://issuetracker.unity3d.com/issues/onaudiofilterread-meter-disappears-when-using-a-custom-editor">1117744</a>, 1162045)</p></li>
<li><p>Editor: Made the "Add Component" popup window receive focus in Linux editor. (1098140)</p></li>
<li><p>Editor: Maximizing an Editor window after resizing it by dragging from the top bar now works correctly. (<a href="https://issuetracker.unity3d.com/issues/editor-windows-dont-change-the-restoredown-to-maximize-when-pulled-from-the-top-bar">1126516</a>)</p></li>
<li><p>Editor: One column layout drop fix (<a href="https://issuetracker.unity3d.com/issues/editor-files-are-not-being-added-to-assets-folder-if-dragged-and-dropped-in-empty-space-below-the-package-manager-folder">1150509</a>, 1158294)</p></li>
<li><p>Editor: Renamed MeshRenderer Priority in the Editor to match the documentation.</p></li>
<li><p>Editor: Renamed the "Logging" preference in "Stack Trace" to avoid confusion. (<a href="https://issuetracker.unity3d.com/issues/turning-off-logging-still-shows-log-messages-and-disables-double-clicking-them">1118914</a>)</p></li>
<li><p>Editor: Renamed the UI Transparency Priority to Renderer Priority in MeshRenderer component.</p></li>
<li><p>Editor: Unity native DefaultImporter is now excluded from Presets. (<a href="https://issuetracker.unity3d.com/issues/presets-defaultinpector-type-needs-to-be-blacklisted">1129083</a>)</p></li>
<li><p>Editor: Updated the Windows splash screen.</p></li>
<li><p>Editor: <code>CustomPropertyDrawer</code>s of array elements inside another array now now work correctly on each element. (<a href="https://issuetracker.unity3d.com/issues/custompropertydrawers-have-different-behavior-now-in-2019-dot-2">1156837</a>, 1158011)</p></li>
<li><p>GI: Fixed a crash that occured when you recompiled Shaders, both manually or when you switched render pipelines.</p></li>
<li><p>GI: Fixed a crash with baking global illumination when HideFlags was configured on objects. (1129038)</p></li>
<li><p>GI: Fixed an intermediate lookup issue in Enlighten when using SSDs with Realtime GI and Baked GI enabled (<a href="https://issuetracker.unity3d.com/issues/realtime-gi-editor-throws-failed-opening-gi-file-errors-when-switching-ambient-modes">1128583</a>, <a href="https://issuetracker.unity3d.com/issues/realtime-gi-editor-throws-failed-opening-gi-file-at-relative-path-errors-when-switching-lighting-backends">1134676</a>, <a href="https://issuetracker.unity3d.com/issues/ui-ssds-do-not-contribute-to-realtime-lightmaps-even-when-contribute-gi-flag-is-enabled">1134702</a>, 1143679, 1143686, 1143687)</p></li>
<li><p>GI: Fixed an issue where Light Probes had corrupted gizmos when there was 1 static object in the Scene. (<a href="https://issuetracker.unity3d.com/issues/light-probe-gizmos-are-corrupted-after-upgrading-the-project">1123892</a>)</p></li>
<li><p>GI: Fixed an issue where push off parameter in Lightmap Parameters asset was ignored when baking lightmaps. (<a href="https://issuetracker.unity3d.com/issues/pushoff-slider-in-lightmap-parameters-asset-has-no-effect">1117680</a>)</p></li>
<li><p>GI: Fixed an issue where selecting Probe groups would make the Editor crash on Metal (macOS). (<a href="https://issuetracker.unity3d.com/issues/osx-editor-crashes-after-selecting-light-probe-group-gameobject-in-the-hierarchy">1123971</a>)</p></li>
<li><p>GI: Fixed broken bake in Editor with additive loaded scenes. (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-in-an-infinite-loop-with-integrate-failed-on-write-lighting-job-error-when-baking-gi">1138556</a>, 1167604)</p></li>
<li><p>GI: Fixed case of missing lighting when baking with GPU lightmapper. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-scene-is-black-after-baking-lighting-with-the-gpu-lightmapper">1121705</a>)</p></li>
<li><p>GI: Fixed error related to cached G buffer data "Failed reading from a9/a9af123a12f31.ghd" when using the progressive lightmapper while having data from older versions in the GI cache.</p></li>
<li><p>GI: Fixed hashing issue when writing out AO textures for PLM.</p></li>
<li><p>GI: Fixed the GPU Lightmapper so it gives stable results when changing compositing parameters, sample counts, or the number of bounces. (1111135)</p></li>
<li><p>GI: Fixed the Lighting Explorer so that it saves the column settings when you restart the Editor. (<a href="https://issuetracker.unity3d.com/issues/light-explorer-does-not-remember-column-states-between-sessions">1131422</a>)</p></li>
<li><p>GI: GI - Fix player crashes on Application.Quit() in Debug builds when using real-time GI (1158498) (1158498, 1160124)</p></li>
<li><p>GI: GPU lightmapper: Ensure OpenCL kernel are recompiled on Nvidia even when only the include files changes.</p></li>
<li><p>GI: GPU lightmapper: Fix crash on application exit when GPU lightmapper openCL context is lost.</p></li>
<li><p>GI: GPU lightmapper: Fixed a crash caused by running out of GPU memory when allocating the BVH (acceleration structure for ray tracing). This could happen when baking a terrain with a high heightmap resolution.</p></li>
<li><p>GI: GPU lightmapper: Make render jobs resilient to not yet prepared materials. This fix a crash when GPU lightmapper fallback to CPU. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-editor-crashes-in-radeonraysmeshmanager-storeperinstancematerialandtransmissiondata-when-baking-the-archviz-project">1133816</a>, 1149276)</p></li>
<li><p>GI: Renamed "Auto Bake On/Off" to "Auto Generate Lighting On/Off" in the app bar.</p></li>
<li><p>GI: Use AI denoising for shadow mask and direct environment samples when baking with the GPU lightmapper. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-ai-denoisers-do-not-denoise-shadowmask">1138839</a>, 1144432)</p></li>
<li><p>Graphics: Delay in bursts no longer works. (<a href="https://issuetracker.unity3d.com/issues/spawner-delay-in-bursts-no-longer-works">1154292</a>, 1156374)</p></li>
<li><p>Graphics: Enabled GPU skinning for BlendShapes on Metal.</p></li>
<li><p>Graphics: Fix CommandBuffer.SetShadowSamplingMode code typo. (1143760, 1158287)</p></li>
<li><p>Graphics: Fix Reflection Probes baking when R11G11B10 HDR mode is used in Graphics Settings. (<a href="https://issuetracker.unity3d.com/issues/reflection-probe-gozmos-are-distorted-when-selected-in-the-scene-and-android-platform-is-selected">1115040</a>, 1169640)</p></li>
<li><p>Graphics: Fixed a crash caused by Unknown LightMode in a ShaderLab Shader. (<a href="https://issuetracker.unity3d.com/issues/shaderlab-shader-is-causing-unity-to-crash-when-closing-the-editor-or-upgrading-the-project-to-newer-version">1132088</a>)</p></li>
<li><p>Graphics: Fixed a crash on GPU skinning when blend shapes had zero vertices. (<a href="https://issuetracker.unity3d.com/issues/crash-slash-freeze-on-skinnedmeshrender-when-gpu-skinning-is-enabled">1121794</a>)</p></li>
<li><p>Graphics: Fixed a crash that happened when updating mesh data from script when using Vulkan and graphics jobs. (1090932)</p></li>
<li><p>Graphics: Fixed an infinite console error loop when the user tried to assign a 2D texture in the Cubemap field of a Custom Reflection Probe. (<a href="https://issuetracker.unity3d.com/issues/lighting-assigning-2d-texture-to-cubemap-property-of-reflection-probe-throws-error">1156727</a>, 1156969)</p></li>
<li><p>Graphics: Fixed an issue where shadow quality settings were hidden when using an SRP, which meant that culling sometimes didn't include shadow casters.</p></li>
<li><p>Graphics: Fixed an issue where the Game view did not fully update streaming mips while in Edit mode. (<a href="https://issuetracker.unity3d.com/issues/game-view-texture-mip-levels-are-loaded-based-on-the-scene-view-camera-when-the-showtexturestreamingsummary-script-has-been-run">1141222</a>, 1145166)</p></li>
<li><p>Graphics: Fixed an issue where visual flickering happened when Mesh data was edited from a script while graphics jobs were in use in Vulkan. (<a href="https://issuetracker.unity3d.com/issues/dx12-dynamic-mesh-corruption-with-native-graphics-jobs-flickering-and-disapearing-meshes">1075277</a>)</p></li>
<li><p>Graphics: Fixed an issue with non-readable mesh where indices were kept in memory when loading from built data (<a href="https://issuetracker.unity3d.com/issues/mesh-memory-usage-increase-from-2018-dot-2-to-2018-dot-3-and-forward">1126675</a>)</p></li>
<li><p>Graphics: Fixed an issue with skinned mesh where vertex compression was disabled for all components. (<a href="https://issuetracker.unity3d.com/issues/vertex-compression-is-completely-disabled-on-platforms-with-compressedgpuskinningdisabled">1118278</a>)</p></li>
<li><p>Graphics: Fixed bad alignment of render surface resource heaps (<a href="https://issuetracker.unity3d.com/issues/d3d12immediatecontext-bindtexture-crash-when-opening-a-scene-with-directx3d12">1155163</a>, 1156592)</p></li>
<li><p>Graphics: Fixed cases where overlapping cross-fade objects sometimes appeared as opaque. (<a href="https://issuetracker.unity3d.com/issues/lod-blinking-artifact-at-speedtree-cross-fade-animation-when-several-tree-billboards-overlap">916831</a>)</p></li>
<li><p>Graphics: Fixed dynamic resolution when using Vulkan. (<a href="https://issuetracker.unity3d.com/issues/android-player-crashes-on-changing-resolution-dynamically">1148341</a>, 1148390)</p></li>
<li><p>Graphics: Fixed issue where Vulkan implementation of Texture2D.SetPixels may pipeline stall. (<a href="https://issuetracker.unity3d.com/issues/vulkan-inefficient-memory-barriers-vkcmdcopybuffertoimage">1141239</a>, 1145494)</p></li>
<li><p>Graphics: Fixed missing caps in the Pixels32 APIs. (1129776)</p></li>
<li><p>Graphics: Fixed missing IsEACFormat and IsXRFormat APIs. (1129777)</p></li>
<li><p>Graphics: Fixed RenderTextureFormat BGRA support. (1141798, 1144325)</p></li>
<li><p>Graphics: Fixed the app bar so it shows "Compiling shader 'x'" instead of just the Shader name.</p></li>
<li><p>Graphics: Fixed: Instancing batcher would crash hard on Vulkan if attempting to draw without an active GPU program.</p></li>
<li><p>Graphics: Made changes to correctly display a preview image of the Billboard Renderer in the Project Window and LODGroup preview panel. (<a href="https://issuetracker.unity3d.com/issues/speedtree-lod-inspector-lod-renderer-preview-is-not-displayed-for-spm-model">769753</a>)</p></li>
<li><p>Graphics: Made create texture occur on a thread in cases where async loads to update an existing texture.</p></li>
<li><p>Graphics: Made normal maps acknowledge the [Normal] attribute in shader when Unity checks that they have "Normal Map" texture usage. (1132148)</p></li>
<li><p>Graphics: Made Textures unsupported by mip map streaming such as reflection probes and decals now load highest mip. (<a href="https://issuetracker.unity3d.com/issues/reflection-probes-have-low-resolution-textures-when-building-with-texture-streaming-enabled-and-and-default-compression-mode">1115306</a>, 1145164)</p></li>
<li><p>Graphics: Metal: Artifacts appear when using Dynamic Resolution with MSAA (<a href="https://issuetracker.unity3d.com/issues/os-x-artifacts-appear-when-using-dynamic-resolution-with-msaa">1111105</a>)</p></li>
<li><p>Graphics: Removed 4G limit on texture mip streaming budget. (<a href="https://issuetracker.unity3d.com/issues/qualitysettings-dot-streamingmipmapsmemorybudget-is-always-clamped-down-to-4096-mb-even-on-64-bit-systems">1147394</a>, 1150741)</p></li>
<li><p>Graphics: Terrain alphamaps now ignore QualitySettings master texture limit (<a href="https://issuetracker.unity3d.com/issues/painting-texture-on-the-terrain-does-not-work-slash-crash-the-editor-when-projects-texture-quality-setting-is-not-set-to-full-res">1148582</a>, 1154326)</p></li>
<li><p>Graphics: Unity crashes when a VFX is playing and the VFX project settings are reset. (<a href="https://issuetracker.unity3d.com/issues/project-settings-unity-crashes-when-a-vfx-is-playing-and-the-vfx-project-settings-are-reset">1154099</a>, 1154781)</p></li>
<li><p>Graphics: unity_LightIndices[1] are identical to every object and are set per frame (<a href="https://issuetracker.unity3d.com/issues/srp-unity-lightindices-1-are-identical-to-every-object-and-are-set-per-frame">1155879</a>, 1166706)</p></li>
<li><p>Graphics: VFX : Enable/Disable doesn't restart effect. (1133474, 1152230)</p></li>
<li><p>Graphics: Vulkan: Fixed a crash that occcured when setting rendertexture sampler properties before creating the actual texture. (1115165)</p></li>
<li><p>Graphics: Vulkan: Fixed an issue that caused an error message to repeatedly occur when attempting to draw with missing bindings.</p></li>
<li><p>Graphics: Vulkan: Fixed crash when rendering reflection probes on Android. (1108968)</p></li>
<li><p>Graphics: Vulkan: Fixed crash when using MSAA.</p></li>
<li><p>IL2CPP: Fixed a crash on background threads when a managed exception occured while the process was shutting down.</p></li>
<li><p>IL2CPP: Fixed a crash when many threadpool threads or sockets were in use. (1129409, 1168721)</p></li>
<li><p>IL2CPP: Fixed a performance issue with lumped builds.</p></li>
<li><p>IL2CPP: Made generated code marshal an array of primitive types as <code>SAFEARRAY</code> by default if it's used as a field. (<a href="https://issuetracker.unity3d.com/issues/the-generated-il2cpp-code-no-longer-marshals-a-struct-to-its-native-representation-before-passing-it-to-a-native-function">1131557</a>, 1146301)</p></li>
<li><p>IL2CPP: Throw a managed exception at runtime when a generic type is marshaled as a delegate parameter. (1122074)</p></li>
<li><p>Input: Fixed a crash that happened with non-ASCII key mapping when trying to map a key which does not produce characters for single key presses (e.g. Japanese).</p></li>
<li><p>Input: Made scrolling delta on Mac work with older mice</p></li>
<li><p>Internal: Fixed <code>BatchRendererGroup</code> group removal.</p></li>
<li><p>iOS: 'UIApplicationExitsOnSuspend' will no longer be included in the Xcode project's info.plist file because it was made obsolete by Apple. (<a href="https://issuetracker.unity3d.com/issues/ios-apps-with-uiapplicationexitsonsuspend-in-info-dot-plist-failing-to-pass-apple-store-validation">1160614</a>, 1165520)</p></li>
<li><p>iOS: Added missing iOS devices to the device list used by the editor for profiler, Unity Remote, etc. (<a href="https://issuetracker.unity3d.com/issues/ios-unity-remote-doesnt-work-with-new-ios-devices-shows-unknown-dot-in-the-project-settings-device-name-dropdown-menu">1111598</a>)</p></li>
<li><p>iOS: Added missing RG16 texture format for Metal.</p></li>
<li><p>iOS: Fixed an issue that caused keyboard type to sometimes not change when switching controls. (<a href="https://issuetracker.unity3d.com/issues/ios-when-int-input-fields-keyboard-is-opened-focusing-other-input-fields-doesnt-open-corresponding-keyboards">1154527</a>, 1165455)</p></li>
<li><p>iOS: Fixed an issue where the Xcode framework search paths setting was overridden when appending an Xcode project. (<a href="https://issuetracker.unity3d.com/issues/ios-framework-search-paths-are-overriden-using-append">703217</a>)</p></li>
<li><p>iOS: Fixed build failure when Xcode <code>DerivedData</code> path was set relative to the project. (1117371)</p></li>
<li><p>iOS: Fixed identification of iPad 6th (it used to be identified as iPadPro10Inch2Genor or iPadUnknown with iOS.Device.generation) (<a href="https://issuetracker.unity3d.com/issues/ios-ipad-6th-generation-is-identified-as-ipadpro10inch2genor-or-ipadunknown-with-ios-dot-device-dot-generation">1065983</a>)</p></li>
<li><p>iOS: Fixed problem where Audio was "jumpy" on some iOS devices, skipping a few frames every few seconds (<a href="https://issuetracker.unity3d.com/issues/ios-audio-is-jumpy-on-some-ios-devices-skipping-a-few-frames-every-few-seconds">1124966</a>)</p></li>
<li><p>iOS: Fixed Screen.autorotateTo causing missing call to UnityOrientationRequestWasCommitted, effectively resulting in running some code every frame from now on erroneously. (<a href="https://issuetracker.unity3d.com/issues/ios-setting-screen-dot-autorotatetolandscapex-causes-the-next-attempt-to-open-safari-to-immediately-return-to-unity-silently">1122902</a>)</p></li>
<li><p>iOS: Fixed UIApplicationExitsOnSuspend is deprecated in iOS 13 (<a href="https://issuetracker.unity3d.com/issues/ios-apps-with-uiapplicationexitsonsuspend-in-info-dot-plist-failing-to-pass-apple-store-validation">1160614</a>, 1165520)</p></li>
<li><p>iOS: <code>Screen.currentResolution.refreshRate</code> now correctly returns the actual refresh rate instead of returning 30 in all situations. (1117877)</p></li>
<li><p>Kernel: Fixed a crash when resizing an array through <code>SerialziedProperty</code>. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-selecting-a-texture-preset-with-different-settings">1123752</a>)</p></li>
<li><p>Linux: Fixed an issue that caused submenus to lose focus and close prematurely. (<a href="https://issuetracker.unity3d.com/issues/linux-sprite-editor-slice-window-disappears-when-trying-to-change-slicing-type">1142911</a>, 1144233)</p></li>
<li><p>Linux: Fixed an issue that caused the Editor to overwrite the PlayerPrefs file at launch. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-overwrites-playerprefs-file-when-launched">1072116</a>)</p></li>
<li><p>Linux: Fixed an issue where the Editor crashed when started from the Hub (<a href="https://issuetracker.unity3d.com/issues/linux-editor-hangs-on-launch-when-running-through-unity-hub">1140369</a>, 1154319)</p></li>
<li><p>Linux: Fixed non-printable characters being allowed in GUI text objects in the Linux Editor. (<a href="https://issuetracker.unity3d.com/issues/linux-empty-characters-are-created-in-text-fields-when-using-ctrl-shortcuts">1126208</a>)</p></li>
<li><p>Linux: Linux Editor no longer fails to delete assets on partitions or network drives that do not contain trash directories. (<a href="https://issuetracker.unity3d.com/issues/you-cannot-delete-assets-on-a-network-drive-in-linux">1062162</a>)</p></li>
<li><p>Linux: Nvidia drivers are now forced to turn off vsync on Linux. (1109048, 1146524)</p></li>
<li><p>Linux: Pausing the Linux editor while playing with cursor lock mode set to locked or confined will now free the cursor. (1132336)</p></li>
<li><p>Linux: Vuforia link is now hidden in the Linux Editor for Linux. (<a href="https://issuetracker.unity3d.com/issues/linux-player-settings-link-to-download-vufora-sdk-fails-due-to-permission-rights">1144110</a>, 1157123)</p></li>
<li><p>Lumin: Fixed error preventing running playmode tests on a Lumin device.</p></li>
<li><p>Lumin: Re-added package signing support for MagicLeap packages.</p></li>
<li><p>macOS: Fixed an issue that caused the built game icon to appear distorted. (<a href="https://issuetracker.unity3d.com/issues/osx-default-icon-for-mac-standalone-is-distorted">1152484</a>, 1158746)</p></li>
<li><p>macOS: Fixed excessive fencing causing all GPU workload to be serialized.</p></li>
<li><p>macOS: Fixed incorrect Input.keyCode value when keyboard layout changes on macOS.</p></li>
<li><p>macOS: Fixed queued key events getting incorrect modifiers flags causing the wrong shortcut to be executed.</p></li>
<li><p>Multiplayer: Fixed an error with the NetworkManagerHUD when clicking Lan Client on WebGL build (<a href="https://issuetracker.unity3d.com/issues/networkmanagerhud-uncaught-typeerror-cannot-read-property-id-of-null-thrown-when-clicking-lan-client-on-webgl-build">860733</a>)</p></li>
<li><p>Package Manager: A local package (using the <code>file:/</code> protocol) is no longer allowed to reference a sub folder inside "Assets", "Library" or "ProjectSettings".</p></li>
<li><p>Package Manager: Added error handling for when a user has an empty <code>package.json</code> file in their Project. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-packages-package-dot-json-contains-incorrect-data-and-package-manager-window-is-open">1157243</a>, 1163613)</p></li>
<li><p>Package Manager: Fix the issue where the up/down arrows cycle through the full list of packages during search (<a href="https://issuetracker.unity3d.com/issues/package-manager-after-a-search-the-up-slash-down-arrows-cycle-through-the-full-list-of-packages">1144663</a>, 1154427)</p></li>
<li><p>Package Manager: Fixed an error in the Package Manager UI when the OS uses a language other than English.</p></li>
<li><p>Package Manager: Fixed an issue where a Git dependency resolved to the locked hash even after removing the commitish part of a Git URL.</p></li>
<li><p>Package Manager: Fixed an issue where cloning a Git repository could wait indefinitely for user input if credentials for that repository were not configured.</p></li>
<li><p>Package Manager: Fixed an issue where the cancel icon (x) on the Search box in the Package Manager UI disappears when installing or removing a package. (<a href="https://issuetracker.unity3d.com/issues/package-manager-search-cross-icon-disappears-on-installing-or-removing-a-package">1152444</a>, 1156832)</p></li>
<li><p>Package Manager: Fixed an issue where the status icons got corrupted whenever a user exits search mode. (1142542, 1144549)</p></li>
<li><p>Package Manager: Fixed an issue with hidden elements erroneously appearing in the UI. (<a href="https://issuetracker.unity3d.com/issues/unnecessary-ui-icons-are-drawn-at-the-top-left-of-the-package-manager-window-when-certain-package-search-strings-are-entered">1139170</a>)</p></li>
<li><p>Package Manager: Fixed incorrect error messages in the Package Manager UI while disabling the Built-in package. (<a href="https://issuetracker.unity3d.com/issues/packman-ui-disabling-modules-error-message-is-inaccurate">1131602</a>, 1145317)</p></li>
<li><p>Particles: Added fade and soft particle properties to the Emissive color of the Standard Particle Shaders.</p></li>
<li><p>Particles: Fixed ETC transparency on particles (1144935, 1150180)</p></li>
<li><p>Particles: Fixed ParticleSystem prewarm not locating WindZones, ForceFields and Colliders during Awake. (<a href="https://issuetracker.unity3d.com/issues/wind-zone-effect-is-not-prewarped-on-a-particle-system-after-reopening-the-project">1122824</a>, 1164545)</p></li>
<li><p>Particles: Fixed stuttering when using scripted simulation to request long simulation times. (<a href="https://issuetracker.unity3d.com/issues/particle-system-simulate-issues">753940</a>, 1144335)</p></li>
<li><p>Particles: Opening a legacy Prefab with a ParticleSystem in Prefab Mode: ParticleSystemRenderer component is now correctly hidden in the Inspector.</p></li>
<li><p>Phyics2D: The implicitly created static ground-body is now not shown in the static body count in the profiler 2D physics area. (<a href="https://issuetracker.unity3d.com/issues/profiler-shows-1-static-body-under-physics-2d-when-profiling-an-empty-scene">1143465</a>, 1148737)</p></li>
<li><p>Physics: Fix issue with bounds in SkinnedMeshRenderer. (<a href="https://issuetracker.unity3d.com/issues/adding-cloth-component-to-skinnedmeshrenderer-changes-bounds">879696</a>, 1153181)</p></li>
<li><p>Player: Fixed the order of event timestamps on windows. (1132707)</p></li>
<li><p>Player: Fixes CoreStats to only send Ads id if Ads service is enabled. (1120830, 1154339)</p></li>
<li><p>Player: New Input System: Fix potential deadlock when adding new devices.</p></li>
<li><p>Player: New Input System: Make Input Debugger work in edit mode.</p></li>
<li><p>Player: PlayerConnection API now works correctly when reconnecting after disconnecting.</p></li>
<li><p>Prefabs: Fix loosing selection of Prefab root in Prefab Mode after draggging script to Inspector.</p></li>
<li><p>Prefabs: Made imports batch when multi-selecting Prefab instances and clicking Apply All.</p></li>
<li><p>Prefabs: PrefabMode: For broken prefabs use the root that the PrefabImporter has chosen when opening the prefab file in Prefab Mode, other dangling roots are deleted.</p></li>
<li><p>Prefabs: Reflection CubeMap for default reflection in Prefab Mode has been replaced with a lower resolution and without a sun (which caused multiple highlights)</p></li>
<li><p>Profiler: Fix [Profiler] "Requested frame does not exists" exception thrown on clearing data while looking at UI Module
(<a href="https://issuetracker.unity3d.com/issues/profiler-requested-frame-does-not-exists-exception-thrown-on-clearing-data">1160622</a>, 1164595)</p></li>
<li><p>Scene Management: Fix reverting object override not working on Prefab instance inside Prefab Asset and throwing errors. (<a href="https://issuetracker.unity3d.com/issues/cannot-revert-changes-to-prefab-variants-when-the-prefab-variant-is-edited-via-project-view">1146441</a>, 1153391)</p></li>
<li><p>Scene Management: Prevent removing or altering components on immutable Prefab Assets via component context menu. (1129842, 1153396)</p></li>
<li><p>SceneManager: MergeTwoScenes test has occasional instability (1150769, 1160351)</p></li>
<li><p>Scripting: Fixed a crash when large array initializer is used. (<a href="https://issuetracker.unity3d.com/issues/windows-editor-crashes-with-a-stackoverflowexception-if-a-script-references-a-large-array">1148592</a>, 1160548)</p></li>
<li><p>Scripting: Fixed an error where assertion failed on expression: '!m_CoroutineEnumeratorGCHandle.HasTarget()' is thrown when GC is collected (<a href="https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-m-coroutineenumeratorgchandle-dot-hastarget-is-thrown-when-running-tests-in-test-runner">1094391</a>)</p></li>
<li><p>Scripting: Fixed an issue when running the Editor with old scripting runtime if incremental GC is enabled in Project Settings. (<a href="https://issuetracker.unity3d.com/issues/incremental-gc-projects-fails-to-open-if-switching-from-net-4-dot-x-to-net-3-dot-5-with-incremental-gc-enabled">1119216</a>)</p></li>
<li><p>Scripting: Fixed an issue where constructors were called twice on ScriptableObjects with custom attributes when referencing the ScriptableObject instance. (<a href="https://issuetracker.unity3d.com/issues/constructors-called-multiple-times-on-scriptableobjects-with-custom-attributes">1113071</a>)</p></li>
<li><p>Scripting: Fixed an issue where user scripts could unload global game managers (<a href="https://issuetracker.unity3d.com/issues/when-loading-up-the-project-fatal-error-unityeditor-dot-assetdatabase-loadassetatpath-is-being-thrown-out-and-unity-hangs">1114406</a>)</p></li>
<li><p>Scripting: Fixed TargetInvocationException when using ML.NET. (<a href="https://issuetracker.unity3d.com/issues/system-dot-reflection-dot-targetinvocationexception-is-thrown-when-using-net-machine-learning">1109657</a>)</p></li>
<li><p>Scripting: Made useGUID enabled by default when the reference field is empty in the  Assembly Definition Reference editor</p></li>
<li><p>Shaders: Fixed non-deterministic Shader binaries in Asset bundles. (<a href="https://issuetracker.unity3d.com/issues/static-batching-makes-the-assetbundles-built-with-the-same-scene-different-from-each-other">749340</a>)</p></li>
<li><p>Shaders: Fixed shader upgrader to not add exclude_renderers due to const array usage. (1053734, 1143646)</p></li>
<li><p>Shaders: Minor HLSLcc fixes. (1105361, <a href="https://issuetracker.unity3d.com/issues/two-shadercompilertests-hitting-asserts-on-reflection-callbacks">1142484</a>, 1143647, 1143648)</p></li>
<li><p>Shadows/Light: Fix shadows culling when camera and frustum are almost perpendicular (<a href="https://issuetracker.unity3d.com/issues/shadows-shadows-flicker-when-camera-is-moving">1150849</a>, 1163791)</p></li>
<li><p>SpeedTree: Fixed the import of collision objects from SpeedTree v8 Assets.</p></li>
<li><p>Terrain: Fix TerrainLayer selection in Paint Texture Tool when the terrain layer assets are deleted. (<a href="https://issuetracker.unity3d.com/issues/unable-to-remove-deleted-terrain-layers">1113312</a>, 1164861)</p></li>
<li><p>Terrain: Fix the case that alpha map textures were lost during saving of newly created TerrainData. (1158454, 1164113)</p></li>
<li><p>Terrain: Made Terrain Tree brush paint across Terrain tiles (<a href="https://issuetracker.unity3d.com/issues/terrain-trees-are-not-painted-on-neighbouring-terrain-when-painting-on-the-edge-of-terrain">1126622</a>)</p></li>
<li><p>Terrain: Support for passing down per-layer attributes regarding mask maps and alpha channels (<a href="https://issuetracker.unity3d.com/issues/terrain-lwrp-lod-popping-of-terrain-quad-nodes-with-instancing-enabled">1110520</a>, 1159521)</p></li>
<li><p>Timeline: Clips will no longer randomly disappear when showing or hiding inline curves. (1141661, 1150620)</p></li>
<li><p>Timeline: Fixed an issue where dragging and dropping objects between tracks did not insert a new track correctly. (<a href="https://issuetracker.unity3d.com/issues/timeline-misleading-track-insertion-when-dragging-objects-between-tracks-inside-a-track-group">1011381</a>)</p></li>
<li><p>Timeline: Fixed an issue where the Track group background would disappear while scrolling. (876340)</p></li>
<li><p>Timeline: Fixed an issue with dragging and dropping objects on a Track group. (1014774)</p></li>
<li><p>Timeline: Fixed Disable the possibility to add Markers to tracks of a Timeline that is ReadOnly (1134463, 1146268)</p></li>
<li><p>Timeline: Fixed record button state not updating when offset modes are changed. (<a href="https://issuetracker.unity3d.com/issues/timelines-animation-track-does-not-refresh-after-changing-track-offsets">1142747</a>, 1150598)</p></li>
<li><p>Timeline: Going to Play Mode while inspecting a Track Asset will no longer throw exceptions. (1141958, 1150599)</p></li>
<li><p>Timeline: Reactions for Signals were not correctly drawn (1134422)</p></li>
<li><p>Timeline: The global/local time referential button will no longer be shown for a top-level timeline. (1080872, 1150607)</p></li>
<li><p>UI: Added support for copying uv2 and uv3 from the UIVertex AddVert overloaded API.</p></li>
<li><p>UI: An animation that updates items no longer dirties the Layout. This fixes some animation-related performance issues.</p></li>
<li><p>UI: Fixed an issue caused by deleting a drop-down list while it is open. (<a href="https://issuetracker.unity3d.com/issues/deleting-a-dropdown-list-while-it-is-open-breaks-other-ui-objects">1106263</a>)</p></li>
<li><p>UI: Fixed an issue where a null TransformHierarchy caused a crash when updating a RectTransform. (<a href="https://issuetracker.unity3d.com/issues/crash-on-transform-gettransformaccess-when-building-list-of-referenced-assemblies-to-the-android">1102234</a>, 1158048)</p></li>
<li><p>UI: Fixed an issue where assigning a togglegroup or changing <strong>isOn</strong> would not set the toggle as dirty. (<a href="https://issuetracker.unity3d.com/issues/changing-the-group-field-on-a-toggle-component-doesnt-mark-the-scene-as-dirty">1141606</a>, 1154185)</p></li>
<li><p>UI: Fixed an issue where enabling a Canvas and polling its RectTransform data in <code>Awake</code>/<code>Start</code> returned incorrect values for root RectTransforms.</p></li>
<li><p>UI: Fixed an issue where the Editor became unresponsive when the <em>GICache</em> tab was open in the Project Preferences. (<a href="https://issuetracker.unity3d.com/issues/editor-is-extremely-slow-and-almost-unresposive-when-the-gicache-tab-is-opened">1149001</a>, 1152685)</p></li>
<li><p>UI: Fixed an issue where vertices generated for rich text tags led to very large vertex buffers.</p></li>
<li><p>UI: Fixed an issue with Canvas sort order being incorrect when Instantiating a GameObject with a Canvas</p></li>
<li><p>UI: Fixed compilation errors in <code>.asmdef</code> files that require a reference to the uGUI package. (<a href="https://issuetracker.unity3d.com/issues/unityengine-dot-ui-reference-is-missing-in-assembly-definition-assemblies-and-plugins">1154163</a>, 1154711)</p></li>
<li><p>UI: Fixed memory leak when rendering to a Camera with a disabled display. (<a href="https://issuetracker.unity3d.com/issues/memory-leak-if-only-one-display-device-is-connected-when-game-is-using-multiple-displays-and-networking">944603</a>)</p></li>
<li><p>UI: Fixed wording in <strong>Advanced</strong> Texture importing options for tiled sprites. (<a href="https://issuetracker.unity3d.com/issues/tiled-sprites-imported-to-newer-versions-from-versions-5-dot-4-and-lower-throw-an-advanced-texture-error-that-cant-be-fixed">1040453</a>)</p></li>
<li><p>UI: Fixing issue with IndexedSet not returning -1 when element is not found in dictionary.</p></li>
<li><p>UI: Made Assembly type check use TypeCache for better performance in Editor (<a href="https://issuetracker.unity3d.com/issues/using-net-api-4-dot-x-increases-performance-spike-in-scripts-twice-when-selecting-an-object-with-a-script-for-the-first-time">1099027</a>, 1163856)</p></li>
<li><p>UI: Made Unity recreate the GFX buffer if the stride size changes. (<a href="https://issuetracker.unity3d.com/issues/canvas-removing-normal-from-the-additional-shader-channel-drop-down-causes-rendering-issues">1143087</a>, 1144234)</p></li>
<li><p>UI: Updated <code>SetChildAlongAxis</code> to have a matching <code>SetChildAlongAxisWithScale</code> that takes a <strong>Scale</strong>.</p></li>
<li><p>UI Elements: A default asset is now created when a USS file import fails. (1125716)</p></li>
<li><p>UI Elements: Changing the an element's <strong>overflow</strong> after adding it to the visual tree now impacts clipping. (<a href="https://issuetracker.unity3d.com/issues/overflow-doesnt-work-when-used-with-ui-elements">1141603</a>, 1158365)</p></li>
<li><p>UI Elements: Fix the drop area of groups in graph view. (1152487, 1155396)</p></li>
<li><p>UI Elements: Fixed an invalid texture for toolbar elements in Light skin. (<a href="https://issuetracker.unity3d.com/issues/missing-texture-for-a-pressed-down-ui-dropdown-when-using-the-personal-editor-skin">1117232</a>)</p></li>
<li><p>UI Elements: Fixed an issue that caused the Editor to freeze when adding new elements while clearing children. (1102592)</p></li>
<li><p>UI Elements: Fixed an issue where resizing a clipper could leave child clippers with an invalid clipping state. (1119623)</p></li>
<li><p>UI Elements: Fixed an issue where some culled Inspectors and fields were displayed in the Inspector window. (<a href="https://issuetracker.unity3d.com/issues/additional-metadata-fields-are-revealed-in-inspector-window-after-switching-from-normal-to-debug-mode-and-vice-versa">1123033</a>, <a href="https://issuetracker.unity3d.com/issues/particlesystemrenderer-component-appears-after-particlesystem-component-was-reverted-from-prefab-instance">1151394</a>, <a href="https://issuetracker.unity3d.com/issues/particlesystemrenderer-component-appears-after-added-script-is-deleted">1152519</a>, 1153150, 1170579, 1170580)</p></li>
<li><p>UI Elements: Fixed an issue where the Material Editor constantly repainted the Inspector window. (1111923)</p></li>
<li><p>UI Elements: Fixed bound array fields in UIE not properly syncing their array sizes when the same object was being edited elsewhere. (<a href="https://issuetracker.unity3d.com/issues/ui-elements-array-element-out-of-bounds-exception-thrown-on-undoing-or-redoing-a-change-in-float-array-field">1141787</a>, 1153154)</p></li>
<li><p>UI Elements: Fixed broken edge expansion system and tesselation.</p></li>
<li><p>UI Elements: Fixed Play mode tint in the Editor for UIElements. (1129564)</p></li>
<li><p>UI Elements: Fixed the foldout triangle size. (1122034)</p></li>
<li><p>UI Elements: Fixed Unable to set the Foldout.text "text" or "value" attributes through UXML. (<a href="https://issuetracker.unity3d.com/issues/unable-to-set-the-foldout-dot-text-text-or-value-attributes-through-uxml-schema">1119589</a>, 1150532)</p></li>
<li><p>UI Elements: Improved consistency of <code>MouseEnter</code> and <code>MouseLeave</code> events. (1081998, 1150185)</p></li>
<li><p>UI Elements: Invalid <strong>Scale</strong> values on the Z component are now ignored and do not prevent the VisualElement from disappearing. (1134758, 1147315)</p></li>
<li><p>UI Elements: Picking is now faster in UIElements. (1124338)</p></li>
<li><p>UI Elements: Prevented the activation of Content Dragger from the Blackboard in GraphView. (1146288)</p></li>
<li><p>UI Elements: Prevented zooming in and out with the scroll wheel while the mouse pointer is over the Blackboard in GraphView. (1139333, 1146282)</p></li>
<li><p>UI Elements: Removed support for instantiating elements with <code>DoCreate()</code> in UXMLFactories</p></li>
<li><p>UI Elements: Resizing a VisualElement no longer causes unnecessary nudges or repainting of children. (1109689, 1144434)</p></li>
<li><p>UI Elements: UI element that has focus now loses focus when the window loses focus,  and gets focus back when window is gets focus back. (<a href="https://issuetracker.unity3d.com/issues/uielements-textfield-still-draw-selection-when-window-is-not-focused">984433</a>)</p></li>
<li><p>Universal Windows Platform: Fixed awaiting async actions and operations on the UI thread continuing on a background thread (the continuations will now run on UI thread). (<a href="https://issuetracker.unity3d.com/issues/uwp-messagedialog-class-causes-crash-on-il2cpp-backend">1130193</a>, 1150948)</p></li>
<li><p>Universal Windows Platform: Fixed IL2CPP crashing when using certain new types (like <code>Windows.Foundation.GuidHelper.Equals</code>) in Windows SDK 17763 or newer.</p></li>
<li><p>Version Control: Editor Fix logging when files/folders in the Unity project are excluded from the Perforce client workspace (<a href="https://issuetracker.unity3d.com/issues/vcs-console-constantly-prints-warning-if-file-is-excluded-from-workspace">1143683</a>, 1145762)</p></li>
<li><p>Video: Camera Near Plane mode in a 2D project is not rendering the video clip only audio is heard (1135033, 1146656)</p></li>
<li><p>Video: Fix camera culling mask for VideoPlayer. (<a href="https://issuetracker.unity3d.com/issues/videoplayer-renders-only-when-default-layer-is-enabled-on-cameras-culling-mask">1146620</a>, 1152117)</p></li>
<li><p>WebGL: Fixed a bug when indexedDB timeout would prevent the build from loading. (1134367)</p></li>
<li><p>WebGL: Fixed an issue with saving PlayerPrefs in WebGL. (<a href="https://issuetracker.unity3d.com/issues/playerprefs-dont-get-saved-in-a-webgl-build">1140820</a>, 1145636)</p></li>
<li><p>WebGL: Fixed rendering errors in WebGL when canvas is not displayed. (<a href="https://issuetracker.unity3d.com/issues/webgl-screen-position-out-of-view-frustum-error-is-thrown-when-using-display-none-style-for-gamecontainer-in-build">1141232</a>, 1154630)</p></li>
<li><p>Windows: Fixed an issue that caused an iOS build to fail when a language with non-Latin characters is set as the Windows display language. (<a href="https://issuetracker.unity3d.com/issues/windows-build-fails-on-ios-and-android-when-language-with-non-latin-characters-is-set-as-windows-display-language">1136098</a>, 1160390)</p></li>
<li><p>Windows: Fixed an issue that caused key 9 sending key 8 events in the input system on Windows. (<a href="https://issuetracker.unity3d.com/issues/windows-editor-alpha-9-key-pressed-always-return-alpha-8-key">1132663</a>)</p></li>
<li><p>Windows: Fixed standalone Windows player hanging on startup on machines with strict group policies (<a href="https://issuetracker.unity3d.com/issues/standalone-build-freezes-at-startup-on-intel-gpus">1083303</a>)</p></li>
<li><p>Windows: Improved Windows crash handling reliability.</p></li>
<li><p>XR: Added Incremental GC on Lumin.</p></li>
<li><p>XR: Deprecated <code>UnityEngine.XR.InputTracking</code>s <code>GetLocalPosition</code> and <code>GetLocalRotation</code>.</p></li>
<li><p>XR: Device is Y-flipped when running scene on iOS Cardboard with Metal (1066864, 1153465)</p></li>
<li><p>XR: Final render image on Vulkan is no longer flipped vertically when single-pass stereo instancing is enabled. (1135134)</p></li>
<li><p>XR: Fixed Magic Leap package download in Lightweight Render Pipeline template. (1106219, 1146997)</p></li>
<li><p>XR: Renamed the two types of raycasts in the XRRaycastSubsystem profiler to <code>XR.RaycastFromScreen</code> and <code>XR.RaycastRay</code> for easier identification.</p></li>
<li><p>XR: The standalone player with Vulkan API and single-pass instanced mode no longer shows a black screen in HMD. (1142602)</p></li>
<li><p>XR: Unity shaders on Vulkan are now set up for stereo instancing. (1129654)</p></li>
<li><p>XR: Vulkan draw calls now draw to the second slice of texture array during stereo instancing. (1129656)</p></li>
<li><p>XR: Vulkan instance extensions are now correctly applied on Oculus. (1123193)</p></li>
</ul>

### Known Issues in 2019.2.0f1
<ul>
<li><p>Animation:  Absence of root motion when gameobject is loaded from assest bundle and override controller is in use (<a href="https://issuetracker.unity3d.com/issues/animation-absence-of-root-motion-when-gameobject-is-loaded-from-assest-bundle-and-override-controller-is-in-use">1165817</a>)</p></li>
<li><p>Animation:  Error is thrown when calling Animator.keepAnimatorControllerStateOnDisable on an inactive GameObject (<a href="https://issuetracker.unity3d.com/issues/animation-error-is-thrown-when-calling-animator-dot-keepanimatorcontrollerstateondisable-on-an-inactive-gameobject">1168475</a>)</p></li>
<li><p>Graphics - General: SRP causes crashes 100% when running with Graphics Jobs enabled (<a href="https://issuetracker.unity3d.com/issues/srp-causes-crashes-100-percent-when-running-with-graphics-jobs-enabled">1159200</a>)</p></li>
<li><p>IL2CPP:  NotImplementedException is thrown when use System.IO.Pipes (<a href="https://issuetracker.unity3d.com/issues/il2cpp-notimplementedexception-is-thrown-when-use-system-dot-io-dot-pipes">1159863</a>)</p></li>
<li><p>Inspector Framework: "ArgumentException: Object at index 0 is null" thrown when entering play mode with two Inspector windows and an attached script (<a href="https://issuetracker.unity3d.com/issues/argumentexception-object-at-index-0-is-null-thrown-when-entering-play-mode-with-two-inspector-windows-and-an-attached-script">1147234</a>)</p></li>
<li><p>MacOS: Unity Editor crashes in dispatch_release when running Tests in Batch Mode (<a href="https://issuetracker.unity3d.com/issues/dispatch-semaphore-dispose-crashes-when-running-tests-in-batch-mode">1169988</a>)</p></li>
<li><p>Mobile: [Android] CommandInvokationFailure appears in console when inspecting the API levels in Player Settings if using Bundled SDK (<a href="https://issuetracker.unity3d.com/issues/cannot-build-android-player-if-the-colour-space-is-set-to-linear">1136069</a>)</p></li>
<li><p>Package Manager: The Package Manager UI does not refresh when you install or remove packages. (<a href="https://issuetracker.unity3d.com/issues/the-package-manager-ui-does-not-refresh-when-packages-are-installed-or-removed">1148329</a>, 1152868)</p></li>
<li><p>Physics: Crash in physics PhysicsManager::Simulate (<a href="https://issuetracker.unity3d.com/issues/crash-in-physics-physicsmanager-simulate">1122684</a>)</p></li>
<li><p>Physics: Crash on block_remove when changing mesh to Plane in Skinned Mesh Renderer while cloth component attached (<a href="https://issuetracker.unity3d.com/issues/crash-on-block-remove-when-changing-mesh-to-plane-in-skinned-mesh-renderer-while-cloth-component-attached">1162918</a>)</p></li>
<li><p>Profiling: GfxDevice::OnProfilerFrameChanged crash (<a href="https://issuetracker.unity3d.com/issues/gfxdevice-onprofilerframechanged-crash">1169456</a>)</p></li>
<li><p>Scripting: [Android][Mono][IL2CPP] "Unable to find libc" error thrown when executing certain SslStream constructor  (<a href="https://issuetracker.unity3d.com/issues/android-mono-il2cpp-unable-to-find-libc-error-thrown-when-executing-certain-sslstream-constructor">1022228</a>)</p></li>
<li><p>Scripting: [Templates] Clamp BlendShapes are set to true by default when creating new projects (<a href="https://issuetracker.unity3d.com/issues/templates-clamp-blendshapes-are-set-to-true-by-default-when-creating-new-projects">1148638</a>)</p></li>
<li><p>VR: [Oculus GO][Oculus Quest] Object is jittering when position is being affected by Time.deltaTime (<a href="https://issuetracker.unity3d.com/issues/oculus-go-oculus-quest-object-is-jittering-when-position-is-being-affected-by-time-dot-deltatime">1157271</a>)</p></li>
<li><p>Windows: Built projects do not launch on some Windows 7 systems (<a href="https://issuetracker.unity3d.com/issues/built-projects-do-not-launch-on-some-windows-7-systems">1150661</a>)</p></li>
<li><p>Windows: Editor stuck on import when importing "GameAnalytics Unity SDK" package (<a href="https://issuetracker.unity3d.com/issues/editor-stuck-on-import-when-importing-gameanalytics-unity-sdk-package">1167747</a>)</p></li>
<li><p>Windows: [Windows 7] GfxDeviceD3D11Base::DrawQuad crash when using Camera with Clear Flags set to "Don't Clear" and Linear rendering (<a href="https://issuetracker.unity3d.com/issues/windows-7-player-crashes-on-pal-memory-free-when-using-camera-with-clear-flags-set-to-dont-clear">1157730</a>)</p></li>
<li><p>XR: Cardboard projects default to 30 frames per second unless <code>targetFrameRate</code> is set to 60. (<a href="https://issuetracker.unity3d.com/issues/cardboard-projects-default-to-30fps">1143799</a>, 1144492)</p></li>
</ul>

### System Requirements

### For development

#### OS: Windows 7 SP1+, 8, 10, 64-bit versions only; macOS 10.12+. (Server versions of Windows & OS X are not tested.)

#### CPU: SSE2 instruction set support.

#### GPU: Graphics card with DX10 (shader model 4.0) capabilities.

#### The rest mostly depends on the complexity of your projects.

### Additional platform development requirements:
<ul>
<li><p>iOS: Mac computer running minimum macOS 10.12.6 and Xcode 9.4 or higher.</p></li>
<li><p>Android: Android SDK and Java Development Kit (JDK); IL2CPP scripting backend requires Android NDK.</p></li>
<li><p>Universal Windows Platform: Windows 10 (64-bit), Visual Studio 2015 with C++ Tools component or later and Windows 10 SDK</p></li>
</ul>

### For running Unity games

#### Generally content developed with Unity can run pretty much everywhere. How well it runs is dependent on the complexity of your project. More detailed requirements:
<ul>
<li><p>Desktop:</p> 
<ul>
<li>OS: Windows 7 SP1+, macOS 10.12+, Ubuntu 12.04+, SteamOS+</li>
<li>Graphics card with DX10 (shader model 4.0) capabilities.</li>
<li>CPU: SSE2 instruction set support.</li>
</ul></li>
<li><p>iOS player requires iOS 9.0 or higher.</p></li>
<li><p>Android: OS 4.1 or later; ARMv7 CPU with NEON support or Atom CPU; OpenGL ES 2.0 or later.</p></li>
<li><p>WebGL: Any recent desktop version of Firefox, Chrome, Edge or Safari.</p></li>
<li><p>Universal Windows Platform: Windows 10 and a graphics card with DX10 (shader model 4.0) capabilities</p></li>
</ul>
