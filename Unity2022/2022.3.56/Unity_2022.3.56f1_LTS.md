# Unity 2022.3.56f1 LTS
Published at Wed, 15 Jan 2025 07:37:15 GMT  
https://unity.com/releases/editor/whats-new/2022.3.56

# Known Issues in 2022.3.56f1

- Audio Authoring: Audio Source clip is not audible when exceeding a high number of active Audio Sources
    ([UUM-91256](https://issuetracker.unity3d.com/issues/audio-source-clip-is-not-audible-when-exceeding-a-high-number-of-active-audio-sources))

- DirectX12: Allocated graphics memory does not get released when the Editor is out of focus while using D3D12 graphics API
    ([UUM-86354](https://issuetracker.unity3d.com/issues/allocated-graphics-memory-does-not-get-released-when-the-editor-is-out-of-focus-while-using-d3d12-graphics-api))

- DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when opening a project after changing the Graphics API to DirectX12
    ([UUM-77757](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-opening-a-project-after-changing-the-graphics-api-to-directx12))

- DirectX12: The Camera does not render correctly when the Camera.Rect() is changed and HDR is enabled and DX12 graphics API is selected
    ([UUM-86917](https://issuetracker.unity3d.com/issues/the-camera-does-not-render-correctly-when-the-camera-dot-rect-is-changed-and-hdr-is-enabled-and-dx12-graphics-api-is-selected))

- Serialization: [windows only] Switching Project when importing complete project does not import all assets and project opens incomplete
    ([UUM-88051](https://issuetracker.unity3d.com/issues/switching-project-when-importing-complete-project-does-not-import-all-assets-and-project-opens-incomplete))



# 2022.3.56f1 Release Notes

## Fixes

- Android: Added support for 16KB page sizes.

- Android: Android: Added dotnet webrequest feature for auto internet access permission.
    ([UUM-83355](https://issuetracker.unity3d.com/issues/android-error-nameresolutionfailure-when-internet-access-is-set-to-auto))

- Android: Bump Android Logcat Package to 1.4.4.

- Asset Bundles: Added a new flag BuildAssetBundleOptions.StripUnatlasedSpriteCopies to the legacy asset bundle system. Currently if we have a assets in multiple bundles that depend upon a source texture we copy it into all relevant bundles. Setting this new flag will keep from creating duplicates if the texture does not belong to a sprite atlas.
    ([UUM-83067](https://issuetracker.unity3d.com/issues/asset-instance-duplicates-when-there-is-no-dependency-duplication-between-asset-bundles))

- Audio: Fixed the 3D audio pan where right audio channel is completely cutoff at specific position.
    ([UUM-82903](https://issuetracker.unity3d.com/issues/the-right-audio-channel-completely-cuts-out-in-a-specific-position-with-the-3d-audio-when-the-audio-should-be-playing-from-both-speaker-in-that-position))

- Audio: Reenabled an unstable test.
    (UUM-346)

- Editor: Asset Import: Fixed FBX import errors when importing models using the IndexToDirect format for normals.
    (UUM-74806)

- Editor: Dont output compile errors when we automatically will retry the compilation, as they will be rerun and potentially fixed.
    (UUM-72688)

- Editor: Editor crash in the HDRP samples.
    (UUM-91532)

- Editor: Editor no longer crashes if a tooltip pops up prior to clicking to show a dropdown menu.
    ([UUM-89006](https://issuetracker.unity3d.com/issues/crash-on-showdelayedcontextmenu-bool-when-changing-the-size-options-of-a-visual-element-in-the-uitoolkit-inspector))

- Editor: Fixed a crash is some Linux configurations where a notification from X11 can be raised before the application is initialized.
    ([UUM-91116](https://issuetracker.unity3d.com/issues/linux-crash-on-application-handleeditorfocuschange-when-opening-a-project-in-specific-environments))

- Editor: Fixed an issue where the editor could occasionally crash when exiting the editor with the Input System package included and the Active Input Handling is set to Both or Input System.
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Editor: Fixed an issue where the TextureImporter "Alpha From Grayscale" and non-default Swizzle settings would have no effect when used with R16 grayscale source images.
    ([UUM-89039](https://issuetracker.unity3d.com/issues/unsupported-texture-format-r16-for-a-swizzle-error-and-texture-is-not-correctly-rendered-when-using-texture-swizzle-and-reimporting-texture-asset))

- Editor: Fixed C\# script imported leading to missing documentation.
    ([UUM-87334](https://issuetracker.unity3d.com/issues/c-number-script-help-button-leads-to-missing-documentation))

- Editor: Fixed console being cleared after building a player.
    ([UUM-91487](https://issuetracker.unity3d.com/issues/build-failure-errors-are-cleared-before-you-can-read-them))

- Editor: Fixed Editor errors when "RGB + 1-bit Alpha Compressed ETC2 4 bits" compression is used.
    ([UUM-65395](https://issuetracker.unity3d.com/issues/editor-crashes-on-libetc-init-when-changing-webgl-texture-format-to-rgb-plus-1-bit-alpha-compressed-etc2-4-bits))

- Editor: Fixed help button tooltip text for some components.

- Editor: Fixed UnityWbRequest.error returning success after querying texture even though texture creation failed.
    ([UUM-90140](https://issuetracker.unity3d.com/issues/the-unitywebrequest-dot-result-of-the-unitywebrequesttexture-dot-gettexture-method-changes-when-accessing-unitywebrequest-dot-downloadhandler-texture))

- Editor: Fixed UniversalCameraAdditionalData trying to create missing UniversalRenderPipeline when OnDestroy\(\) is called.
    ([UUM-75237](https://issuetracker.unity3d.com/issues/cannot-create-required-material-because-shader-is-null-error-still-thrown-when-running-a-dedicated-server-build-with-checked-enable-dedicated-server-optimizations-player-settings-checkbox))

- Editor: Timeline tracks now accepts Objects with both object and exposed references.
    ([UUM-83224](https://issuetracker.unity3d.com/issues/the-object-is-not-attached-slash-assigned-when-assigning-an-object-to-a-timeline-track-expose-reference))

- GI: Ensured that the Lighting Window open reference button links to documentation for the correct Editor Version.
    ([UUM-83218](https://issuetracker.unity3d.com/issues/lighting-window-open-reference-button-links-to-documentation-for-wrong-editor-version))

- Graphics: Fixed a crash when importing a 16K normal map texture from gray scale.
    ([UUM-79322](https://issuetracker.unity3d.com/issues/crash-on-miniheightmap-extractnormalmap-00-when-16k-map-size-is-applied-with-create-from-grayscale-enabled))

- Graphics: Fixed an issue on Android platforms with Vulkan where swapchain recreation synchronization could cause a degenerate case where pausing the application during a scene load would result in a crash due to an invalid vkCmdEndRenderPass command being added to command buffers that have not begun a render pass.
    ([UUM-90287](https://issuetracker.unity3d.com/issues/vulkan-android-application-crashes-on-android-devices-with-vulkan-when-restoring-from-background))

- HDRP: Fixed HDRP ambient scene lighting leaking into the material preview window.
    ([UUM-84064](https://issuetracker.unity3d.com/issues/preview-of-the-material-is-displayed-incorrectly-when-the-texture-is-assigned-to-its-base-map))

- HDRP: Fixed invalid global state pushed when using override camera rendering in the CustomPassUtils functions.
    ([UUM-82849](https://issuetracker.unity3d.com/issues/render-passes-break-when-using-the-hdrp-custompassutils-dot-renderfromcamera-method-in-a-custom-pass))

- HDRP: Fixed wrong SSR when using a shader graph with a clear coat value of 0.
    ([UUM-84980](https://issuetracker.unity3d.com/issues/hdrp-clear-coat-materials-produce-screen-space-reflections-when-the-clear-coat-value-is-0-in-forward-only-lit-shader-mode))

- iOS: Fixed crash in Unity as a Library configuration after unloading Unity and rotating device.
    ([UUM-87752](https://issuetracker.unity3d.com/issues/uaal-freeze-on-getlightingsettingsordefaultsfallback-when-rotating-device-screen-after-unloading-unity-framework))

- iOS: Fixed QualitySettings handling \(when AA is involved\) in Split View.
    ([UUM-61559](https://issuetracker.unity3d.com/issues/ios-game-view-resolution-is-altered-when-changing-between-quality-levels-that-have-a-different-anti-aliasing-setting-on-ipad-with-split-view-active))

- iOS: Fixed WebCamDevice.availableResolutions returning \[0;0\] on some devices.
    ([UUM-87792](https://issuetracker.unity3d.com/issues/ios-webcamdevice-dot-availableresolutions-returns-a-single-resolution-with-width-and-height-both-0-on-some-ios-devices))

- Kernel: Optimized job system scheduling to scale better as thread count increases.
    (UUM-90028)

- Scripting: Added InstantiateParameters struct, this adds support for local space and target scenes to Object.InstantiateAsync.
    ([UUM-83002](https://issuetracker.unity3d.com/issues/cube-instantiated-by-the-instantiateasync-method-spawns-on-the-world-center-when-in-the-arguments-the-parent-is-passed-in))

- SpeedTree: Importer Model Editor Inspector: Custom unit conversion no longer allows negative scaling values, will display a warning when negative value is entered.
    ([UUM-82593](https://issuetracker.unity3d.com/issues/custom-unit-conversion-allows-to-set-negative-scale-factor))

- Terrain: Changed to use hierarchical transform for tree representation matrix.
    ([UUM-78866](https://issuetracker.unity3d.com/issues/shadows-of-trees-painted-on-the-terrain-are-incorrectly-placed-when-the-lighting-is-baked))

- UI Toolkit: Fixed layout issues that sometimes occurred between scene changes.
    ([UUM-87950](https://issuetracker.unity3d.com/issues/ui-elements-shrinking-misaligned-buttons-swapped-icons-or-incorrect-styles-when-rapidly-cycling-through-scenes-in-the-player))

- Version Control: By default, the additional line breaks are not getting added to asset files when merging with UnityYAMLMerge with an extra option for user to get the line breaks.
    ([UUM-72934](https://issuetracker.unity3d.com/issues/additional-line-breaks-are-added-to-asset-files-when-merging-with-unityyamlmerge))

- VFX Graph: Fixed an exception that could prevent opening a VFX in one specific case.
    ([UUM-85231](https://issuetracker.unity3d.com/issues/opening-a-vfx-graph-file-triggers-a-windows-prompt-select-an-app-to-open-this-vfx-file-and-logs-a-nullreferenceexception-error-to-the-console))

- VFX Graph: Usage of FogNode is always returning 1.0 in URP.
    ([UUM-85384](https://issuetracker.unity3d.com/issues/vfx-graph-urp-shadergraph-integration-issue-with-vfx-and-fog))

- Web: Fixed bug in `config.autoSyncPersistentDataPath` option in Unity Web.
    ([UUM-87753](https://issuetracker.unity3d.com/issues/webgl-typeerror-cannot-read-properties-of-undefined-reading-length-error-is-thrown-when-starting-the-player-when-config-dot-autosyncpersistentdatapath-is-set-to-true))

- Web: Fixed the mouse scrolling sensitivity in Web.
    ([UUM-84978](https://issuetracker.unity3d.com/issues/scrolling-on-a-default-scrollview-in-a-webgl-build-is-too-sensitive-when-compared-to-other-platform-builds-and-the-editor))

- XR: Fixed tracking origin mode validation logic.
    (UUM-90392)




## Package changes in 2022.3.56f1

## Packages updated

- com.unity.mobile.android-logcat: [1.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.performance.profile-analyzer: [1.2.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) to [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.4//changelog/CHANGELOG.html) to [2.5.1](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.13.2](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.13//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.11.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.11//changelog/CHANGELOG.html) to [1.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.12//changelog/CHANGELOG.html)

- com.unity.polyspatial: [1.3.9](https://docs.unity3d.com/Packages/com.unity.polyspatial@1.3//changelog/CHANGELOG.html) to [1.3.11](https://docs.unity3d.com/Packages/com.unity.polyspatial@1.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.visionos: [1.3.9](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@1.3//changelog/CHANGELOG.html) to [1.3.11](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@1.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.xr: [1.3.9](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@1.3//changelog/CHANGELOG.html) to [1.3.11](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@1.3//changelog/CHANGELOG.html)

- com.unity.xr.visionos: [1.3.9](https://docs.unity3d.com/Packages/com.unity.xr.visionos@1.3//changelog/CHANGELOG.html) to [1.3.11](https://docs.unity3d.com/Packages/com.unity.xr.visionos@1.3//changelog/CHANGELOG.html)