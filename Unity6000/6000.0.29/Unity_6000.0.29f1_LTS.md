# Unity 6000.0.29f1 LTS
Published at Thu, 28 Nov 2024 09:51:13 GMT  
https://unity.com/releases/editor/whats-new/6000.0.29

# Known Issues in 6000.0.29f1

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- DirectX12: Allocated graphics memory does not get released when the Editor is out of focus while using D3D12 graphics API
    ([UUM-86354](https://issuetracker.unity3d.com/issues/allocated-graphics-memory-does-not-get-released-when-the-editor-is-out-of-focus-while-using-d3d12-graphics-api))

- DirectX12: The Camera does not render correctly when the Camera.Rect() is changed and HDR is enabled and DX12 graphics API is selected
    ([UUM-86917](https://issuetracker.unity3d.com/issues/the-camera-does-not-render-correctly-when-the-camera-dot-rect-is-changed-and-hdr-is-enabled-and-dx12-graphics-api-is-selected))

- Graphics Device Features: [Quest] Editor crashes on toggleFoveation when activating SRP Foveated Rendering in DX12
    ([UUM-85208](https://issuetracker.unity3d.com/issues/quest-editor-crashes-on-togglefoveation-when-activating-srp-foveated-rendering-in-dx12))

- HDRP: Graphics Compositor breaks Unity rendering when the "Output Camera" is changed to a scene Camera and one Camera SubLayer is active.<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84610

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Mono: [Silicon] Crash on Bytenado.Chatterbox:.ctor when opening a project after creating a partial class of a Dictionary<string,  int> containing about 125k entries
    ([UUM-87488](https://issuetracker.unity3d.com/issues/silicon-crash-on-bytenado-dot-chatterbox-dot-ctor-when-opening-a-project-after-creating-a-partial-class-of-a-dictionary-string-int-containing-about-125k-entries))

- Optimization: Average FPS in Play Mode degradation on a newly created BiRP project when it's upgraded from 2020.3.48f1 to a newer Editor version
    ([UUM-89979](https://issuetracker.unity3d.com/issues/average-fps-in-play-mode-degradation-on-a-newly-created-birp-project-when-its-upgraded-from-2020-dot-3-48f1-to-a-newer-editor-version))

- Scene Management: [MacOS] Crash on [NSApplication endModalSession:] when saving while Play Mode is loading
    ([UUM-87930](https://issuetracker.unity3d.com/issues/macos-crash-on-nsapplication-endmodalsession-when-saving-while-play-mode-is-loading))

- SpeedTree: This release of SpeedTree includes a change to the interface of the SpeedTree8Wind shadergraph node. If you have an animated SpeedTree in the shadergraph, be sure to connect an ObjectSpacePosition node to the input of the SpeedTree8Wind.  If the wind node does not have an input on the ObjectSpacePosition port, the mesh will be shrunk down to a point at origin \(making it seem to vanish\).<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84616

- Terrain: Trees do not render in 'Unity Terrain - URP Demo Scene'
    ([UUM-84616](https://issuetracker.unity3d.com/issues/trees-do-not-render-in-unity-terrain-urp-demo-scene))

- Vulkan: [Android] Particles not rendered in the Player on some Android devices with Android 14
    ([UUM-68080](https://issuetracker.unity3d.com/issues/android-particles-not-rendered-in-the-player-on-some-android-devices-with-android-14))



# 6000.0.29f1 Release Notes

## Improvements

- Editor: Added array slice and mipmap info  to the render graph debugger.

- Editor: Added extra validation to the render graph texture descriptor to avoid silently failing when a user tried to create  an invalid texture.

- Editor: Improved material creation for PBR Sky custom material.
    (UUM-86718)



## Fixes

- 2D: Fixed issue where Tile Palette windows does not automatically show changes for the Tile Palette when the user changes the Tile Palette's cell swizzle properties.
    (UUM-86005)

- Accessibility: Fixed text overflow when resizing Accessibility Hierarchy Viewer Inspector pane.
    ([UUM-82909](https://issuetracker.unity3d.com/issues/text-on-inspector-pane-in-hierarchy-viewer-overflows-into-hierarchy-pane))

- Android: Enabled PBG video test on GameActivity after fix.
    (UUM-87630)

- Android: Fixed FrameTimings calculation on Android when using OpenGLES graphics.
    (UUM-87325)

- Animation: Fixed calls to AnimationUtility.GetEditorCurve leaking memory in c\#.
    (UUM-87015)

- Asset Pipeline: Fixed a crash when changing the extension for plugins and scripts.
    ([UUM-83233](https://issuetracker.unity3d.com/issues/freeze-slash-crash-on-hash128tostring-when-opening-project-with-google-dot-iosresolver-dot-dll-renamed-to-google-dot-iosresolver-dot-dll-dot-removed))

- Cache Server: Fixed the crash while importing the Assets from Accelerator when it is disconnected.
    (UUM-76355)

- Editor: Crash on mdb_txn_begin when activating any of the Virtual Players.
    ([UUM-87484](https://issuetracker.unity3d.com/issues/crash-on-mdb-txn-begin-when-activating-any-of-the-virtual-players))

- Editor: Fixed an incorrect label for the culling mask in the built-in render pipeline's camera inspector.
    (UUM-87404)

- Editor: Fixed assertion asserts being spammed in the console when Maximum Reflection Probe count is higher than 64 \(HDRP\).
    ([UUM-86779](https://issuetracker.unity3d.com/issues/hdrp-assertion-printed-when-maximum-reflection-probe-count-is-higher-than-64-due-to-k-maxcubereflectionsonscreen-when-raytracing-is-enabled))

- Editor: Fixed bug  where toggling the Incremental GC or active input handling player settings and then restarting the editor didn't result in the new setting taking effect.
    (UUM-85422)

- Editor: Fixed build profile bugs when toggling the virtual texturing setting:<br>
    1. Updating the player setting value didn't get serialized to the asset file.<br>
    2. Toggling the virtual texture player setting for an inactive profile still showed the restart editor prompt.<br>
    3. Even after restarting the editor, we didn't update EditorOnlyVirtualTextureState.json that the PlayerSetting methods used as the source of truth for the setting, which resulted in a subsequent restart prompt appearing as the project was opening after the initial restart.
    (UUM-77905)

- Editor: Fixed Editor errors when "RGB + 1-bit Alpha Compressed ETC2 4 bits" compression is used.
    ([UUM-65395](https://issuetracker.unity3d.com/issues/editor-crashes-on-libetc-init-when-changing-webgl-texture-format-to-rgb-plus-1-bit-alpha-compressed-etc2-4-bits))

- Editor: Fixed for Linux crash on right click in the middle of a window drag.
    ([UUM-82814](https://issuetracker.unity3d.com/issues/linux-crash-on-containerwindow-togglemaximize-when-clicking-rmb-while-moving-window-inside-the-editor))

- Editor: Fixed Inter not being created at runtime.
    ([UUM-79518](https://issuetracker.unity3d.com/issues/ui-is-not-visible-when-displayed-in-runtime))

- Editor: Fixed issue where Scene View navigation would not function properly when using a pen tablet as the input device.
    ([UUM-77768](https://issuetracker.unity3d.com/issues/macos-scene-view-is-not-rotating-when-pressing-the-binded-rmb-button-on-a-drawing-tablet-and-moving-the-drawing-pen))

- Editor: Fixed null ref exception when trying to maximize a pop-up window.
    ([UUM-76218](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-trying-to-maximize-view-in-anchor-presets-menu))

- Editor: Fixed some settings Asset icons that were missing in the selection window.
    ([UUM-83464](https://issuetracker.unity3d.com/issues/lighting-settings-asset-icon-is-missing-in-the-selection-window))

- Editor: The Linux editor will now reduce CPU usage when moved to the background, respecting the "Interaction Mode" setting.
    ([UUM-79514](https://issuetracker.unity3d.com/issues/linux-high-cpu-usage-when-editor-interaction-mode-is-set-to-no-throttling))

- Graphics: Fixed an issue where STP is disabled if TAA is disabled.
    ([UUM-87121](https://issuetracker.unity3d.com/issues/game-view-fails-to-render-when-cameras-are-stacked-and-stp-is-enabled))

- Graphics: Fixed msaa resolves of SetRenderTarget-based rending not being done before beginning a new renderpass.
    ([UUM-72239](https://issuetracker.unity3d.com/issues/fullscreen-blit-is-not-working-when-render-graph-is-enabled))

- Graphics: Fixed picking and outline for all BatchRendererGroup draw types.
    (UUM-87382)

- Graphics: The Render pass API was sometimes erroneously considering a configuration that was valid as invalid when rendering to array slices or mipmaps.

- HDRP: Fixed to avoid calling the Cleanup method twice so the celestial data remains.
    ([UUM-83616](https://issuetracker.unity3d.com/issues/hdrp-empty-template-starts-with-incorrect-physically-based-sky-ground))

- iOS: Fixed plugin framework folders showing up red in exported iOS Xcode project.
    (UUM-84687)

- Kernel: Fixed a hang that would occur when accessing transforms immediately after scheduling a transform job with dependencies.
    ([UUM-86782](https://issuetracker.unity3d.com/issues/the-editor-freezes-when-schedulereadonly-of-ijobparallelfortransform-with-dependency-is-used))

- Mono: Fixed crash when loading a class which contains fields at the end of the metadata table with a table size 65535.
    ([UUM-78961](https://issuetracker.unity3d.com/issues/crash-on-mono-class-setup-basic-field-info-when-opening-a-project))

- Mono: Fixed rare NullReferenceException during a constrained call on a value type.
    ([UUM-79115](https://issuetracker.unity3d.com/issues/unity-mono-release-mode-jit-causes-an-error-when-using-a-memorymappedfile))

- Package Manager: Fixed the issue where quick start button does not link to the document page for the current unity version.
    ([UUM-78210](https://issuetracker.unity3d.com/issues/quickstart-buttons-for-unity-registry-feature-sets-links-to-outdated-documentation))

- Package Manager: Fixed the issue where update available filter doesn't refresh list properly sometimes.
    (UUM-85700)

- Package Manager: Fixed the issue where `Experimental Package in Use`  dropdown button not selecting the correct page in the Package Manager.
    (UUM-85699)

- Profiler: Fixed an issue in the Profiler Timeline view where the 'Show' dropdown would lead to the incorrect views.
    (UUM-83138)

- Scripting: Fixed false positives of warning CS8602 when user code is compiled with nullability checks and implicit converter from UnityEngine.Object to bool is used.
    (UUM-87634)

- Shaders: Fixed a rare error involving incompatible keyword states.
    (UUM-87539)

- Shaders: Fixed an issue where SHADER_TARGET macro was not available during shader import.
    ([UUM-87423](https://issuetracker.unity3d.com/issues/editing-the-unitydotsinstancing-dot-hlsl-file-does-not-cause-a-shader-recompilation))

- SpeedTree: Crash in SpeedTreeWindManager with certain prefab assets when play mode is engaged.
    ([UUM-85328](https://issuetracker.unity3d.com/issues/crash-on-anonymous-namespace-preparetreesandwritewindparamsjobdata-execute-when-entering-play-mode-on-a-specific-project-1))

- SpeedTree: Fixed an issue where undo was not possible when the branch was rotated.
    ([UUM-82599](https://issuetracker.unity3d.com/issues/branch-rotation-cant-be-undone))

- SpeedTree: Importer error for .st files when there are special characters in the file path.
    ([UUM-83783](https://issuetracker.unity3d.com/issues/speedtree-importer-fails-to-import-st-files-when-path-to-the-project-includes-a-special-character))

- SRP Core: Fixed render graph incorrectly handling rendering to array slices and mipmaps other than 0 in some cases.
    (UUM-77828)

- Text: Enabled OSFontFallbacks for ATG.
    (UUM-78505)

- Text: Removed the need for the ICU data to be in the user's project.
    (UUM-86054)

- TextCore: Ensure we only clear FontAssets that are initialized.
    ([UUM-82370](https://issuetracker.unity3d.com/issues/tmp-fontasset-dot-clearatlastextures-set-the-size-of-atlases-to-1x1-when-setatlassizetozero-is-true-resulting-in-a-constant-clearing-of-atlases-of-size-1x1-on-editor-shutdown))

- TextMeshPro: Avoid creating a new submesh if the previous one still has space.
    ([UUM-76335](https://issuetracker.unity3d.com/issues/a-lot-of-submesh-children-are-created-when-a-specific-text-is-displayed))

- TextMeshPro: Fixed TMP crash on Hyphen wrapping.
    ([UUM-84379](https://issuetracker.unity3d.com/issues/editor-hangs-when-rendering-tmp-text-component-with-left-and-right-margins-set-in-the-extra-settings))

- UI Toolkit: Fixed a bug in the UI Builder where it would always delete the first selector with the same value.
    (UUM-87169)

- UI Toolkit: Fixed an issue where data sources could remain cached after an element was removed from the panel.
    (UUM-87201)

- UI Toolkit: Fixed PointerOutEvent sent too many times on the same element when clicking on it and then elsewhere using Touch.
    ([UUM-54208](https://issuetracker.unity3d.com/issues/pointeroutevent-is-not-being-called-after-pressing-the-first-button-on-the-touchscreen-when-the-first-button-exchanges-places-with-a-second-button-leaving-the-second-button-in-a-hover-state))

- Universal RP: Fixed an issue where Transparent Receive Shadows setting didn't work for custom shaders.
    ([UUM-79471](https://issuetracker.unity3d.com/issues/main-light-shadows-are-shown-on-transparent-material-when-the-transparent-receive-shadows-parameter-is-disabled))

- Universal RP: Fixed depth texture format used for URP 2D RenderPass with Android devices.
    (UUM-86791)

- VFX Graph: Subgraph blocks now accept correct types of block based on their suitable context.
    ([UUM-83521](https://issuetracker.unity3d.com/issues/vfx-graph-subgraph-nesting-isnt-functionnal))

- Video: Fixed Video with transparency having artifacts on the border of the sprite.
    ([UUM-74644](https://issuetracker.unity3d.com/issues/android-artifacts-in-video-file-on-android-player))

- WebGL: \[WebGPU\] Fix SubPass rendering due to incorrect viewport.

- XR: Updated XR Interaction Toolkit \(com.unity.xr.interaction.toolkit\) to 3.0.7.




## Package changes in 6000.0.29f1

## Packages updated

- com.unity.sentis: [2.1.0](https://docs.unity3d.com/Packages/com.unity.sentis@2.1//changelog/CHANGELOG.html) to [2.1.1](https://docs.unity3d.com/Packages/com.unity.sentis@2.1//changelog/CHANGELOG.html)

- com.unity.services.leaderboards: [2.1.0](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.1//changelog/CHANGELOG.html) to [2.2.0](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.2//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [3.0.5](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html) to [3.0.7](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html)

- com.unity.learn.iet-framework: [4.0.2](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@4.0//changelog/CHANGELOG.html) to [4.0.3](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@4.0//changelog/CHANGELOG.html)

- com.unity.ai.navigation: [2.0.4](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) to [2.0.5](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)