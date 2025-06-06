# Unity 6000.0.34f1 LTS
Published at Wed, 15 Jan 2025 13:46:28 GMT  
https://unity.com/releases/editor/whats-new/6000.0.34

# Known Issues in 6000.0.34f1

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- Audio Authoring: Audio Reverb Zone still produces sound when the Audio Source volume is 0
    ([UUM-92689](https://issuetracker.unity3d.com/issues/audio-reverb-zone-still-produces-sound-when-the-audio-source-volume-is-0))

- Audio Authoring: Audio Source clip is not audible when exceeding a high number of active Audio Sources
    ([UUM-91256](https://issuetracker.unity3d.com/issues/audio-source-clip-is-not-audible-when-exceeding-a-high-number-of-active-audio-sources))

- Build Settings Window: Application Cloud Connection Id is incorrect when using Build Profile with Player Setting Overrides.
    ([UUM-90426](https://issuetracker.unity3d.com/issues/application-cloud-connection-id-is-incorrect-when-using-build-profile-with-player-setting-overrides))

- DirectX12: A memory leak occurs in Play mode when using Direct3D12 Graphics API
    ([UUM-91900](https://issuetracker.unity3d.com/issues/a-memory-leak-occurs-in-play-mode-when-using-direct3d12-graphics-api))

- DirectX12: Allocated graphics memory does not get released when the Editor is out of focus while using D3D12 graphics API
    ([UUM-86354](https://issuetracker.unity3d.com/issues/allocated-graphics-memory-does-not-get-released-when-the-editor-is-out-of-focus-while-using-d3d12-graphics-api))

- DirectX12: The Camera does not render correctly when the Camera.Rect() is changed and HDR is enabled and DX12 graphics API is selected
    ([UUM-86917](https://issuetracker.unity3d.com/issues/the-camera-does-not-render-correctly-when-the-camera-dot-rect-is-changed-and-hdr-is-enabled-and-dx12-graphics-api-is-selected))

- Graphics Device Features: D3D12 PSO disk cache feature crashes if paths contain non-ASCII characters
    ([UUM-92417](https://issuetracker.unity3d.com/issues/d3d12-pso-disk-cache-feature-crashes-if-paths-contain-non-ascii-characters))

- Graphics Optimization Systems: Vertex snapping doesn't work when the GPU Resident Drawer is enabled
    ([UUM-66422](https://issuetracker.unity3d.com/issues/vertex-snapping-doesnt-work-when-the-gpu-resident-drawer-is-enabled))

- HDRP: Graphics Compositor breaks Unity rendering when the "Output Camera" is changed to a scene Camera and one Camera SubLayer is active.<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84610

- Input: Player .exe remains open as a background task after closing it when Active Input Handling is set to "Input System Package (New)"
    ([UUM-91181](https://issuetracker.unity3d.com/issues/player-exe-remains-open-as-a-background-task-after-closing-it-when-active-input-handling-is-set-to-input-system-package-new))

- Materials: Decal Projector produces artifacts when the normal and decal are projected in negative z-direction and Normal Blend is set to 1
    ([UUM-92200](https://issuetracker.unity3d.com/issues/decal-projector-produces-artifacts-when-the-normal-and-decal-are-projected-in-negative-z-direction-and-normal-blend-is-set-to-1))

- Packman: Unable to install ProBuilder package when project is located in an external FAT32/exFAT drive
    ([UUM-86351](https://issuetracker.unity3d.com/issues/unable-to-install-probuilder-package-when-project-is-located-in-an-external-fat32-slash-exfat-drive))

- Scene View: Can not navigate through the Scene view when using a drawing tablet
    ([UUM-90436](https://issuetracker.unity3d.com/issues/can-not-navigate-through-the-scene-view-when-using-a-drawing-tablet))

- Serialization: [windows only] Switching Project when importing complete project does not import all assets and project opens incomplete
    ([UUM-88051](https://issuetracker.unity3d.com/issues/switching-project-when-importing-complete-project-does-not-import-all-assets-and-project-opens-incomplete))

- SpeedTree: This release of SpeedTree includes a change to the interface of the SpeedTree8Wind shadergraph node. If you have an animated SpeedTree in the shadergraph, be sure to connect an ObjectSpacePosition node to the input of the SpeedTree8Wind.  If the wind node does not have an input on the ObjectSpacePosition port, the mesh will be shrunk down to a point at origin \(making it seem to vanish\).<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84616

- Terrain: Trees do not render in 'Unity Terrain - URP Demo Scene'
    ([UUM-84616](https://issuetracker.unity3d.com/issues/trees-do-not-render-in-unity-terrain-urp-demo-scene))

- Text: Crash on tlsf_free when generating the Font Atlas
    ([UUM-91956](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-the-font-atlas))

- Texture: Sprite Atlas Override for iOS setting remains disabled when saving its change to enabled
    ([UUM-90066](https://issuetracker.unity3d.com/issues/sprite-atlas-override-for-ios-setting-remains-disabled-when-saving-its-change-to-enabled))

- Vulkan: [Android] [Vulkan] Cubes stuck on the first few frames of rotation and application flickering when an Overlay Camera is added to the Camera Stack with MSAA enabled
    ([UUM-92429](https://issuetracker.unity3d.com/issues/android-vulkan-cubes-stuck-on-the-first-few-frames-of-rotation-and-application-flickering-when-an-overlay-camera-is-added-to-the-camera-stack-with-msaa-enabled))

- Windows: Player remains in Windows Background processes when the application is closed
    ([UUM-87775](https://issuetracker.unity3d.com/issues/urp-player-remains-in-windows-background-processes-when-the-application-is-closed))



# 6000.0.34f1 Release Notes

## Fixes

- 2D: Fixed active buffers for overlay in Rendergraph2D
    ([UUM-83013](https://issuetracker.unity3d.com/issues/errors-are-thrown-when-using-stacking-cameras-with-two-different-renderer2ddata))

- Editor: Fixed an editor crash in the HDRP samples
    (UUM-91532)

- Editor: Fixed an issue where the editor could occasionally crash when exiting the editor with the Input System package included and the Active Input Handling is set to Both or Input System.
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Editor: Fixed incorrect reporting of missing script compilation files when using source generators
    ([UUM-86938](https://issuetracker.unity3d.com/issues/path-could-not-be-found-for-script-compilation-file-error-is-thrown-when-the-files-are-injected-with-registerpostinitializationoutput))

- Editor: Fixed timeline tracks to now accepts Objects with both object and exposed references
    ([UUM-83224](https://issuetracker.unity3d.com/issues/the-object-is-not-attached-slash-assigned-when-assigning-an-object-to-a-timeline-track-expose-reference))

- GI: Ensured that the Lighting Window open reference button links to documentation for the correct Editor Version
    ([UUM-83218](https://issuetracker.unity3d.com/issues/lighting-window-open-reference-button-links-to-documentation-for-wrong-editor-version))

- GI: Fixed sample APV to get proper reflection probe normalization when doing SSGI in scenes where APV has been baked.
    ([UUM-88018](https://issuetracker.unity3d.com/issues/apv-reflection-probe-normalization-breaks-when-ssgi-is-enabled))

- HDRP: Fixed black line artifacts on top of the screen with DRS and downsampled SSAO
    ([UUM-69425](https://issuetracker.unity3d.com/issues/artifacts-are-seen-in-the-game-view-when-setting-dlss-custom-quality-mode-to-ultra-performance-and-using-the-qhd-resolution-in-play-mode))

- HDRP: Fixed invalid global state pushed when using override camera rendering in the CustomPassUtils functions.
    ([UUM-82849](https://issuetracker.unity3d.com/issues/render-passes-break-when-using-the-hdrp-custompassutils-dot-renderfromcamera-method-in-a-custom-pass))

- HDRP: Fixes the bug where DebugDisplay Camera list grew beyond number of active cameras, every time a camera was registered or unregistered.
    (UUM-86686)

- macOS: Ctrl+C not caught on headless MacOS games, in turn, OnApplicationQuit does not get called
    ([UUM-87122](https://issuetracker.unity3d.com/issues/onapplicationquit-is-not-called-and-logger-debug-lines-are-missing-in-player-log-when-exiting-mac-dedicated-server))

- Shaders: Fixed a rare crash during removal of unused material properties.
    ([UUM-91648](https://issuetracker.unity3d.com/issues/crash-on-material-removeunusedproperties-when-removing-unused-properties-from-a-broken-material-component))

- SpeedTree: Fixed Importer Model Editor Inspector: Custom unit conversion no longer allows negative scaling values, will display a warning when negative value is entered
    ([UUM-82593](https://issuetracker.unity3d.com/issues/custom-unit-conversion-allows-to-set-negative-scale-factor))

- UI Toolkit: Fixed a recursive event dispatching loop when scrolling to the last item in a dynamic height ListView.
    ([UUM-87164](https://issuetracker.unity3d.com/issues/listviews-plus-button-causes-a-recursively-dispatching-event-when-the-visual-element-area-is-filled-up))

- UI Toolkit: Fixed an issue that caused an InvalidOperationException when selecting a VisualTreeAsset with a referenced data source.
    ([UUM-86661](https://issuetracker.unity3d.com/issues/invalidoperationexception-error-appears-when-selecting-a-specific-visual-tree-asset))

- VFX Graph: Fixed a small cursor offset when drawing a rectangle selection
    ([UUM-86681](https://issuetracker.unity3d.com/issues/vfx-graph-selection-rectangle-corner-misaligned-with-mouse))

- VFX Graph: Fixed reordering properties inside a category was not possible anymore.<br>
    Also reordering a category could not work if there was properties at the root \(with no category\)
    ([UUM-83678](https://issuetracker.unity3d.com/issues/vfx-graph-properties-cannot-be-reordered-when-inside-a-categoy))

- Web: Fixed the mouse scrolling sensitivity in Web
    ([UUM-84978](https://issuetracker.unity3d.com/issues/scrolling-on-a-default-scrollview-in-a-webgl-build-is-too-sensitive-when-compared-to-other-platform-builds-and-the-editor))




## Package changes in 6000.0.34f1

## Packages updated

- com.unity.xr.core-utils: [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) to [2.5.1](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.sharp-zip-lib: [1.3.8](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.3//changelog/CHANGELOG.html) to [1.3.9](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.3//changelog/CHANGELOG.html)