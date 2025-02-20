# Unity 2021.3.49f1 LTS
Published at Tue, 18 Feb 2025 11:00:25 GMT  
https://unity.com/releases/editor/whats-new/2021.3.49

# 2021.3.49f1 Release Notes

## Improvements

- Documentation: Added a copy button to code examples in the documentation.



## Fixes

- Android: Allow build and run to work correctly when exporting an app bundle project.
    (UUM-91102)

- Audio: Fixed a bug that would cause the audio to not resume properly after unpausing a timeline.
    ([UUM-91654](https://issuetracker.unity3d.com/issues/audio-does-not-resume-playing-in-timeline-when-timescale-is-set-to-0-and-back-to-1-after-the-remainder-of-the-audio-has-passed-in-real-time))

- Editor: Do not accumulate vertical/horizontal scroll deltas for IMGUI events being triggered from native code.
    (UUM-79079)

- Editor: Editor exits Play mode when another project is being created.
    ([UUM-68141](https://issuetracker.unity3d.com/issues/editor-exits-play-mode-when-another-project-is-being-created-using-unity-hub-3-dot-8-0-beta-dot-1))

- Editor: Fixed a bug where using a render pipeline asset extending `UniversalRenderpipelineAsset` or its HDRP equivalent resulted in significantly longer build times.
    ([UUM-73223](https://issuetracker.unity3d.com/issues/shaders-are-not-being-striped-and-build-times-increase-when-using-a-custom-subclass-of-universalrenderpipelineasset))

- Editor: Fixed an error that caused terrain layer map corruption and console errors when painting with a global mipmap limit set.
    ([UUM-55985](https://issuetracker.unity3d.com/issues/terrain-layers-are-drawn-as-black-rectangular-splotches-on-a-terrain-when-the-terrain-splatmap-mip-levels-in-the-editor-and-on-the-gpu-are-mismatched-due-to-the-global-mipmap-limit-being-set-to-any-option-less-than-full-resolution))

- Editor: Fixed an issue on Windows where closing a Utility window with the Escape key would not prompt the user about saving or discarding unsaved changes.
    ([UUM-71291](https://issuetracker.unity3d.com/issues/pop-up-to-save-unsaved-changes-does-not-appear-when-closing-a-custom-editor-window-using-esc-key))

- Editor: Fixed crash when adding "MudBun" renderer.
    ([UUM-78781](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d11base-drawbuffersindirect-when-adding-mudbun-renderer))

- Editor: Fixed editor crash when a null object is passed in to EnsureUniqueSiblingName.
    ([UUM-91927](https://issuetracker.unity3d.com/issues/crash-on-ensureuniquesiblingname-when-calling-gameobjectutility-dot-ensureuniquenameforsibling-with-a-null-argument))

- Editor: Fixed GizmoType.NotInSelectionHierarchy gizmos not being restored on deselect.
    ([UUM-72297](https://issuetracker.unity3d.com/issues/gizmotype-dot-inselectionhierarchy-not-detected-correctly-when-nonselected-or-notinselectionhierarchy-is-defined))

- Editor: Fixed issue where the Gizmos and Layers menu opens and then closes and immediately reopens when you click the dropdown.
    ([UUM-91078](https://issuetracker.unity3d.com/issues/inconsistent-menu-behaviors-when-clicking-on-the-gizmo-menu-button-a-second-time))

- Editor: Fixed the selected marker on the timeline being offset incorrectly when zoomed out.
    ([UUM-55366](https://issuetracker.unity3d.com/issues/the-marker-highlight-is-offset-when-zooming-out-in-the-profiler-timeline))

- Graphics: Fixed the rendered color of the preset differs from the preview color when adding a new swatch in the HDR Color Picker.
    ([UUM-86724](https://issuetracker.unity3d.com/issues/the-rendered-color-of-the-preset-differs-from-the-preview-color-when-adding-a-new-swatch-in-the-hdr-color-picker))

- HDRP: Fixed an issue where the padding in the Lighting window was different between tabs.
    ([UUM-83840](https://issuetracker.unity3d.com/issues/lighting-window-has-a-different-padding-in-tabs))

- HDRP: Fixed black line artifacts on top of the screen with DRS and downsampled SSAO.
    ([UUM-69425](https://issuetracker.unity3d.com/issues/artifacts-are-seen-in-the-game-view-when-setting-dlss-custom-quality-mode-to-ultra-performance-and-using-the-qhd-resolution-in-play-mode))

- HDRP: Fixed HDRP sky rendering when Camera Relative Rendering is disabled.
    ([UUM-90251](https://issuetracker.unity3d.com/issues/sky-does-not-get-rendered-when-camerarelativerendering-is-disabled))

- IL2CPP: Removed the html report.  This fixes a UnityLinker crash when `--enable-report` is used on a large project.
    ([UUM-95599](https://issuetracker.unity3d.com/issues/unitylinker-causes-crash-when-outputting-snapshot-data-for-very-large-projects))

- Linux: Fixed assertion failure on ExFAT File systems when "Build and Run" is executed.
    ([UUM-91555](https://issuetracker.unity3d.com/issues/linux-assertion-failed-on-expression-success-and-and-actual-equals-equals-size-error-is-thrown-when-building-project-to-another-partition-with-a-different-file-system))

- Package Manager: Fixed crash when package contains a dependency with null version in the package manifest.
    ([UUM-64442](https://issuetracker.unity3d.com/issues/crash-on-stackwalker-getcurrentcallstack-when-opening-a-specific-project))

- Package Manager: Fixed the issue where selecting an organization with spaces in its name in the inspector caused validation errors and won't let save changes. Organization names are now automatically sanitized to remove spaces.
    (UUM-79730)

- Package Manager: Packages installed on external `FAT32/exFAT` drives should not fail when the `mtime` is outside of the supported range.
    ([UUM-86351](https://issuetracker.unity3d.com/issues/unable-to-install-probuilder-package-when-project-is-located-in-an-external-fat32-slash-exfat-drive))

- Scripting: Fixed pool cleanup on entering playmode with domain reload disabled.
    ([UUM-90313](https://issuetracker.unity3d.com/issues/object-pools-do-not-reset-when-re-entering-the-play-mode-with-reload-domain-disabled))

- Shaders: Fixed a situation where some shaders would appear to cause an internal communcations error with the shader compiler.
    ([UUM-72852](https://issuetracker.unity3d.com/issues/linux-shader-communication-error-gets-thrown-when-opening-the-project-which-is-using-bruteforce-shader))

- Shaders: Fixed corrupted shader property name after loading an asset bundle.
    ([UUM-59309](https://issuetracker.unity3d.com/issues/isbuiltin-method-skips-new-index-generation-when-called-in-a-different-order))

- Terrain: Fixed bug in which grass details always used the default rendering layer mask.
    ([UUM-91894](https://issuetracker.unity3d.com/issues/light-is-not-applied-properly-to-terrain-details-when-using-light-layers))

- Terrain: Terrain Detail objects are not rendered in the build when the Terrain is generated at runtime.
    ([UUM-62407](https://issuetracker.unity3d.com/issues/terrain-detail-objects-are-not-rendered-in-the-build-when-the-terrain-is-generated-at-runtime))

- Universal RP: Fixed Implicit truncation of vector type shader warning.
    ([UUM-87081](https://issuetracker.unity3d.com/issues/shader-warning-in-universal-render-pipeline-slash-particles-slash-simple-lit-implicit-truncation-of-vector-type-warning-is-thrown-after-building-the-project))

- Universal RP: Fixed light cookie texture memory leak when entering Playmode.
    ([UUM-92512](https://issuetracker.unity3d.com/issues/lights-with-cookies-generate-cookie-atlas-and-increase-memory-usage-every-time-when-play-mode-is-entered))

- Video: Resolve issue where VideoClip importer incorrectly caches failed import results on the cache server.
    (UUM-77249)

- Web: Fixed a bug where users could not successfully set the webcam resolution on the Web platform.
    ([UUM-87702](https://issuetracker.unity3d.com/issues/webcamtexture-does-not-set-the-requested-resolution-when-used-in-webgl))

- XR: Updated XR Legacy Input Helpers \(com.unity.xr.legacyinputhelpers\) to version 2.1.12.




## Package changes in 2021.3.49f1

## Packages updated

- com.unity.2d.aseprite: [1.1.7](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) to [1.1.8](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.18](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.19](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.xr.legacyinputhelpers: [2.1.11](https://docs.unity3d.com/Packages/com.unity.xr.legacyinputhelpers@2.1//changelog/CHANGELOG.html) to [2.1.12](https://docs.unity3d.com/Packages/com.unity.xr.legacyinputhelpers@2.1//changelog/CHANGELOG.html)