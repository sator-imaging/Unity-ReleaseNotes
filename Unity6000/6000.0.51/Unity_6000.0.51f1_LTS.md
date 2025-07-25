# Unity 6000.0.51f1 LTS
Published at Wed, 11 Jun 2025 09:43:13 GMT  
https://unity.com/releases/editor/whats-new/6000.0.51

# Known Issues in 6000.0.51f1

- Android: [GameActivity] Crash on "UnityMotionEventCallbacks::_GetPointerIdImpl" when giving 9+ simultaneous touch inputs 
    ([UUM-108743](https://issuetracker.unity3d.com/issues/android-crash-on-unitymotioneventcallbacks-getpointeridimpl-when-giving-8-simultaneous-touch-inputs))

- Cloud Diagnostics: [Android]Crash on lib/arm64/libil2cpp.so when Unity Analytics and Engine Code stripping are enabled
    ([UUM-95408](https://issuetracker.unity3d.com/issues/android-crash-on-lib-slash-arm64-slash-libil2cpp-dot-so-when-unity-analytics-and-engine-code-stripping-are-enabled))

- DirectX12: Crash on D3D12CommonShader::ApplyGpuProgram when attaching material which samples "_UnityFBInput0" to "Full Screen Pass Renderer Feature" Component
    ([UUM-105412](https://issuetracker.unity3d.com/issues/crash-on-d3d12commonshader-applygpuprogram-when-attaching-material-which-samples-unityfbinput0-to-full-screen-pass-renderer-feature-component))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Graphics Device Features: Graphics.RenderMeshIndirect does not issue multi-draw rendering commands when using a graphics API capable of multi-draw commands
    ([UUM-91617](https://issuetracker.unity3d.com/issues/graphics-dot-rendermeshindirect-does-not-issue-multi-draw-rendering-commands-when-using-a-graphics-api-capable-of-multi-draw-commands))

- Hub: Licensing Client fails to launch when opening Unity Hub
    ([UUM-103995](https://issuetracker.unity3d.com/issues/licensing-client-fails-to-launch-when-opening-unity-hub-1))

- Hub: Licensing Client fails to launch when opening Unity Hub (licensing client path is not found)
    ([UUM-103996](https://issuetracker.unity3d.com/issues/licensing-client-fails-to-launch-when-opening-unity-hub-licensing-client-path-is-not-found))

- Lighting: All baked data for all scenes using APV is always loaded in Editor
    ([UUM-104833](https://issuetracker.unity3d.com/issues/all-baked-data-for-all-scenes-using-apv-is-always-loaded-in-editor))

- Lighting: Android Player freezes on some Mali GPU devices when Lighting Cast Shadows changed to OFF at runtime
    ([UUM-105246](https://issuetracker.unity3d.com/issues/android-player-freezes-on-some-mali-gpu-devices-when-lighting-cast-shadows-changed-to-off-at-runtime))

- Mono: UnmanagedReadOrWrite objects are not disposed off when GZipStream is used in the "using" statement
    ([UUM-105139](https://issuetracker.unity3d.com/issues/unmanagedreadorwrite-objects-are-not-disposed-off-when-gzipstream-is-used-in-the-using-statement))

- Platform Audio: Android Player freezes when an Audio Source is playing and an incoming call is picked up and then hung up and the Audio Source is started again
    ([UUM-103525](https://issuetracker.unity3d.com/issues/android-player-freezes-when-an-audio-source-is-playing-and-an-incoming-call-is-picked-up-and-then-hung-up-and-the-audio-source-is-started-again))

- SRP XR: GameObjects are transparent when a custom fog renderer feature is enabled
    ([UUM-104832](https://issuetracker.unity3d.com/issues/gameobjects-are-transparent-when-a-custom-fog-renderer-feature-is-enabled))

- SRP XR: The Player renders black on a Quest headset when MSAA, Post Processing, and Spacewarm depth submission are enabled
    ([UUM-84612](https://issuetracker.unity3d.com/issues/the-player-renders-black-on-a-quest-headset-when-msaa-post-processing-and-spacewarm-depth-submission-are-enabled))

- Vulkan: [Android] Runtime performance deteriorates on certain Android devices when Graphics API is set to Vulkan on an upgraded project
    ([UUM-107530](https://issuetracker.unity3d.com/issues/build-performance-deteriorates-on-certain-android-devices-when-graphics-api-is-set-to-vulkan-on-an-upgraded-project))



# 6000.0.51f1 Release Notes

## Features

- Package Manager: Added `pinnedPackages` optional property to the project manifest. This feature forces specified direct dependencies to use their exact manifest versions during package resolution and project update.



## Improvements

- Documentation: Removed the CreateRenderGraphTexture API references from the create-custom-renderer-feature page.

- Physics: Better tooltips for PhysicsSettings window.
    (UUM-105527)



## API Changes

- Kepler: Added: Launch Arguments API.



## Changes

- Package Manager: Removed the `overrideBuiltIns` property making all `builtin` packages with semver version unable to be overridden.



## Fixes

- 2D: Fixed a rendering issue where soft shadows were darker than expected.
    (UUM-18392)

- 2D: Fixed case where last segment is missed if any of the segment uses Null Sprite inbetween.
    ([UUM-105570](https://issuetracker.unity3d.com/issues/last-segment-of-a-sprite-shape-spline-is-affected-by-other-segments-sprite-variant-change-when-no-edge-sprite-is-selected))

- 2D: Fixed FullScreenRendererFeature exception when use with Rendergraph 2D.
    ([UUM-104830](https://issuetracker.unity3d.com/issues/assertion-failed-and-argumentexception-are-thrown-and-scene-slash-game-views-do-not-render-when-render-graph-is-enabled-and-requirements-are-set-in-full-screen-pass-renderer-feature))

- 2D: Fixed hdr encoding and postprocess resolve for rendergraph 2d.
    ([UUM-105392](https://issuetracker.unity3d.com/issues/game-view-is-rendered-white-when-viewing-the-editor-with-hdr-display-and-post-proccesing-is-enabled-on-the-main-camera-with-2d-urp))

- 2D: Fixed normals to account for Sprite FlipXY.
    (UUM-104352)

- Android: Fixed Integer input field allowing multiple "-" symbols under certain conditions.
    ([UUM-103402](https://issuetracker.unity3d.com/issues/multiple-symbols-are-allowed-to-appear-in-a-row-when-inputting-dot-into-a-non-decimal-numeric-field))

- Android: The application will continue to update/render while built for 'GameActivity + run in split screen + permission dialog is shown' if RunWithFocus is set to true. Previously the application would pause for GameActivity, but would continue to run if built for Activity.
    (UUM-105630)

- Editor: Added emoji font fallback on WIN, OSX and Linux.
    (UUM-97030)

- Editor: Added new callback `onDeleteArrayElementCallback ` to `ReorderableList`. This is called from the "Delete Array Element" context menu to let you control the removal, like `onRemoveCallback`.
    ([UUM-104534](https://issuetracker.unity3d.com/issues/onremovecallback-is-not-called-when-removing-an-element-from-the-reoderablelist-using-contextmenu))

- Editor: Fixed a bug where the 'RectTransform' component values were set to NaN when scaling UI elements using the Scene Rect Tool.
    ([UUM-102690](https://issuetracker.unity3d.com/issues/rect-transform-values-are-set-to-nan-when-scaling-ui-element-with-centered-scaling))

- Editor: Fixed a bug whereby when evaluating an interrupted transition, the Animator writes the last evaluated values for all values instead of correctly defaulting to the state's current configuration.
    ([UUM-99493](https://issuetracker.unity3d.com/issues/all-animators-previous-animations-are-activated-while-transitioning-when-a-second-split-off-transition-overrides-the-first-split-off-transition))

- Editor: Fixed a Windows Editor crash on exit that could occur with some specific combinations of packages such as Google Mobile Ads and JetBrains Rider integration.
    ([UUM-103723](https://issuetracker.unity3d.com/issues/crash-on-pluginmanager-refreshplugins-when-closing-the-editor-without-making-any-changes-with-jetbrains-rider-selected-as-the-external-code-editor-and-google-mobile-ads-third-party-plugin-imported))

- Editor: Fixed an issue where Scene view gizmo icons were not loaded properly if "Load textures on demand" was enabled in project settings.
    ([UUM-104825](https://issuetracker.unity3d.com/issues/load-texture-data-on-demand-corrupts-unitys-packages-gizmos-in-scene-view))

- Editor: Fixed an issue where, for compressed cubemap texture assets, the 'CubemapInspector' would display controls that perform operations unsupported by such textures. This also fixes an issue where merely inspecting a crunched cubemap texture asset would provoke errors.
    (UUM-86485)

- Editor: Fixed case where ScreenCapture.CaptureScreenshotAsTexture\(\) could cause the player or editor to crash when a XR device was connected.
    ([UUM-103220](https://issuetracker.unity3d.com/issues/capturescreenshotastexture-fails-when-vr-headset-is-connected-and-is-inactive-during-play-mode))

- Editor: Fixed IMGUI Errors on LinuxEditor arising when RepaintImmediately\(\) called on window currently being painted.
    ([UUM-104622](https://issuetracker.unity3d.com/issues/linux-using-ctrl-plus-alt-plus-a-shortcut-for-add-component-throws-gui-rendering-errors))

- Editor: Fixed issue with TMP bloom effects not working anymore.
    ([UUM-90091](https://issuetracker.unity3d.com/issues/non-hdr-color-picker-opens-when-selecting-material-color-with-hdr-enabled))

- Editor: Fixed LinuxEditor failing to trigger some shortcuts when InputManager is disabled.
    ([UUM-104604](https://issuetracker.unity3d.com/issues/linux-shortcuts-that-use-shift-modifier-and-numbers-row-are-not-triggered))

- Editor: Fixed macOS progress bars always being shown on the main display rather than over the main Editor window.
    ([UUM-102920](https://issuetracker.unity3d.com/issues/progress-bar-defaults-to-main-monitor-when-editor-is-on-secondary-monitor))

- Editor: Fixed OverlayMenu behaviour when deleting or reverting presets.
    ([UUM-103066](https://issuetracker.unity3d.com/issues/when-reverting-all-presets-or-deleting-the-currently-chosen-preset-the-overlay-preset-is-not-switched-to-the-default-preset))

- Editor: Fixed OverlayMenu width when preset name is very long.
    ([UUM-103059](https://issuetracker.unity3d.com/issues/the-overlay-menu-preset-option-text-is-not-truncated-and-the-overlay-menu-is-unusable-at-certain-sizes-when-preset-name-is-a-long-string))

- Editor: Fixed tooltip position when mouse is over Scripting Defines in Build Profiles window.
    (UUM-104272)

- Editor: Fixed UnityEvent drawer changing the object argument when editing multiple objects.
    ([UUM-104854](https://issuetracker.unity3d.com/issues/references-placed-in-a-unityevent-change-to-the-same-reference-when-multi-selecting-their-gameobjects))

- Editor: Fixed `PlayerSettings` icon APIs so that `GetIcons`, `GetIconsForTargetGroup`, `GetIconSizes`, and `GetIconSizesForTargetGroup` return the correct icon arrays for the provided `NamedBuildTarget` or `BuildTargetGroup` argument.
    ([UUM-97474](https://issuetracker.unity3d.com/issues/player-settings-icons-are-not-retrieved-when-using-playersettings-dot-geticons-method))

- Editor: RG16 texture format is now fully supported and available in Editor Inspector.
    (UUM-81515)

- Graphics: BatchRendererGroup's OnPerformCulling function now correctly checks for job safety between the provided buffers and the JobHandle returned by the user.
    ([UUM-98559](https://issuetracker.unity3d.com/issues/no-error-slash-warning-in-console-when-batchrenderergroup-reads-draw-commands-before-culling-jobs-are-complete))

- Graphics: Fixed a potential deadlock that could freeze players when loading or unloading AssetBundles with threaded texture uploads enabled.
    ([UUM-102896](https://issuetracker.unity3d.com/issues/arm-the-player-freezes-when-awaiting-g-uploadedtexturecondvar-in-the-main-thread))

- Graphics: Fixed an issue where mesh changes would not propagate correctly when using GPU Resident Drawer and GPU Occlusion Culling.
    ([UUM-103207](https://issuetracker.unity3d.com/issues/modified-meshes-are-not-uploaded-to-gpu-in-urp-when-resident-drawer-is-enabled))

- Graphics: Fixed an issue where the value reported by "Texture.nonStreamingTextureMemory" would not update when mipmap limits were modified.
    ([UUM-79327](https://issuetracker.unity3d.com/issues/texture-dot-nonstreamingtexturememory-value-does-not-update-when-qualitysettings-dot-globaltexturemipmaplimit-is-changed))

- Graphics: Fixed duplicated color resolve when mixing native render pass and set render target workflows.
    (UUM-103751)

- Graphics: Fixed libGLES.so crash on small subset of PowerVR devices.
    (UUM-102249)

- Graphics: Fixed shadow culling not working correctly for intermediate renderers like Graphics.RenderMesh or Terrain.
    ([UUM-96217](https://issuetracker.unity3d.com/issues/terrain-detail-mesh-triangles-value-increases-when-occlusion-culling-is-used-and-cast-shadows-is-enabled-on-the-mesh))

- Graphics: Removed an assert exception in UnityEngine.Rendering.CreateDrawBatchesJob.ProcessRenderer when changing a material property of a material used in MeshRenderers with multiple submeshes, after re-importing URP or HDRP.
    ([UUM-103975](https://issuetracker.unity3d.com/issues/assertionexception-thrown-and-mesh-turns-invisible-when-changing-material-offset-manually-via-the-inspector-or-through-settextureoffset-on-a-mesh-with-more-than-one-material))

- HDRP: Prevent CustomPass using camera depth if the injection point is set to AfterPostprocess. Show a warning in the CustomPass inspector if this configuration is present.
    ([UUM-79283](https://issuetracker.unity3d.com/issues/drawrendererescustompass-onpostprocess-only-draws-within-the-original-render-area-when-dynamic-resolution-is-enabled-and-graphics-api-is-set-to-directx12))

- iOS: Fixed warning in the Xcode console when keyboard is open and changing orientation on iPad.
    (UUM-95530)

- Kernel: JobHandle.Complete\(\) goes to sleep sooner when there is no work to steal. This allows the waiting thread to give up the CPU core sooner to allow another thread to perform work or to preserve battery life.
    (UUM-83082)

- Package Manager: Fixed an issue where installing a git package using Git LFS would not work with Git LFS 3.6.0 and higher.
    (UUM-91342)

- Package Manager: Fixed the issue where Assets cannot be imported when the Asset package contains project settings and all project settings are unchanged.
    ([UUM-100078](https://issuetracker.unity3d.com/issues/assets-do-not-get-imported-from-an-asset-package-when-library-assets-in-the-asset-package-are-unchanged))

- Package Manager: Fixed the issue where extension buttons are not consistently shown.
    ([UUM-84399](https://issuetracker.unity3d.com/issues/inconsistent-logic-on-when-open-vfx-graph-samples-button-appears-on-visual-effect-graph-in-package-manager))

- Package Manager: UnityEditor.PackageManager.UI.Sample.FindByPackage will no longer throw an exception when passed an unknown package.
    (UUM-86326)

- Player: Fixed an issue where the startup logs would be missing from the normal log file \(or standard output\) when the "Capture Startup Logs" player setting was enabled.
    ([UUM-102670](https://issuetracker.unity3d.com/issues/startup-logs-are-missing-in-player-logs-when-capture-startup-logs-is-enabled))

- Terrain: Ensure that TreeRenderer position is initialized when creating Terrain camera render data.
    (UUM-104978)

- Text: Fixed IME issue.
    ([UUM-100552](https://issuetracker.unity3d.com/issues/the-textmeshpro-input-field-gets-cleared-when-characters-are-entered-using-a-japanese-keyboard-layout-and-a-suggestion-is-selected-from-the-composition-string-window))

- Text: Improved WeakReference handling to protect against the \(extremely unlikely, but still possible\) event that the GC runs between checking that the handle is alive and dereferencing it.
    (UUM-86325)

- Text: Removed redundant check for null SpriteCharacters when generating text meshes.
    (UUM-86328)

- UI Elements: Fixed the items not expanding on creation when autoExpand is set to true.
    ([UUM-107968](https://issuetracker.unity3d.com/issues/multicolumntreeview-does-not-auto-expand-foldouts-when-autoexpand-is-set-to-true))

- UI Toolkit: Batched the scroll events on fixed height virtualizations for ListView and TreeView controls.
    (UUM-55912)

- UI Toolkit: Fixed "UnityException: Load can only be called from the main thread" when generating the text meshes.
    (UUM-91740)

- UI Toolkit: Fixed incorrect reporting of 'Out of root' elements in the UI Layout Debugger.
    (UUM-86327)

- UI Toolkit: Fixed the ListView content disappearing when removing items outside of the offset.
    (UUM-104445)

- UI Toolkit: Fixed the threshold on drag when near the end of the ListView.
    (UUM-44911)

- UI Toolkit: Fixed USS selector is reparented when clicking on stylesheet after applying to element.
    ([UUM-104962](https://issuetracker.unity3d.com/issues/uss-selector-is-duplicated-when-it-is-added-to-an-element-the-action-is-undone-and-then-another-selector-is-clicked))

- Undo System: Keep undo stack in sync during project load by pausing serialization.
    (UUM-97070)

- URP: Fixed IndexOutOfRangeException by allocating size with respect to visible light's length.
    ([UUM-102022](https://issuetracker.unity3d.com/issues/an-unclear-error-occurs-when-exceeding-the-light-limit-set-in-urp-config-package))

- URP: Fixed unclear warnings when user creates more lights than the light limit when using Deferred rendering path.
    ([UUM-102023](https://issuetracker.unity3d.com/issues/property-additionalshadowparams-exceeds-previous-array-size-41-vs-32-dot-dot-dot-warning-is-spammed-when-exceeding-the-light-limit-set-in-urp-config-package))

- VFX Graph: Fixed matrix 4x4 was overflowing when displayed in a context block.
    ([UUM-102349](https://issuetracker.unity3d.com/issues/matrix4x4-exposed-property-is-cropped-in-subgraph-block))

- VFX Graph: Fixed rendering of volumetric output connected to particle strips.
    ([UUM-102654](https://issuetracker.unity3d.com/issues/connecting-volumetric-fog-output-to-a-strip-breaks-compilation-and-throws-errors))

- VFX Graph: Fixed VFX command culling when using Custom Passes in HDRP.
    ([UUM-83094](https://issuetracker.unity3d.com/issues/frustumculling-is-not-functional-in-vfx-graph-rendered-with-custom-pass-when-using-aggregatecullingparameters))

- Video: Fixed double invocation of onLoopPoint callback when `skipOnDrop` is false and codec is decoding to memory.
    ([UUM-97953](https://issuetracker.unity3d.com/issues/videoplayer-dot-looppointreached-invokes-twice-when-waitforfirstframe-is-enabled))




## Package changes in 6000.0.51f1

## Packages updated

- com.unity.visualscripting: [1.9.6](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) to [1.9.7](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.12//changelog/CHANGELOG.html) to [1.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.13//changelog/CHANGELOG.html)

- com.unity.ai.navigation: [2.0.7](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) to [2.0.8](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- com.unity.polyspatial: [2.2.4](https://docs.unity3d.com/Packages/com.unity.polyspatial@2.2//changelog/CHANGELOG.html) to [2.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial@2.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.visionos: [2.2.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@2.2//changelog/CHANGELOG.html) to [2.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@2.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.xr: [2.2.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@2.2//changelog/CHANGELOG.html) to [2.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@2.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.extensions: [2.2.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@2.2//changelog/CHANGELOG.html) to [2.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@2.3//changelog/CHANGELOG.html)

- com.unity.xr.visionos: [2.2.4](https://docs.unity3d.com/Packages/com.unity.xr.visionos@2.2//changelog/CHANGELOG.html) to [2.3.1](https://docs.unity3d.com/Packages/com.unity.xr.visionos@2.3//changelog/CHANGELOG.html)