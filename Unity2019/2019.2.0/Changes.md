# Unity 2019.2.0

https://unity3d.com/unity/whats-new/2019.2.0

## Changes

- [Improvements](#improvements)


*   Android: Gradle version updated up to 5.1.1.
    
*   Android: Updated Bundletool to version 0.7.2.
    
*   VFX: Changed the awakening process of the VisualEffect component, so you can now use the Inspector even if the component is disabled. ([1117103](https://issuetracker.unity3d.com/issues/vfx-graph-overrides-stored-in-prefabs-get-disabled-when-using-prefabs-in-scenes-making-new-overrides-even-when-reverting))
    

### Improvements

*   2D: Added a toggle switch to the Grid Brush for a mode to change Z Positions of Tiles.
    
*   2D: Added multitexture support to SpriteShapeRenderer.
    
*   2D: Added multitexture support to TilemapRenderer.
    
*   2D: Added the CreateTileFromPaletteAttribute to allow users to specify how and what Tiles are created when dragging Assets onto the Tile Palette window.
    
*   2D: Exposed GridPaintingState APIs to allow users to programatically change Tile Palette Painting states
    
*   2D: Users can now convert Prefabs to Tile Palettes by dragging a valid Prefab onto the Tile Palette window.
    
*   Android: Enabled Vulkan support for Optimized frame pacing on Android.
    
*   Android: Implemented Screen.Brightness property for Android (read-only).
    
*   Android: Improved performance of string marshaling between C# and Java (up to 50% faster).
    
*   Android: Moved AndroidJava\* and AndroidJNI APIs to built-in package AndroidJNI.
    
*   Android: Reduced armv7 code size by 20% by enabling thumb.
    
*   Android: Small reduction in job overhead when few cores are being used.
    
*   Android: The Unity video player can now be used with the Vulkan renderer.
    
*   Android: When set to true, you can mimic TouchScreenKeyboard.hideInput by drawing an input field outside the screen.
    
*   Animation: Added a contextual menu option that jumps to a specific AnimatorController State while liveLinked is enabled.
    
*   Animation: Added a selection filter that shows properties and animation curves for only the selected GameObjects.
    
*   Animation: Added an option to hide read-only clip properties and animation curves in the Animation window, to improve performance.
    
*   Animation: Added visibility feedback to the Animator Inspector.
    
*   Animation: Added visual feedback and keyboard shortcuts for the Ripple option in the Animation window.
    
*   Animation: Updated the Animation window to preview and author Animation C# Jobs constraints.
    
*   Asset Import: Added a new Cancel option for changing the Import Settings for Assets in addition to Apply and Revert. The Cancel option is the default when pressing or closing the popup. Canceling restores the current selection and keeps the unapplied changes.
    
*   Asset Import: Compressor Quality can now be set in the texture asset import settings for BC6H and BC7 formats allowing compression quality to be traded for import speed.
    
*   Asset Import: Undo and Redo are now available on the Import Settings window while importing Assets.
    
*   Asset Import: Updated Sketchup SDK to version 19.0.
    
*   DX12: Improved performance of async texture loading in DX12 to avoid a rendering stall when 2D textures are created.
    
*   Editor: Added **Enable Code Coverage** option in General Preferences. Added a popup and a Console warning that notifies users that enabling Coverage slows performance. The window title now displays `[CODE COVERAGE]` when Coverage is enabled.
    
*   Editor: Added a message box whenever the OS fails to delete an asset when deleted from the Project Browser view.
    
*   Editor: Added a proxy icon for the currently open Scene to the title bar in the main Editor window on macOS.
    
*   Editor: Added a toggle to the Scene Camera settings for infinite acceleration when navigating with flying mode.
    
*   Editor: Added Araxis Merge support on Revision Control Diff/Merge tool.
    
*   Editor: Added new options for expanding/collapsing the components in the inspector context menu.
    
*   Editor: Added shortcut for Scene Visibility **Show All**.
    
*   Editor: Exposed ProjectWindowUtil.CreateScriptAssetFromTemplateFile. This function allows Editor scripts to create new text-based assets from template files in a similar way to how the built-in C# Script template is used to create new MonoBehaviour classes.
    
*   Editor: Made ProBuilder a recommended package.
    
*   Editor: Made the RenderDoc capture button in the Scene/Game view work with the Xcode frame debugger in Metal. This requires launching Unity through Xcode with the Metal frame capture enabled.
    
*   Editor: Moved Camera Easing options from Preferences to Camera Settings in the Scene view.
    
*   Editor: Moved Camera Easing options from Preferences to Camera Settings in the Scene view.
    
*   Editor: Optimized Inspector refresh after entering Play mode.
    
*   Editor: Reduced the number of key presses in order to start a rebind in the Shortcut manager.
    
*   GI: Added a 'None' mode for emissive GI contribution in the standard shader GUI.
    
*   GI: Added mixed area lights to culling results, which enable mixed rectangular lights in HDRP.
    
*   GI: Added Rendering.GraphicsSettings.realtimeDirectRectangularAreaLights to enable HDRP to provide direct realtime area lighting.
    
*   GI: Improved baking speed for the Progressive lightmapper in cases with many Light Probe sets in the Scene.
    
*   GI: Improved GPU Lightmapper performance by generating many rays per texel/Light Probe for indirect lighting. Optimized direct lighting by using compaction.
    
*   GI: Improved the GPU Lightmapper performance by generating many rays per texel/Light Probe for direct lighting.
    
*   GI: Optimized time to first lit texel for the progressive lightmappers by multithreading heavy functions.
    
*   GI: Realtime GI now uses correct lightomg falloff for indirect Lights when you use configurable light falloff.
    
*   GI: Reduced GPU memory footprint for the GPU Lightmapper when baking lighting. This is done by compressing normal vectors and albedo.
    
*   GI: The GPU Lightmapper now supports the Optix AI denoiser.
    
*   GI: Upgraded Optix AI Denoiser to version 6. This new version has better performance and a lower memory footprint.
    
*   Graphics: Added profiler markers for the Made with Unity splash screen.
    
*   Graphics: Added sprite Mesh support for custom splash screen logos. You can now use tight mesh mode and Vector sprites.
    
*   Graphics: Added SRP hooks for detail rendering Shaders.
    
*   Graphics: Added support for Dynamic Resolution Scaling to the Lightweight Rendering Pipeline.
    
*   Graphics: Added the ability to disable the blur on the Made with Unity splash screen. background.
    
*   Graphics: Asynchronous Shader compilation: Minimized cyan dummy shader flashes by variant tracking and warmup.
    
*   Graphics: Deferred the creation of command buffers and render encoders until they are needed in Metal.
    
*   Graphics: Improved the performance of asyncronous Texture loading on the PS4 by fixing a rendering stall that occured when you created a 2D Texture.
    
*   Graphics: The SRP Batcher is now supported on Xbox DirectX11.
    
*   Graphics: You can now use the SRP batcher on OpenGL 4.2+ and OpenGL ES 3.1+.
    
*   iOS: Added new iOS device (released in 2018) identification support to the Profiler.
    
*   iOS: Added `LowPowerModeEnabled` and `WantsSoftwareDimming` properties to `iOS.Device` and a `Brightness` Property to `Screen` (currently only supported on iOS).
    
*   iOS: Can now select architecture for native plugins on iOS & TvOS.
    
*   iOS: ReplayKit improvements:
    
    *   For local recordings, we can now capture the local camera, microphone, and screen.
    *   The size of the preview window overlay can now be adjusted.
    *   Added `ReplayKit.isPreviewControllerActive`, `ReplayKit.PauseBroadcasting`, and `ReplayKit.ResumeBroadcasting`.
*   Kernel: Improveed the performance of the internal Matrix4x4 Invert method that Rendering and Cameras primarily use.
    
*   macOS: Native plugins with the .dylib file extension are now supported.
    
*   Mobile: Improved performance of async texture loading on iOS to remove a rendering stall when 2D textures are created.
    
*   Package Manager: Added support to include built-in packages in the Project as dependencies of other packages.
    
*   Package Manager: Improved package visibility in the Project view and the Object Picker.
    
*   Package Manager: Improved Undo/Redo and Cancel button handling in the Package Manifest Importer window.
    
*   Package Manager: Installed modules now appear in the Dependencies list alongside package dependencies.
    
*   Particles: Made missing External Forces module properties available in scripting API.
    
*   Physics: Upgraded the cloth library to use NVIDIA's NvCloth Library instead of the deprecated PxCloth.
    
*   Plugins: Added Unity Companion license to the Plugin API header.
    
*   Profiler: Added names to Unity-created threads in VTune profiler.
    
*   Profiler: Added reduced profiler overhead when flushing data from Job threads.
    
*   Profiler: Added single threaded platform support to the Memory Profiler.
    
*   Profiler: Made players show up consistently in the profiler list,when there are a lot of players running on the same network.
    
*   Profiler: Provide dynamic code (Mono JIT) information to VTune Amplifier.
    
*   ps4: Improved PS4 Additional content to support multiple products.
    
*   Scripting: Enabled incremental Garbage Collection in the Editor.
    
*   Scripting: The managed debugger now outputs the network port it's listening on to the player log.
    
*   Shaders: Defined `UNITY_SEPARATE_TEXTURE_SAMPLER` in `HlslSupport.cginc` for platforms capable of separate texture and sampler objects.
    
*   Shaders: Moved 38 built-in keywords to local keywords. Shaders inspector now shows used global/local keywords by shader.
    
*   Terrain: Made changes such that the system no longer generates basemap Textures if you do not use the basemap shader.
    
*   Terrain: Made changes to allow local keywords, which are defined with `multi_compile_local` or `shader_feature_local`, for Terrain shaders.
    
*   Terrain: Removed the Terrain Material enum type, and changed built-in Terrain Materials into selectable Assets.
    
*   Timeline: Added mute to Track groups.
    
*   Timeline: Added new user interface to animate track and clip properties.
    
*   Timeline: Added the ability to override the loop setting on Animation clips. (1140766, 1144743)
    
*   Timeline: Implemented a new read-only mode for when a Timeline asset is not editable. This is caused by either the file readonly flag or source control.
    
*   UI: Added ability to modify the UI Dropdown's Alpha fade when showing and hiding.
    
*   UI: Added the ability to modify the number of pixels per unit used when calculating sliced and tiled sprites.
    
*   UI: Removed the `spritePacking` tag option from the TextureImporter when not using the legacy packing mode.
    
*   UI Elements: Prevented exceptions thrown by user code from corrupting the UI renderer.
    
*   Video: Improved the documentation for platform strings used by VideoClipImporter methods.
    
*   Windows: Added a Player Setting for reverting to BltBlt swapchain model which was used before 2019.1. This enables several scenarios like transparent window to be used once again.
    
*   XR: Added GPU Profiler support for Oculus Quest and Oculus Go.
    
*   XR: Added Low Overhead Mode setting to Oculus (Android) to do less driver validation, which can potentially increase performance.
    
*   XR: Moved the Google VR Cardboard and Daydream support to a package and updated to version 1.180.
    
*   XR: Updated Oculus to use the 1.36 plugin.
    
*   XR: Updated Vuforia to version 8.0.10.