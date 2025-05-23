# Unity 6000.0.45f1 LTS
Published at Wed, 02 Apr 2025 17:28:25 GMT  
https://unity.com/releases/editor/whats-new/6000.0.45

# Known Issues in 6000.0.45f1

- Analytics: [Android]Crash on lib/arm64/libil2cpp.so when Unity Analytics and Engine Code stripping are enabled
    ([UUM-95408](https://issuetracker.unity3d.com/issues/android-crash-on-lib-slash-arm64-slash-libil2cpp-dot-so-when-unity-analytics-and-engine-code-stripping-are-enabled))

- Culling: "Draw Additional Lights Shadowmap" calls increase when custom MaterialBlockProperty is used
    ([UUM-97309](https://issuetracker.unity3d.com/issues/draw-additional-lights-shadowmap-calls-increase-when-custom-materialblockproperty-is-used))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Graphics Device Features: Crash on TypeContainer<int>::rtti when deleting a Render Texture that is used by the Main Camera
    ([UUM-101233](https://issuetracker.unity3d.com/issues/crash-on-typecontainer-rtti-when-deleting-a-render-texture-that-is-used-by-the-main-camera))

- Input: Touch Input is not registered correctly when using multiple displays
    ([UUM-99077](https://issuetracker.unity3d.com/issues/touch-input-is-not-registered-correctly-when-using-multiple-displays))

- Lighting: Adaptive Probe Volumes are not applied to URP Simple Lit or Lit Shaders when using "Mixed" Light Mode
    ([UUM-98838](https://issuetracker.unity3d.com/issues/adaptive-probe-volumes-are-not-applied-to-urp-simple-lit-or-lit-shaders-when-using-mixed-light-mode))

- Raytracing: Crash on GfxDeviceD3D12::AllocBottomLevelAccelerationStructure when using Raytracing
    ([UUM-101163](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12-allocbottomlevelaccelerationstructure-when-using-raytracing))

- Serialization: Crash on MonoBehaviour::VirtualRedirectTransfer when closing Editor after removing HDRP and importing Water Samples before
    ([UUM-97847](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-virtualredirecttransfer-when-closing-editor-after-removing-hdpr-and-importing-water-samples-before))

- SRP XR: GPU utilization increases by 20% on Meta Quest headsets when Render Graph is enabled on 6000.0.16f1 and higher
    ([UUM-90118](https://issuetracker.unity3d.com/issues/gpu-utilization-increases-by-20-percent-on-meta-quest-headsets-when-render-graph-is-enabled-on-6000-dot-0-16f1-and-higher))

- SRP XR: The Player renders black on a Quest headset when MSAA, Post Processing, and Spacewarm depth submission are enabled
    ([UUM-84612](https://issuetracker.unity3d.com/issues/the-player-renders-black-on-a-quest-headset-when-msaa-post-processing-and-spacewarm-depth-submission-are-enabled))

- Vulkan: Editor crash on "(nvoglv64) vkGetInstanceProcAddr" when opening Prefab with Gizmos enabled in the Scene View
    ([UUM-99992](https://issuetracker.unity3d.com/issues/editor-crash-on-nvoglv64-vkgetinstanceprocaddr-when-opening-prefab-with-gizmos-enabled-in-the-scene-view))

- Vulkan: Standalone Player unresponsive/frozen in HDRP when built using Vulkan Graphics API on specific GPUs
    ([UUM-101692](https://issuetracker.unity3d.com/issues/standalone-player-unresponsive-slash-frozen-in-hdrp-when-built-using-vulkan-graphics-api-on-specific-gpus))

- Vulkan: [Android] [Vulkan] [UI Toolkit] Application crashes when the device is rotated when it has UI Toolkit TextField on Vulkan devices 
    ([UUM-100171](https://issuetracker.unity3d.com/issues/android-vulkan-ui-toolkit-application-crashes-when-the-device-is-rotated-when-it-has-ui-toolkit-textfield-on-vulkan-devices))



# 6000.0.45f1 Release Notes

## Features

- Package Manager: Added a version history entry for the registry version for installed packages that are Local/Git/Custom.



## Improvements

- Documentation: Added a fixed width to the body of the user manual so that the text doesn't overrun on large screens.

- GI: Added option to enable stitching lightmap shadowmask seams.



## Changes

- Package Manager: Change the default value of overrideBuiltins to prevent breaking user projects that override built-in packages during an upgrade.



## Fixes

- 2D: Fixed case Sprite Atlas samples show white textures in playmode when using late binding.
    ([UUM-100501](https://issuetracker.unity3d.com/issues/2d-sprite-atlas-samples-show-white-textures-in-playmode-when-using-late-binding))

- 2D: Fixed case where sprites are rendered improperly when SRP batcher is toggled off.
    ([UUM-99288](https://issuetracker.unity3d.com/issues/sprites-are-rendered-in-a-rounded-way-when-srp-batcher-is-toggled-off))

- 2D: Fixed rendering of bounds of grid in the TilePalette window.
    (UUM-99965)

- Android: Fixed an issue where objects would not render when using multiple overlay cameras with the OpenGL API on certain Adreno-GPU Android devices.
    ([UUM-98958](https://issuetracker.unity3d.com/issues/opengl-adreno-additional-overlay-cameras-do-not-render-world-objects-when-an-overlay-camera-is-rendering-a-canvas-in-the-player))

- Android: Fixed Integer input field now allowing negative integers to be entered.
    ([UUM-85618](https://issuetracker.unity3d.com/issues/android-the-symbol-is-not-allowed-to-be-entered-when-entering-a-negative-number-in-an-inputfield-when-the-content-type-is-set-to-integer-number))

- Android: Fixed multi-display support when using Android SurfaceViews as additional displays.
    (UUM-92490)

- Android: Switching to rendering some objects with MSAA and high quality settings during runtime could cause rendering issues or a black screen on certain older Android devices, this has been fixed.
    ([UUM-87091](https://issuetracker.unity3d.com/issues/android-application-either-crashes-renders-the-screen-black-or-doesnt-render-lit-gameobjects-when-switching-to-the-highest-quality-universal-render-pipeline-asset-during-runtime))

- Android: Update AGP to 8.72, Gradle to 8.11 and Command-Line Tools to 16.0

- Animation: Fixed blend node UI collapsing in the AnimatorController window when entering playmode.
    ([UUM-99052](https://issuetracker.unity3d.com/issues/the-blend-tree-node-is-artifacting-when-entering-play-mode-and-the-animator-window-is-open))

- Asset Pipeline: Fixed problem with main thread potentially being blocked, while doing async asset loads.
    ([UUM-95528](https://issuetracker.unity3d.com/issues/loading-animations-are-hitching-or-stopping-when-using-scenemanager-dot-loadsceneasync-to-load-new-scenes))

- Audio: Fixed an issue where playing an Audio Clip with non-zero reverb mix on an Audio Source could cause successive silent Audio Clip playbacks with the same codec settings to play reverberated, and more generally be capable of cloning any behaviour from previously pooled codecs.
    ([UUM-92689](https://issuetracker.unity3d.com/issues/audio-reverb-zone-still-produces-sound-when-the-audio-source-volume-is-0))

- Editor: Fixed a performance issue with user-provided or package-provided gizmo icons. Optimized gizmo icon rendering to significantly improve their performance in large scenes.
    ([UUM-97855](https://issuetracker.unity3d.com/issues/script-icon-gizmos-cause-lag-slash-performance-issues-in-scene-view-even-when-the-scene-camera-is-not-pointed-at-gizmos))

- Editor: Fixed an issue where changes to a prefab could be lost because the inspector would refresh when a curve/color/gradient editor window opened.
    ([UUM-99614](https://issuetracker.unity3d.com/issues/animation-curve-edits-are-not-always-saved-when-editing-in-a-prefab))

- Editor: Fixed an issue where the Occlusion Window active filter would be reset on domain reload.
    ([UUM-99535](https://issuetracker.unity3d.com/issues/scene-filter-buttons-reset-to-all-in-the-occlusion-window-when-entering-play-mode-but-the-scene-filters-themselves-do-not-reset))

- Editor: Fixed an issue where UIBuilder viewport doesn't reflect certain property changes.
    ([UUM-97052](https://issuetracker.unity3d.com/issues/text-outline-changes-dont-update-until-after-save-in-ui-builder))

- Editor: Fixed AssetDatabase.GetAssetBundleDependencies returned list doesn't include dependency when it's a Prefab Asset.
    ([UUM-83829](https://issuetracker.unity3d.com/issues/assetdatabase-dot-getassetbundledependencies-returned-list-doesnt-include-dependency-when-its-a-prefab-asset))

- Editor: Fixed Bold and Bold-Italic font weight for the editor font.
    (UUM-98978)

- Editor: Fixed build profile player settings changed through APIs not saved when using AssetDatabase.SaveAssets\(\).
    (UUM-90038)

- Editor: Fixed documentation for box light support in RT.
    (UUM-100900)

- Editor: Fixed GradientPicker removing all swatches when dragging them outside.
    ([UUM-100664](https://issuetracker.unity3d.com/issues/all-newly-created-color-markers-of-gradient-editor-get-removed-at-once-when-trying-to-remove-one-of-them))

- Editor: Fixed red spots appearing when using blending scenarios with APV.
    ([UUM-92338](https://issuetracker.unity3d.com/issues/red-spots-appear-when-blending-lighting-scenarios-using-adaptive-probe-volumes))

- Editor: Fixed skin-mesh shadow cascade culling.
    ([UUM-98273](https://issuetracker.unity3d.com/issues/shadow-cascade-culling-does-not-work-when-used-with-skinned-mesh-renderer-in-urp))

- Editor: Fixed the `EditorStyles.whiteBoldLabel` style so the text is white.
    ([UUM-84114](https://issuetracker.unity3d.com/issues/editorguilayout-dot-labelfield-displays-black-text-when-the-editorstyles-dot-whiteboldlabel-parameter-is-passed-in))

- Editor: Fixed UseDebugLibraries for GameCore visual studio debug projects.
    (UUM-95514)

- Editor: \[APV\] Impossible to switch between multiple Baking Set when multiple scenes are loaded additively.
    ([UUM-85396](https://issuetracker.unity3d.com/issues/apv-impossible-to-switch-between-multiple-baking-set-when-multiple-scenes-are-loaded-additively))

- GI: Fixed an issue where Adaptive Probe Volumes could not be loaded from Asset Bundles.
    ([UUM-90705](https://issuetracker.unity3d.com/issues/adaptive-probe-volumes-are-not-loaded-when-adaptive-light-probes-are-exported-via-asset-bundles-and-opened-on-another-project))

- Graphics: Fixed potential race condition when calling GraphicsBuffer.SetData and GraphicsBuffer.LockBufferForWrite/GraphicsBuffer.UnlockBufferAfterWrite.
    ([UUM-83339](https://issuetracker.unity3d.com/issues/calling-beginwrite-before-endwrite-errors-logged-in-the-console-window-of-a-macos-editor-when-in-play-mode))

- Graphics: Fixed the artifacts of Volumetric Clouds on certain platforms.
    (UUM-87074)

- HDRP: Fixed a shader compilation error of HDRP Lit Shader if UV mapping for Emissive Map is set to "Same as Base".
    ([UUM-100070](https://issuetracker.unity3d.com/issues/hdrp-lit-shader-errors-are-thrown-and-artifacts-are-generated-when-using-emissive-map-and-same-as-base-uv-mapping-setting))

- HDRP: Fixed bad Reflection Probe rendering of Volumetric Clouds in HDRP.
    ([UUM-84729](https://issuetracker.unity3d.com/issues/baked-reflection-color-of-clouds-does-not-match-the-scene-sky-color-when-generating-lighting-in-unity))

- iOS: Fixed soft keyboard Done/Cancel buttons truncating \(to "..."\) in languages like Korean due to decimal font width.
    ([UUM-97527](https://issuetracker.unity3d.com/issues/ios-hwagin-done-and-cwiso-cancel-text-is-displayed-as-dot-dot-dot-in-the-on-screen-keyboard-when-the-system-preferred-language-is-set-to-korean))

- Scene/Game View: Fixed an issue where the CameraOverlay render texture would throw errors in the console.
    ([UUM-100338](https://issuetracker.unity3d.com/issues/scene-view-has-an-inverted-game-view-window-when-changing-from-game-view-to-scene-view-on-a-specific-project))

- Terrain: Terrain Trees with custom Tree Height and any materials without a "_TreeInstanceScale" property return to their correct height when zoomed in. Prior to this fix, trees materials without _TreeInstanceScale would always render at scale 1, even if the tree instance had height data.
    ([UUM-40370](https://issuetracker.unity3d.com/issues/terrain-trees-with-custom-tree-height-return-to-their-default-height-when-zoomed-in))

- Text: Fixed an issue to ensure default editor fontAssets are properly initialized.
    (UUM-98848)

- Text: Fixed an issue to ensure the SamplingPoint size for color font are set properly.
    (UUM-71284)

- UI Toolkit: Added missing high dpi icons for HelpBox.
    (UUM-48260)

- UI Toolkit: Fixed an issue with the final item of a ListView hiding at high display scales when another item was moved.
    ([UUM-81516](https://issuetracker.unity3d.com/issues/element-disappears-from-a-list-after-its-reordered-when-a-high-display-resolution-and-a-250-percent-display-scale-is-used))

- UI Toolkit: Fixed drag and moving an item from one index to another index outside of the viewport.
    (UUM-98986)

- UI Toolkit: Fixed element being drag and dropped after opened context menu in the UI Builder hierarchy view.
    (UUM-69261)

- UI Toolkit: Fixed expressions for serialized properties in numeric fields.
    ([UUM-82983](https://issuetracker.unity3d.com/issues/numeric-field-expressions-do-not-provide-correct-results-when-used-in-a-public-float-field-in-the-inspector))

- UI Toolkit: Fixed TextFields blocking the KeyDownEvents for shortcuts.
    (UUM-76370)

- UI Toolkit: Workaround for focus-follow-mouse not supported on MacOS to allow single click picking in UI Toolkit Debugger.
    ([UUM-100383](https://issuetracker.unity3d.com/issues/ui-toolkit-debugger-pick-element-selection-works-only-after-clicking-it-for-the-second-time))

- URP: Fixed the shadow jittering issue with TAA in deferred pass on URP scenes.
    ([UUM-97957](https://issuetracker.unity3d.com/issues/shadow-is-jittering-when-taa-is-on-lens-shift-is-enabled-and-the-camera-is-at-least-800-units-away-from-the-origin))

- VFX Graph: Fixed exception when converting a selection that contains an empty group to a subgraph.
    ([UUM-97951](https://issuetracker.unity3d.com/issues/converting-empty-groups-along-with-nodes-into-a-subgraph-prevents-subgraph-creation-and-throws-errors))

- VFX Graph: Fixed messy expand/collapse icon when zoomed in.
    ([UUM-95343](https://issuetracker.unity3d.com/issues/visual-effects-graph-node-expansion-icon-is-corrupted))

- VFX Graph: Update documentation to remove mention of VFXFIXED_RAND macro which is not supported in custom hlsl nodes
    ([UUM-83777](https://issuetracker.unity3d.com/issues/vfx-graph-hlsl-vfxfixed-rand-isnt-working))

- Web: Fixed an issue where loading Entities content on the Web platform might fail with an error "Loading Entity Scene failed because the entity header file couldn't be resolved".
    (UUM-98767)

- Windows: Fixed this issue by reverting original PR that cause the regression, related to losing focus on windows player during startup.
    ([UUM-100910](https://issuetracker.unity3d.com/issues/the-windows-built-project-fails-to-load-or-run-when-using-the-fullscreen-window-or-windowed-build-resolution-options))

- Windows: Fixed Windows player crashing when embedded into an executable that does not export the D3D12SDKPath symbol.
    ([UUM-96170](https://issuetracker.unity3d.com/issues/windows-player-with-a-custom-exe-file-crashes-in-fixupd3d12sdkpath))




## Package changes in 6000.0.45f1

## Packages updated

- com.unity.addressables: [2.3.16](https://docs.unity3d.com/Packages/com.unity.addressables@2.3//changelog/CHANGELOG.html) to [2.4.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.4//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.13.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.13//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.14//changelog/CHANGELOG.html)

- com.unity.probuilder: [6.0.4](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html) to [6.0.5](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html)

- com.unity.services.authentication: [3.4.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.4//changelog/CHANGELOG.html) to [3.4.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.4//changelog/CHANGELOG.html)

- com.unity.splines: [2.7.2](https://docs.unity3d.com/Packages/com.unity.splines@2.7//changelog/CHANGELOG.html) to [2.8.0](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)