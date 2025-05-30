# Unity 6000.0.26f1 LTS
Published at Thu, 07 Nov 2024 03:58:16 GMT  
https://unity.com/releases/editor/whats-new/6000.0.26

# Known Issues in 6000.0.26f1

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- Graphics Device Features: [Quest] Editor crashes on toggleFoveation when activating SRP Foveated Rendering in DX12
    ([UUM-85208](https://issuetracker.unity3d.com/issues/quest-editor-crashes-on-togglefoveation-when-activating-srp-foveated-rendering-in-dx12))

- HDRP: Graphics Compositor breaks Unity rendering when the "Output Camera" is changed to a scene Camera and one Camera SubLayer is active.<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84610

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Scripting Runtime: Crash on tlsf_free when exiting Play Mode in a specific project
    ([UUM-86106](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-exiting-play-mode-in-a-specific-project))

- Shader System: Editor crash when saving Currently Tracked Variants to Asset
    ([UUM-86510](https://issuetracker.unity3d.com/issues/editor-crash-when-saving-currently-tracked-variants-to-asset))

- Shader System: Shaders are always recompiled when the Editor is opened
    ([UUM-75262](https://issuetracker.unity3d.com/issues/shaders-are-always-recompiled-when-the-editor-is-opened))

- SpeedTree: This release of SpeedTree includes a change to the interface of the SpeedTree8Wind shadergraph node. If you have an animated SpeedTree in the shadergraph, be sure to connect an ObjectSpacePosition node to the input of the SpeedTree8Wind.  If the wind node does not have an input on the ObjectSpacePosition port, the mesh will be shrunk down to a point at origin \(making it seem to vanish\).<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84616

- Vulkan: [Android] Particles not rendered in the Player on some Android devices with Android 14
    ([UUM-68080](https://issuetracker.unity3d.com/issues/android-particles-not-rendered-in-the-player-on-some-android-devices-with-android-14))



# 6000.0.26f1 Release Notes

## Improvements

- Scripting: Now Logs an error message and exit the Editor instead of crashing if SynchronizationContext is set to anything other than UnitySynchronizationContext.



## Fixes

- Audio: Fixed error in in editor window for the AudioRandomContainer asset when undoing removal of an list element that was done in play mode after going back to edit mode.
    ([UUM-55847](https://issuetracker.unity3d.com/issues/error-arc-audio-clip-entry-reference-is-lost-when-undoing-edits-made-in-play-mode))

- Editor: Added additional check to GraphicsSettings if URP or HDRP asset is a missing type.
    ([UUM-79997](https://issuetracker.unity3d.com/issues/a-nullreferenceexception-error-is-thrown-when-trying-to-add-tags-and-layers-when-urp-settings-are-present-in-the-project-with-a-broken-universalrp-asset))

- Editor: Do not accumulate vertical/horizontal scroll deltas for IMGUI events being triggered from native code.
    (UUM-79079)

- Editor: Fixed a crash caused by a \(rare\) failure to initialize NetworkListManager COM interface.
    (UUM-83823)

- Editor: Fixed an issue  that tree wireframe is incorrectly rendered outside of Scene view when editing a tree.
    ([UUM-82833](https://issuetracker.unity3d.com/issues/branch-editing-tools-draw-flashing-lines-with-black-backgrounds-in-editor-ui-windows))

- Editor: Fixed console logs not being cleared on recompile if Clear on Recompile option was enabled.
    ([UUM-73031](https://issuetracker.unity3d.com/issues/the-console-window-is-not-cleared-when-scripts-are-recompiled-and-the-clear-on-recompile-option-is-enabled))

- Editor: Fixed memory leak in Texture2D.CreateExternalTexture when using D3D11 platform.
    ([UUM-77354](https://issuetracker.unity3d.com/issues/memory-leak-in-texture2d-dot-createexternaltexture-when-using-d3d11-platform))

- Editor: Fixed text not being updated after changing some FontAsset's values.
    (UUM-82887)

- Editor: Fixed the version string in the about box of the editor.
    ([UUM-85505](https://issuetracker.unity3d.com/issues/about-unity-window-shows-extended-version-numbers-including-staging-tag))

- Editor: Fixed warning message occurring when Focusing a text just after enabling a UIDocument.
    ([UUM-83856](https://issuetracker.unity3d.com/issues/cant-generate-mesh-no-font-asset-has-been-assigned-warning-is-thrown-when-setting-focus-to-a-visual-element))

- Graphics: Fixed GPUResidentDrawer crash in ParallelSortExtensions.ParallelSort because of an array being diposed while still used by some jobs.
    ([UUM-83578](https://issuetracker.unity3d.com/issues/crash-in-parallelsortextensions-parallelsort))

- Graphics: Fixed GPUResidentDrawer deadlock because of a double dispose of CPUSharedInstanceData.materialIDArrays.
    (UUM-83561)

- Graphics: Fixed GPUResidentDrawer Editor crash on Metal when occluderDepthPyramidKernels compute shader import fails.
    (UUM-84509)

- Input System: Fixed an internal Unity issue that could cause the Input System package to stop processing data from devices.
    ([UUM-85315](https://issuetracker.unity3d.com/issues/input-is-not-received-after-some-time-when-using-a-gamepad))

- iOS: Fixed the character limit of the keyboard shown with TouchScreenKeyboard.Open.
    ([UUM-77509](https://issuetracker.unity3d.com/issues/ios-touchscreenkeyboard-allows-an-extra-character-when-characterlimit-is-set))

- Package Manager: Fixed an issue where incorrect registry info is shown for packages that do not belong to any registry.
    (UUM-84168)

- Package Manager: Fixed NullException thrown in a multi page wizard import when clicking on the previous button.
    (UUM-82611)

- Package Manager: Users can now import without having to choose a project setting with at least one asset previously selected.
    (UUM-82612)

- Physics: Fixed an issue where vehicle data would not be preserved when adding multiple WheelCollider components using the GameObject scripting APIs.
    ([UUM-85527](https://issuetracker.unity3d.com/issues/colliders-of-gameobject-with-rigidbody-component-fail-to-collide-with-another-gameobject-when-rigidbody-becomes-kinematic))

- Shadergraph: Fixed an issue where the Main Light Direction node always returned 0 on the built-in render pipeline.
    ([UUM-78803](https://issuetracker.unity3d.com/issues/the-main-light-direction-node-in-the-shader-graph-does-not-output-light-direction-for-directional-light-when-used-with-the-built-in-render-pipeline))

- Shadergraph: Fixed an issue where Unity pragmas were not used in files included by the Custom Function Node, and added a "Use Pragmas" toggle to enable/disable them as needed.
    (UUM-78849)

- Shaders: Fixed rare occasions of objects batching together incorrectly.
    (UUM-35593)

- Text: Fixed issue where the text cache would continue to refer to a cleared font asset.
    ([UUM-79381](https://issuetracker.unity3d.com/issues/the-fallback-source-continues-to-refer-to-the-clearfontassetdataed-glyph-after-clearfontassetdata-is-applied))

- Text: Fixed out of range issue when dragging on a empty field.
    ([UUM-79222](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-continuously-clicking-the-textfield-and-dragging))

- TextCore: Fixed thread issue when using CJK text.
    ([UUM-78458](https://issuetracker.unity3d.com/issues/unityexception-get-bytes-can-only-be-called-from-the-main-thread-dot-error-is-thrown-when-asset-name-contains-chinese-characters))

- TextMeshPro: Fixed color picker not being the same color as the Text in the scene.
    ([UUM-77652](https://issuetracker.unity3d.com/issues/the-color-in-the-inspector-is-different-than-the-gameobject-in-the-scene-when-changing-the-material-face-color))

- TextMeshPro: Fixed the broken URL of the help button on the TextMesh Pro Settings page.
    ([UUM-74086](https://issuetracker.unity3d.com/issues/sorry-dot-dot-dot-that-page-seems-to-be-missing-is-a-result-when-user-clicks-on-textmesh-pro-settings-help-icon))

- UI Toolkit: Fixed null-ref exception when converting the UXML preview window into floating mode.
    (UUM-85493)

- Universal RP: Fixed a redundant empty line in a tooltip for Cast Shadows toggle in the URP Asset for Additional lights.
    ([UUM-83534](https://issuetracker.unity3d.com/issues/redundant-empty-space-on-tooltip-for-cast-shadows-option-for-additional-lights))

- Universal RP: Fixed an issue where WorldToCamera matrix wasn't set before rendering shadows.
    ([UUM-84287](https://issuetracker.unity3d.com/issues/gameobjects-shadows-affected-by-custom-shaders-change-their-scale-and-position-when-the-scene-camera-is-adjusted))

- Universal RP: Fixed issue with spot light clipping incorrectly in URP Forward+.
    ([UUM-85566](https://issuetracker.unity3d.com/issues/spot-light-with-high-outer-spot-angle-produces-artefacts-slash-clipping-when-using-the-forward-plus-rendering-path))

- Universal RP: Fixed spamming errors and broken visual when resizing GameView with Free Aspect in DepthBlit sample.
    ([UUM-84029](https://issuetracker.unity3d.com/issues/scene-slash-game-view-visually-breaks-and-console-is-spammed-with-errors-when-using-depthblit-sample-scene))

- URP: Remove 'implicit truncation of vector type' warnings at URP ScreenSpaceAmbientOcclusion.shader.
    ([UUM-79253](https://issuetracker.unity3d.com/issues/warnings-are-thrown-after-building-universal-3d-sample-template))

- VisionOS: OnApplicationFocus\(false\) is now called when a visionOS app in Metal app mode is sent to the background.
    ([AVPB-443](https://issuetracker.unity3d.com/issues/onapplicationfocus-isnt-called-when-the-application-goes-in-or-out-of-focus))




## Package changes in 6000.0.26f1

## Packages updated

- com.unity.2d.animation: [10.1.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.1//changelog/CHANGELOG.html) to [10.1.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.1//changelog/CHANGELOG.html)

- com.unity.2d.common: [9.0.6](https://docs.unity3d.com/Packages/com.unity.2d.common@9.0//changelog/CHANGELOG.html) to [9.0.7](https://docs.unity3d.com/Packages/com.unity.2d.common@9.0//changelog/CHANGELOG.html)

- com.unity.2d.spriteshape: [10.0.6](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html) to [10.0.7](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html)

- com.unity.2d.tilemap.extras: [4.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.0//changelog/CHANGELOG.html) to [4.1.0](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html)

- com.unity.cinemachine: [2.10.1](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) to [2.10.2](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.mobile.notifications: [2.3.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.3//changelog/CHANGELOG.html) to [2.4.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- com.unity.toolchain.linux-x86_64: [2.0.9](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.10](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.toolchain.macos-x86_64-linux-x86_64: [2.0.9](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.10](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.toolchain.macos-arm64-linux-x86_64: [2.0.3](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-arm64-linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.4](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-arm64-linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.toolchain.win-x86_64-linux-x86_64: [2.0.9](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html) to [2.0.10](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux-x86_64@2.0//changelog/CHANGELOG.html)

- com.unity.toolchain.win-arm64-linux-x86_64: [1.0.3](https://docs.unity3d.com/Packages/com.unity.toolchain.win-arm64-linux-x86_64@1.0//changelog/CHANGELOG.html) to [1.0.4](https://docs.unity3d.com/Packages/com.unity.toolchain.win-arm64-linux-x86_64@1.0//changelog/CHANGELOG.html)