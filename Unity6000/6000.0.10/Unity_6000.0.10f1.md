# Unity 6000.0.10f1
Published at Wed, 10 Jul 2024 16:45:22 GMT  
https://unity.com/releases/editor/whats-new/6000.0.10

# Known Issues in 6000.0.10f1

- Asset - Database: OnAfterDeserialize is not called when Prefabs are instantiated using InstantiateAsync
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- Asset Bundles: The resource is not properly referenced when there is a dependency on another asset bundle
    ([UUM-74871](https://issuetracker.unity3d.com/issues/the-resource-is-not-properly-referenced-when-there-is-a-dependency-on-another-asset-bundle))

- Audio Random Container: Play on awake does not work with an audio random container when instantiating a game object
    ([UUM-74723](https://issuetracker.unity3d.com/issues/play-on-awake-does-not-work-with-an-audio-random-container-when-instantiating-a-game-object))

- Build Settings Window: [Windows] Hold on is being shown after switching platform and only disappears after hovering on the window 
    ([UUM-74797](https://issuetracker.unity3d.com/issues/windows-hold-on-is-being-shown-after-switching-platform-and-only-disappears-after-hovering-on-the-window))

- DirectX12: Crash on D3D12 when entering Play Mode in High Definition 3D Core project's Environment scene
    ([UUM-74769](https://issuetracker.unity3d.com/issues/crash-on-d3d12-when-entering-play-mode-in-high-definition-3d-core-projects-environment-scene))

- DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when selecting the “Cloud Layer“ option in Visual Environment component
    ([UUM-75220](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-selecting-the-cloud-layer-option-in-visual-environment-component))

- DOTS: Job allocator contention causes slow job execution
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- Editor Platform: The "Hold On" dialog box persists when entering the Play Mode
    ([UUM-74916](https://issuetracker.unity3d.com/issues/the-hold-on-dialog-box-persists-when-entering-the-play-mode))

- Environment Effects: Visible light glares appear on GameObjects when a Volumetric Clouds effect is added to the Sky and Fog Volume
    ([UUM-74923](https://issuetracker.unity3d.com/issues/visible-light-glares-appear-on-gameobjects-when-a-volumetric-clouds-effect-is-added-to-the-sky-and-fog-volume))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Lighting: Alpha clipping in lightbaking does not work as expected in HDRP
    ([UUM-74735](https://issuetracker.unity3d.com/issues/lightmap-has-artifacts-when-generating-lighting))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Vulkan:  Editor crash when changing Vulkan Number of Swapchain Buffers
    ([UUM-60016](https://issuetracker.unity3d.com/issues/vulkan-editor-crash-when-changing-vulkan-number-of-swapchain-buffers))



# 6000.0.10f1 Release Notes

## Improvements

- Accessibility: Added information about the minimum Android version supported \(Android 8\) on the AssistiveSupport class.
    (UUM-64651)

- Graphics: \[Internal\] Add a IUnityXRTextureManagerInterface and a function pointer in it which is called when VR RenderTexture is destroyed.<br>
    `vrDevice->OnTextureDestroyed(ptr);`.

- HDRP: Improved decal region resolution on non-infinite surfaces.

- HDRP: Optimised the water vertex shader.

- HDRP: Reduced memory usage when foam is disabled.

- IL2CPP: Updated the GC bitmap size on 64 bit platforms.

- Mono: Added Unity Embedding API to load assembly refs with error checking.

- Mono: Updated the GC bitmap size on 64 bit platforms.

- Universal RP: Changed the URP render pass names for consistency in the RenderGraph viewer, the Profiler, and the frame debugger.



## API Changes

- iOS: Deprecated: Native function UnityRegisterRenderingPluginV5 has been deprecated, UnityRegisterPlugin is exact replacement.<br>
    No real functional changes.
    (UUM-74319)

- Physics: Added: Fixed 'Reuse Collision Callbacks' behaviour in CharacterController; when on it now prevents garbage generation when using the OnControllerColliderHit callback.
    ([UUM-60515](https://issuetracker.unity3d.com/issues/charactercolliders-oncontrollercolliderhit-allocates-80b-of-gc))



## Fixes

- AI: Nav mesh agent will not move in Y axis if the surface is rotated to 90 in X.
    ([UUM-49446](https://issuetracker.unity3d.com/issues/nav-mesh-agent-is-unable-to-move-on-the-y-axis-when-the-navmeshsurface-gameobject-is-rotated-90-degrees))

- Android: Fixed detection of Play Asset Delivery support to avoid problems if there is play.core dependency in the project.
    (UUM-74252)

- Android: Fixed ndkVersion attribute missing from custom Gradle templated files.
    (UUM-74561)

- Asset Import: Fixed a performance regression causing increased import times.
    (UUM-73645)

- Build Pipeline: Fixed a regression introduced in unity 2023.1 that caused the Build Profiles UI to erroneously disable cross-compiling for linux on windows and mac hosts.
    (UUM-67303)

- Core: Fixed missing option to offset probe at runtime.
    (UUM-74499)

- Core: Fixed shader warnings in editor APV shaders.
    (UUM-69985)

- Core: Fixed shader warnings in runtime APV shaders.
    ([UUM-74315](https://issuetracker.unity3d.com/issues/shader-warnings-in-probevolumedata-are-thrown-after-building-a-high-definition-3d-sample-template-project))

- Editor: Enabled animation clip list to be excluded in animation settings for model importer Presets.
    (UUM-73901)

- Editor: Fixed an issue with point cache and vector field that could cause unexpected import when referenced from VFX.
    (UUM-73877)

- Editor: Fixed for bring to front always removing and re adding the overlay.
    (UUM-74512)

- Editor: Fixed HDRP area light culling.
    ([UUM-70390](https://issuetracker.unity3d.com/issues/area-light-is-culled-when-camera-frustrum-is-outside-the-lights-range))

- GI: Avoided a memory leak and null pointer references when the Lighting window closes while APV is baking.
    ([UUM-71743](https://issuetracker.unity3d.com/issues/closing-the-lighting-window-while-generating-lighting-and-having-apvs-in-the-scene-leads-to-a-memory-leak))

- GI: Enabled the CPU lightmapper to run on ARM-based Windows machines.
    (UUM-74103)

- GI: Fixed error occuring when baking APV with rendering layers and mesh having multiple submeshes.
    (UUM-74749)

- GI: Improved robustness of `IsRunningLightmapping()`.
    (UUM-74944)

- Graphics: Fixed a crash on Linux Editor where Vulkan may recreate SwapChains while the previous SwapChain's images may still be in use by a command buffer.
    ([UUM-73447](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-when-using-nvidia-drivers-545-and-graphics-api-set-to-vulkan))

- Graphics: Fixed broken URL for documentation on Texture2D.
    ([UUM-74607](https://issuetracker.unity3d.com/issues/texture-2d-reference-links-to-missing-documentation))

- Graphics: Fixed shader compilation timeout error on console platforms.
    ([UUM-72861](https://issuetracker.unity3d.com/issues/shader-timeout-error-in-pathtracingmain-when-building-the-player-via-script-using-buildplayer))

- Graphics: The condition for the "Graphics.CopyTexture with a region will not copy readable texture data for compressed formats" warnings has been fixed to match the documentation so that when a CPU copy would not normally be attempted \(ie., at least one texture is not readable\), the warnings will not appear.
    ([UUM-73721](https://issuetracker.unity3d.com/issues/graphics-dot-copytexture-with-a-region-will-not-copy-readable-texture-data-for-compressed-formats-warnings-are-thrown-when-copying-compressed-texture-regions))

- HDRP: Changed `ProbeSettings.cubeResolution` field from internal to public.
    ([UUM-74949](https://issuetracker.unity3d.com/issues/hdrp-probessettings-dot-cuberesolution-is-internal-and-can-not-be-changed-easilly))

- HDRP: Cull water decals based on distance to camera.
    (UUM-74812)

- HDRP: Fixed decals not updated in atlas when ShaderGraph is saved.

- HDRP: Fixed deformation offset when water surface is rotated.

- HDRP: Fixed error when drawing water excluder gizmo.
    (UUM-74809)

- HDRP: Fixed foam and deformation using separate regions.

- HDRP: Fixed lens flare screen space and bloom frame settings confusion.
    ([UUM-74226](https://issuetracker.unity3d.com/issues/hdrp-enabling-sslf-overrides-disabling-bloom-in-the-frame-settings-which-is-not-super-user-frendly))

- HDRP: Fixed range remap for decal materials.
    (UUM-73754)

- HDRP: Fixed water decal gizmo when scale is non uniform.

- HDRP: Fixed water decals not affecting simulation mask.

- HDRP: Fixed water mask applied before deformation.
    (UUM-74810)

- IL2CPP: Fixed possible crash in fully shared generic code at calls at the generic code generation limit.
    (UUM-73629)

- Installer: Updated OpenCL compatibility pack to 1.2404.1.0.
    (UUM-72730)

- License: Fixed a bug where normal floating communication regarding feature status would generate too many log messages.

- License: Fixed a bug where web proxy credentials would not be found when added through a dialog triggered by macOS/Safari after web proxy auto-discovery was enabled.

- macOS: Fixed forward and back buttons being recognized as middle button.
    ([UUM-70259](https://issuetracker.unity3d.com/issues/macos-forward-and-backward-mouse-buttons-are-recognized-as-middle-mouse-button))

- Mobile: Enabled UnitySendMessage to now accept null arguments. This is treated the same way as an empty string.
    (UUM-74320)

- Mono: Fixed issue that caused some stack traces on Windows ARM64 to fail to generate.
    (UUM-65149)

- Mono: Fixed memory leak when validating a SSL certificate.
    ([UUM-72433](https://issuetracker.unity3d.com/issues/ios-memory-leaks-when-using-the-sslstream-class))

- Particles: Enabled converting particles trail vertex color to linear space when needed.
    ([UUM-71125](https://issuetracker.unity3d.com/issues/the-particle-system-trail-module-creates-trails-with-a-lighter-coloring-than-the-particles-when-the-color-space-is-set-to-linear))

- Particles: Fixed crash when calling Camera.Render during OnApplicationQuit.
    ([UUM-55832](https://issuetracker.unity3d.com/issues/crash-when-calling-camera-dot-render-during-onapplicationquit-while-cast-shadows-is-checked-in-the-particle-system-component))

- Physics: Fixed an issue where collider trigger event dispatching would incorrectly keep some trigger pairs when processing PhysX trigger events.
    ([UUM-74444](https://issuetracker.unity3d.com/issues/inaccurate-collision-detection-in-ontriggerstay-when-alternating-iskinematic-and-collision-detection-modes-in-fixedupdate))

- Scripting: Fixed awaitable cancellation preventin other awaitables from successful completion.
    (UUM-69613)

- Scripting: Prevented a crash when processing a C\# assembly that has invalid assembly references.
    ([UUM-66498](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-opening-a-specific-project))

- SRP Core: Fixed a null reference exception on the Graphics Settings stripper.
    ([UUM-74223](https://issuetracker.unity3d.com/issues/macos-unity-render-pipeline-nullreferenceexception-errors-appear-when-building-standalone))

- UI Toolkit: Fixed an issue where ListView would not automatically call RefreshItems when autoAssignMode is used.
    ([UUM-72871](https://issuetracker.unity3d.com/issues/listview-does-not-automatically-update-when-using-data-binding))

- Undo System: Improved performance of recording property modifications for large object groups.
    ([UUM-53686](https://issuetracker.unity3d.com/issues/editor-hangs-for-several-seconds-when-changing-static-flags))

- Universal RP: Fixed ScriptableRenderPass.profilerSampler being null in Compatibility mode. This will now only be null in release \(non-dev\) when using RenderGraph. This nullification was done previously as a small performance optimization.
    (UUM-74696)

- URP: Fixed CopyDepthPass setup causing Vulkan validation errors under specific circumstances.
    ([UUM-60387](https://issuetracker.unity3d.com/issues/android-mali-vulkan-does-not-render-object-after-depthcopypass))

- URP: Fixed the yflip issue when depth texture is required and color texture is not required in RenderGraph compatibility mode.
    ([UUM-70472](https://issuetracker.unity3d.com/issues/cameradepthtexture-is-flipped-upside-down-when-urp-is-rendering-without-the-final-blit))

- VFX Graph: Custom HLSL can be missing when connected to several contexts.
    (UUM-74518)

- VFX Graph: Fixed an exception when trying to create curl noise sub-variant nodes.
    ([UUM-72985](https://issuetracker.unity3d.com/issues/vfx-argumentexception-error-thrown-when-trying-to-add-slash-create-curl-noise-node))

- VFX Graph: Fixed potential crash and correctness when using a system with multiple Volumetric Fog Outputs.
    (UUM-73870)

- VFX Graph: Fixed SpawnIndex attribute when using instancing.
    ([UUM-74856](https://issuetracker.unity3d.com/issues/vfx-graph-spawnindex-values-are-wrong-with-instancing-on-and-several-vfx-instances))

- VFX Graph: Fixed variadic attributes to not be allowed to be used in custom HLSL code.
    ([UUM-74375](https://issuetracker.unity3d.com/issues/the-visual-effect-graphs-custom-hlsl-node-does-not-generate-errors-when-the-hlsl-code-used-is-incorrect))

- VFX Graph: Improved how the sleep state is updated for particle systems receiving GPU events.
    ([UUM-73758](https://issuetracker.unity3d.com/issues/the-visual-effect-gpu-event-is-forced-into-sleep-until-another-event-is-sent-when-the-visual-effect-consists-of-two-particle-systems-that-communicate-with-trigger-event-set-to-on-die))

- VFX Graph: Wrong mesh rendered with instancing, when using multi mesh and exposed submesh mask.
    (UUM-74240)

- Video: \[Android\] The first few seconds of the video audio is distorted on the Android Player.
    ([UUM-69721](https://issuetracker.unity3d.com/issues/android-the-first-few-seconds-of-the-video-audio-is-distorted-on-the-android-player))

- WebGL: Disabled URP Depth Priming support due to issues with Apple Arm64 GPUs.

- Windows: Fixed issue with non-native Refreshrate not being restored in Exclusive Fullscreen mode upon restart.
    ([UUM-62542](https://issuetracker.unity3d.com/issues/player-refresh-rate-is-not-restored-after-restarting-when-setting-the-refresh-rate-to-a-non-native-one-in-exclusivefullscreen-mode))




## Package changes in 6000.0.10f1

## Packages updated

- com.unity.microsoft.gdk: [1.0.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.1//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk.tools: [1.0.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.1//changelog/CHANGELOG.html)