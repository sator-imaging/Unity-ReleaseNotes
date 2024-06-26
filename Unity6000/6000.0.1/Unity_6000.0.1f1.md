# Unity 6000.0.1f1
Wed, 08 May 2024 15:11:21 GMT  
https://unity.com/releases/editor/whats-new/6000.0.1

### Known Issues in 6000.0.1f1

- 3D Physics: 3D Physics Layer Collision Matrix elements are misaligned when new Layers are added
    ([UUM-61750](https://issuetracker.unity3d.com/issues/3d-physics-layer-collision-matrix-elements-are-misaligned-when-new-layers-are-added))

- DOTS: Job scheduling with batching is slow with dependencies and worker threads have poor utilization
    ([UUM-72097](https://issuetracker.unity3d.com/issues/job-scheduling-with-batching-is-slow-with-dependencies-and-worker-threads-have-poor-utilization))

- Graphics Optimization: Crash on PrepareDrawShadowsCommandStep1 when selecting a camera while the Occlusion Culling window is open
    ([UUM-506](https://issuetracker.unity3d.com/issues/crash-on-preparedrawshadowscommandstep1-when-selecting-a-camera-while-the-occlusion-culling-window-is-open))

- Lighting: [HDRP] Light doesn't bounce off terrains
    ([UUM-71171](https://issuetracker.unity3d.com/issues/hdrp-light-doesnt-bounce-off-terrains))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Universal RP: Errors are thrown and the Scene view is not rendered when Rendering Path is set to Deferred
    ([UUM-63928](https://issuetracker.unity3d.com/issues/errors-are-thrown-and-the-scene-view-is-not-rendered-when-rendering-path-is-set-to-deferred))

- Vulkan:  Editor crash when changing Vulkan Number of Swapchain Buffers
    ([UUM-60016](https://issuetracker.unity3d.com/issues/vulkan-editor-crash-when-changing-vulkan-number-of-swapchain-buffers))



### 6000.0.1f1 Release Notes

#### Improvements

- SRP Core: Improved the Native Render Pass CPU performance by implementing a Render Pass pooling system \(URP RG\).

- SRP Core: Reworked the additional properties.
    (UUM-59559)

- WebGL: Rebalanced the WebGL audio memory pool size values.
    ([UUM-49655](https://issuetracker.unity3d.com/issues/webgl-returns-error-messages-when-playing-many-sounds-simultaneously))



#### API Changes

- Graphics: Added: SystemInfo.supportsDepthFetchInRenderPass to check if RenderPass' depth attachment can be used as input, added UNITY_PLATFORM_SUPPORTS_DEPTH_FETCH shader macro to detect it in shader code.

- URP: Changed: Fixing resource setters in the URP UniversalResourceData that should not be public and will introduce errors when used.



#### Changes

- Editor: Added a warning dialog to prevent users from closing the Multiplayer Playmode Clone window.



#### Fixes

- 2D: Fixed an issue with Sprite preview where a small Sprite would have its pixels drawn inaccurately.
    ([UUM-68491](https://issuetracker.unity3d.com/issues/image-of-the-sprite-is-not-accurate-when-previewing-it-in-the-inspector-window))

- 2D: Fixed an issue with undo for GridSelection where undoing or redoing does not restore a GridSelection properly.
    ([UUM-70084](https://issuetracker.unity3d.com/issues/tile-paint-action-disappears-from-undo-history-when-tile-selection-tool-has-been-used-beforehand))

- 2D: Fixed issue where the error log "ScriptableRenderContext::ShouldUseRenderPipeline\(\)" repeats continuously when running the DragonCrashers project in DX12 graphics mode.
    (UUM-69883)

- Android: Cached libUnity and il2cpp image info for Android stacktrace optimizations.

- Android: Fixed a crash that occurred when destroying and re-creating `WebCamTexture` on the same frame.
    ([UUM-69176](https://issuetracker.unity3d.com/issues/android-player-crashes-when-calling-stop-and-play-of-webcamtexture))

- Android: Fixed the IMGUI input even position when screen is scaled to different resolution than the view it's in with input backend set to *New Input*.
    (UUM-68787)

- Android: Fixed unexpected permissions when using `.androidlibs`.
    ([UUM-69911](https://issuetracker.unity3d.com/issues/android-with-the-latest-unity-6-editor-default-apk-permissions-are-not-being-set-correctly))

- Android: Fixed warnings from deprecated Gradle attributes.
    (UUM-70596)

- Android: Modified permission requests to queue instead of being sent as a batch, to fix an issue where requests were closing when multiple permission requests were sent.
    ([UUM-47781](https://issuetracker.unity3d.com/issues/android-permission-requests-are-automatically-denied-when-write-permission-is-set-to-external-sd-and-show-splash-screen-is-disabled))

- Android: The symbols are no longer included in AAB when manually building gradle project \(e.g., from Android Studio\), if the *Symbols output options* is not set to *App Bundle*. Unity will instead use the `android.bundle.includeNativeDebugMetadata` property.
    (UUM-69888)

- Apple TV: Fixed a crash that occurred in UnityWebRequest when running on tvOS versions lower than 17.
    ([UUM-69946](https://issuetracker.unity3d.com/issues/tvos-making-any-unitywebrequest-request-on-an-appletv-crashes-the-app-on-tvos-versions-below-17-dot-0))

- Asset Import: Fixed an issue where older assets referencing URP materials have missing asset preview thumbnails.
    ([UUM-41411](https://issuetracker.unity3d.com/issues/prefab-thumbnails-are-only-shown-when-the-prefabs-are-reimported))

- Audio: Fixed an issue that would cause the yellow lines that shows the amount of randomisation that is applied in the audio random container to be drawn incorrectly.
    (UUM-50328)

- Build Pipeline: Fixed a crash that occurred when building `AssetBundles` with Multi-Process building enabled.
    (UUM-59121)

- Core: Fixed an issue where APV generates bricks of excluded subdivision levels.
    (UUM-70558)

- Core: Fixed an issue where APV validity sampling ignored light layers.
    (UUM-70560)

- Core: Fixed an issue where APVs would load slowly.
    (UUM-70561)

- Core: Fixed errors that occurred when using baked GI node on builtin.
    ([UUM-70376](https://issuetracker.unity3d.com/issues/shader-errors-are-thrown-when-using-baked-gi-node-within-the-shader-graph))

- DX12: Fixed `ComputeBuffer CopyCount` to return correct value following multiple compute dispatches.
    ([UUM-66900](https://issuetracker.unity3d.com/issues/directx-12-copycomputebuffercount-is-getting-a-wrong-value-when-the-resource-transition-is-missing))

- DX12: Improved the consecutive drawcalls with UAV that write to the same target to respect render ordering.
    (UUM-66473)

- Editor: A progress pie chart has been added to appear in the macOS dock when Unity first opens your project.
    ([UUM-68465](https://issuetracker.unity3d.com/issues/macos-splash-screen-doesnt-display-progress-in-the-dock))

- Editor: Added a fix for `UnityEngine.Bindings.ThrowHelper.ThrowNullReferenceException` after deleting a profile in the Build Profile window.
    (UUM-69505)

- Editor: Exposed an option in the Unity's *Preferences* settings to switch the Editor's default rendering mode between *SDF* or *Bitmap*.
    ([UUM-49006](https://issuetracker.unity3d.com/issues/blurry-text))

- Editor: Fixed a crash that was caused by the shader variant collection \(SVC\) shaders with dynamic branching when entering the Play mode.
    ([UUM-70277](https://issuetracker.unity3d.com/issues/crash-on-shaderlab-shaderstate-applyshaderstate-when-entering-play-mode-and-calling-shaderwarmup-dot-warmupshaderfromcollection-with-a-shader-that-has-dynamic-branch))

- Editor: Fixed ADB performance.
    ([UUM-70242](https://issuetracker.unity3d.com/issues/adb-provider-is-really-slow))

- Editor: Fixed an issue where IME input would not work with Input System when using Chinese \(Simplified\) input bug resolution.

- Editor: Fixed an issue where sprites wouldn't be generated due to incorrect NPOT scaling setting.
    ([UUM-67831](https://issuetracker.unity3d.com/issues/sprites-can-not-be-generated-from-textures-with-npot-scaling-warning-is-displayed-when-importing-a-texture-via-texture-importer-preset-feature))

- Editor: Fixed an issue where the clicking *Open Scene List* in the Build Profile Window highlights correct list option.
    ([UUM-68478](https://issuetracker.unity3d.com/issues/clicking-open-scene-list-doesnt-highlight-the-scene-list-option-in-the-build-profiles))

- Editor: Fixed an issue with word and paragraph selection.
    ([UUM-67715](https://issuetracker.unity3d.com/issues/the-caret-is-placed-on-the-wrong-side-of-the-double-clicked-word-when-selecting-text))

- Editor: Fixed crash in LMDB_Transaction::AbortAndRestart\(\).
    (UUM-70115)

- Editor: Fixed crash of an import worker process during asset importing which results in "Unexpected transport error from import worker 0" error in the Editor log.
    ([UUM-64341](https://issuetracker.unity3d.com/issues/unexpected-transport-error-from-import-worker-0-error-is-thrown-when-importing-an-asset))

- Editor: Fixed infinite recurssion when loading assemblies with circular references in the Editor.
    ([UUM-68119](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-selecting-quit-in-a-fatal-error-pop-up))

- Editor: Fixed issue with text being corrupted under certain circumstances.
    ([UUM-67343](https://issuetracker.unity3d.com/issues/some-information-in-the-ui-toolkit-event-debugger-is-rendered-incorrectly-while-in-play-mode))

- Editor: Fixed issue with text being corrupted under certain circumstances.
    ([UUM-68077](https://issuetracker.unity3d.com/issues/ui-elements-get-visually-broken-in-the-game-view-when-the-elements-are-recalled-in-play-mode))

- Editor: Fixed materials with shaders using grab passes that were generating `incompatible keyword space` assertions.
    ([UUM-60832](https://issuetracker.unity3d.com/issues/material-using-a-particle-standard-unlit-shader-with-rendering-mode-set-to-fade-additive-or-subtractive-causes-console-errors-to-be-thrown-when-the-editor-is-active))

- Editor: Fixed the context menu function in the Build Profile Inspector so that its reset button no longer produces errors when pressed.
    ([UUM-61000](https://issuetracker.unity3d.com/issues/build-profile-the-console-displays-invalidoperationexception-the-operation-is-not-possible-when-moved-past-all-properties-next-returned-false-after-the-reset))

- Editor: Fixed the issue with the scene-view filtering that would grey out unfiltered objects when using URP Deferred in the RenderGraph's Compatibility mode.
    ([UUM-22103](https://issuetracker.unity3d.com/issues/the-scene-view-is-not-greyed-out-when-searching-in-the-scene-with-urp-deferred-rendering-path))

- Editor: Fixed the TLS Allocator errors that were logged when creating a new project with 3D template with *Connect to Unity Cloud* enabled.
    ([UUM-61109](https://issuetracker.unity3d.com/issues/console-error-tls-allocator-alloc-temp-tls-underlying-allocator-alloc-temp-main-has-unfreed-allocations-size-37-with-warnings-and-messages-is-thrown-when-opening-a-new-project-for-the-first-time))

- Editor: Fixed the `MissingComponentExceptions` thrown every frame error that appeared when removing a `TerrainCollider` component from a Terrain object. It is replaced with a warning in the Inspector for every tool that involves painting \(Paint Terrain, Paint Trees, Paint Details\). The warning message also includes a button that allows the user to easily add/enable the `TerrainCollider` component.
    ([UUM-67250](https://issuetracker.unity3d.com/issues/missingcomponentexception-errors-are-thrown-when-using-terrain-with-no-terrain-collider))

- Editor: Fixed transmission settings so that they're affected by volumetric clouds' shadows.
    (UUM-69817)

- Editor: Removed obsolete warnings about differing baking backends when using multi-scene setups.

- Editor: Updated error message thrown when trying to load a scene not added to the active profile or shared scene list.
    ([UUM-61399](https://issuetracker.unity3d.com/issues/outdated-naming-of-build-settings-error-message-when-changing-scenes))

- Editor: Updated the RenderTextureCreationFlags.DynamicallyScalableExplicit value.
    (UUM-70474)

- Graphics: Added errors about failed texture decompression instead of letting it silently fail and upload invalid data.
    ([UUM-18354](https://issuetracker.unity3d.com/issues/texturearray-asset-format-is-not-converted-causing-runtime-artifacts-on-non-mobile-platforms))

- Graphics: Fixed an issue that occurred when editing a UniversalRenderPipelineAsset that referenced the same Renderers as the UniversalRenderPipelineAsset in use.
    ([UUM-60618](https://issuetracker.unity3d.com/issues/sliders-in-the-urp-dot-asset-throws-nullreferenceexception))

- Graphics: Fixed an issue with accumulating ambient probe lighting where the sky light multiplier is not equal to one when GPU Resident Drawer is enabled.
    ([UUM-69385](https://issuetracker.unity3d.com/issues/lighting-intensity-is-added-every-frame-when-the-gpu-resident-drawer-is-set-to-instanced-drawing-and-the-intensity-multiplier-is-set-to-over-1))

- Graphics: Fixed an issue with read-only depth in RenderPass handling on Metal.
    ([UUM-64536](https://issuetracker.unity3d.com/issues/urp-objects-are-not-rendered-in-the-game-view-when-decal-feature-and-anti-aliasing-are-enabled-on-mac-silicon))

- Graphics: Fixed D3D12 crash on integrated GPU due to missing constant buffer binding.
    (UUM-69598)

- Graphics: Fixed the issue with Shader Graph previews not updating correctly.
    ([UUM-70011](https://issuetracker.unity3d.com/issues/noise-nodes-do-not-update-after-connecting-a-time-node-to-them-in-shader-graph))

- Graphics: Fixed Vulkan color mask behavior so that color mask is applied to all render targets when separate MRT \(multi render targets\) blend is disabled.
    ([UUM-69202](https://issuetracker.unity3d.com/issues/inconsistent-colormask-behavior-in-mrt-deferred-rendering-with-vulkan-graphics-api))

- Graphics: Resolved an issue where the *Overlay Canvas* was occasionally rendered incorrectly following post effects.
    ([UUM-62691](https://issuetracker.unity3d.com/issues/canvas-is-resized-when-enabling-bloom))

- Graphics: The screen space UI overlay now scales correctly in URP with Render Graph.
    (UUM-54329)

- HDRP: Added a shortcut to modify the Advanced properties within the Water System Inspector:

- HDRP: Fixed a corruption issue when using a non square atlas and improve blit performance.
    ([UUM-64604](https://issuetracker.unity3d.com/issues/mixed-cached-shadows-on-directional-lights-not-working-correctly-when-cascade-count-is-set-to-2))

- HDRP: Fixed an issuse with viewport flickering when multi-frame rendering API is used with certain parameters.
    ([UUM-59115](https://issuetracker.unity3d.com/issues/game-view-starts-flickering-when-enabling-accumulation-with-a-set-shutter-interval-in-the-recorder-clip))

- HDRP: Fixed inconsistent text capitalizations in various parts of the Editor.
    (UUM-70038)

- HDRP: Fixed `materialValidatorDebugModeEnumIndex` so that it does not get stuck in the Rendering Debugger when enabling another mode.
    ([UUM-70780](https://issuetracker.unity3d.com/issues/material-debug-view-options-material-validator-stay-selected-when-switching-to-other-material-debug-views-in-the-rendering-debugger))

- HDRP: Improved the Rendering Debugger to allow changing the mat cap values.
    (UUM-59559)

- HDRP: Optimized water foam reprojection when it's unused.
    (UUM-70590)

- macOS: Fixed an issue with the mouse button that was stuck when focusing a window with mouse using Input System.
    ([UUM-69724](https://issuetracker.unity3d.com/issues/new-input-system-registers-mouse-down-events-when-clicking-or-dragging-the-title-bar-of-the-windowed-player-window-with-locked-cursor-on-macos))

- Networking: Fixed a UnityWebRequest crash that occurred if the texture was queried multiple times and destroyed between queries.
    ([UUM-70009](https://issuetracker.unity3d.com/issues/downloadhandlertexture-can-access-a-destroyed-texture-object-on-destruction))

- Package Manager: Fixed a Package Manager issue that prevented button states from refreshing after updating a package.
    ([UUM-44775](https://issuetracker.unity3d.com/issues/package-description-window-does-not-repaint-after-other-package-is-updated-and-button-operations-are-unavailable-until-repainted))

- Package Manager: Fixed a Package Manager issue that prevented packages from displaying when a local tarball dependency doesn't point to a file on disk.
    ([UUM-63177](https://issuetracker.unity3d.com/issues/cannot-view-installed-packages-in-package-manager-when-a-tarball-package-is-removed-from-the-project-folder))

- Package Manager: Fixed a Package Manager issue to display the *Git* label for Git packages in the *Version History* tab in the *Details* panel.
    (UUM-70055)

- Package Manager: Fixed an issue where adding packages could fail with the error message "Converting circular structure to JSON".
    ([UUM-63996](https://issuetracker.unity3d.com/issues/unable-to-add-package-due-to-converting-circular-structure-to-json-error))

- Package Manager: Fixed an issue where removing a scope from package scoped registry in Project Settings resulted in `No package to display` in Packman list view.
    (UUM-65955)

- Package Manager: Updated icons and styles to make the installed icon clearly visible in light mode.
    (UUM-70540)

- Particles: Fixed the output array size of `GetTriggerParticles` to equal the actual number of "trigger particles" so that it isn't larger than it should be and thus contain uninitialized values.
    ([UUM-68018](https://issuetracker.unity3d.com/issues/invalid-worldaabb-errors-when-using-prewarm-particles-with-triggers-set-to-callback))

- Physics 2D: Ensure that Static 2D Colliders in the Editor Scene view are updated per-frame rather than per-fixed-update when moving them outside of Play mode.
    ([UUM-15955](https://issuetracker.unity3d.com/issues/gizmo-does-not-update-correctly-when-moving-a-box-collider-2d-and-time-scale-is-less-than-1))

- Physics 2D: Fixed the issue with scene/prefab corruption that was causing the `CompositeCollider2D` to crash when any of the referred colliders were missing.
    ([UUM-70051](https://issuetracker.unity3d.com/issues/crash-on-gizmodrawingphysics2d-drawcompositecollider2dgizmo-when-opening-a-scene-that-has-corrupted-gameobjects-with-tilemap-components))

- Physics 2D: Fixed unwanted contacts when a Rigidbody2D set to use Continuous Collision Detection, catches the edges of Colliders placed side-by-side.
    (UUM-70407)

- Prefabs: Fixed issue causing crashes by having Unity not destroy removed GameObjects if they are referenced in the scene.
    ([UUM-69243](https://issuetracker.unity3d.com/issues/crash-on-attachaddedcomponents-when-opening-a-specific-project))

- Profiler: Added capacity argument checks to the ProfilerRecorder api to prevent crashes due to invalid initialization.
    (UUM-64295)

- Scene Manager: Resolved issue so that the prefab scale value does not default to zero when a prefab with canvas is modified with `EditPrefabContentsScope`.
    ([UUM-47434](https://issuetracker.unity3d.com/issues/the-prefab-scale-values-are-set-to-zero-when-the-prefab-with-a-nested-canvas-is-modified-through-a-script))

- Scene/Game View: Fixing a Gizmo from disappearing when selecting nested prefabs.
    ([UUM-67501](https://issuetracker.unity3d.com/issues/reflection-probe-gizmo-disappears-when-selecting-nested-prefabs))

- Scripting: Corrected `TransformAccess.GetLocalPositionAndRotation()` to return accurate results.
    ([UUM-62533](https://issuetracker.unity3d.com/issues/wrong-position-and-rotation-values-are-returned-when-using-transformaccess-dot-getlocalpositionandrotation))

- Scripting: Fixed an Editor crash that occured when trying to determine assembly information for a path does not belong to an assembly.
    ([UUM-64099](https://issuetracker.unity3d.com/issues/crash-on-getgroupnamefromguid-when-opening-a-specific-project))

- Serialization: Fixed a crash that occured in `SerializedProperty:CopyInternalImpl` when clicking on a specific Asset.
    ([UUM-68293](https://issuetracker.unity3d.com/issues/crash-on-serializedproperty-copyinternalimpl-when-clicking-on-a-specific-asset))

- Shaders: Improved shader import performance.
    (UUM-66848)

- SRP Core: Improved the compiler logic that detects if the current render target is being used outside the current native render pass \(e.g., when the pass is broken up by an unsafe pass\), and determines the store action for this case. The fix now ensures that the `StoreAndResolve` action is used when the resource is read by an Unsafe Pass.
    (UUM-67135)

- uGUI: Fixed an issue where the Canvas inspector would not allow all possible choices of the "Additional Shader Channels" property.
    ([UUM-64603](https://issuetracker.unity3d.com/issues/cannot-toggle-normal-or-tangent-when-selecting-in-additional-shader-channels-dropdown))

- UI Elements: Addressed the `ScrollToItem` behaviour after detachment so that it no longer scroll all the way up to the first item in a list randomly.
    ([UUM-68280](https://issuetracker.unity3d.com/issues/incorrect-scrolltoitem-behavior-when-called-on-a-deattached-listview))

- UI Elements: Resolved an issue with `ScrollToItem` so that it does not block the scroll action if it's invoked prior to a Rebuild.
    ([UUM-67721](https://issuetracker.unity3d.com/issues/mouse-scrolling-and-slider-arrows-do-not-work-when-calling-scrolltoitem-before-filling-the-itemssource-list))

- UI Toolkit: Fixed an issue that occurred when binding a ListView to a field marked as \[HideInInspector\].
    (UUM-69780)

- UI Toolkit: Fixed an issue with refreshing ListView on Undo/Redo when using custom callbacks on a bound list.
    (UUM-69779)

- UI Toolkit: Fixed an issue with the height of generic dropdown which was not set properly because of which the menu items weren't visible.
    (UUM-68404)

- UI Toolkit: Fixed an issue with the selection not refreshed when calling RefreshItems.
    (UUM-69848)

- UI Toolkit: Fixed comment parsing in the ExCSS library.
    ([UUM-44485](https://issuetracker.unity3d.com/issues/uss-parsing-error-an-unexpected-error-occurred-errors-appear-when-having-one-or-more-slash-in-the-uss-file-after-slash-star-symbols))

- UI Toolkit: Fixed errors when PropertyField was drawing an IMGUI property drawer and the SerializedObject was no longer valid.
    (UUM-69862)

- UI Toolkit: Fixed generic dropdown menu issues, where the dropdown was not dismissible after the first one was opened.
    (UUM-68406)

- UI Toolkit: Fixed null reference exception that occured when pressing the Enter key on a ListView.
    ([UUM-70108](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-pressing-the-enter-key-to-select-an-item-in-a-listview))

- UI Toolkit: Fixed the issue with `GenericDropdownMenu` that appeared cropped when displaed at the bottom of a window.
    (UUM-68407)

- UI Toolkit: \[UI Builder\] Fixed an issue where typing an invalid selector string would sometimes use a banner to display the error and sometimes use the console. The banner will now be used.
    ([UUM-63589](https://issuetracker.unity3d.com/issues/naming-selectors-with-improper-character-combinations-in-ui-builder-logs-errors-and-has-inconsistent-indications-to-users))

- Universal RP: Fixed an issue with corrupt cookie sampling when targeting mobile platforms.
    ([UUM-70600](https://issuetracker.unity3d.com/issues/cookie-looks-corrupt-in-editor-when-android-is-current-target-platform))

- URP: Added a warning the Scene to inform users about light limits.
    ([UUM-56213](https://issuetracker.unity3d.com/issues/the-realtime-point-lights-are-casting-shadows-non-dependant-on-the-surrounding-gameobjects-when-the-camera-is-being-moved-around-the-scene))

- URP: Fixed inconsistent text capitalizations in various parts of the Editor.
    (UUM-70038)

- URP: Fixed Native Render Pass to render `RenderTextureDescriptor` with the correct dimensions when the render scale is not equal to one.
    (UUM-61468)

- VFX Graph: A compilation issue occured when declaring a gradient in ShaderGraph blackboard.
    ([UUM-69751](https://issuetracker.unity3d.com/issues/shadergraph-gradients-do-not-work-with-vfx))

- VFX Graph: Added support for more HLSL function prototype declaration.
    ([UUM-64314](https://issuetracker.unity3d.com/issues/vfx-custom-type-failing-with-custom-hlsl))

- VFX Graph: Improved CustomHLSL to consider custom HLSL and includes workflow.
    (UUM-69735)

- VFX Graph: Resolved a corner case issue where the presence of multiple instances of the same buffer led to a compilation failure.
    (UUM-66018)

- Video: Fixed an issue where the video was freezing when building a project on Android.
    ([UUM-65398](https://issuetracker.unity3d.com/issues/android-video-freezes-when-built-for-android-with-specific-project))

- Video: Fixed `VideoPlayer.DecodeNextFrame` that continued decoding in Profiler even after the Video Clip stops playing after reaching the end.
    ([UUM-64898](https://issuetracker.unity3d.com/issues/videoplayer-dot-decodenextframe-continues-decoding-in-profiler-when-the-video-clip-has-finished-playing))

- Video: Resolved an issue so that video playback can be resumed when returning from the background when `VideoPlayer.isLooping` is enabled.
    ([UUM-60922](https://issuetracker.unity3d.com/issues/video-playback-stops-and-cannot-be-resumed-when-returned-from-the-background-with-videoplayer-dot-islooping-set-to-true))

- XR: Fixed a crash that occured in `CreateRenderTexture` when booting a scene on Vulkan.
    (UUM-64258)

- XR: Fixed a crash that occured in `CreateRenderTexture` when booting a scene on Vulkan.
    (UUM-68323)




#### Package changes in 6000.0.1f1

#### Packages updated

- com.unity.inputsystem: [1.8.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.8//changelog/CHANGELOG.html) to [1.8.2](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.8//changelog/CHANGELOG.html)

- com.unity.services.vivox: [16.2.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.2//changelog/CHANGELOG.html) to [16.3.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.3//changelog/CHANGELOG.html)

- com.unity.test-framework: [1.4.3](https://docs.unity3d.com/Packages/com.unity.test-framework@1.4//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.test-framework@1.4//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.8.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.8//changelog/CHANGELOG.html) to [1.9.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.9//changelog/CHANGELOG.html)

- com.unity.sharp-zip-lib: [1.3.7](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.3//changelog/CHANGELOG.html) to [1.3.8](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.3//changelog/CHANGELOG.html)