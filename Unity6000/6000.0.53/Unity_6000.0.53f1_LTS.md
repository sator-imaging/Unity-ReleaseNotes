# Unity 6000.0.53f1 LTS
Published at Wed, 09 Jul 2025 06:34:27 GMT  
https://unity.com/releases/editor/whats-new/6000.0.53

# Known Issues in 6000.0.53f1

- 2D: UI is not rendering and an error is thrown when FXAA is enabled and cameras are stacked in a 2D URP project
    ([UUM-110338](https://issuetracker.unity3d.com/issues/ui-is-not-rendering-and-an-error-is-thrown-when-fxaa-is-enabled-and-cameras-are-stacked-in-a-2d-urp-project))

- Android: [GameActivity] Crash on "UnityMotionEventCallbacks::_GetPointerIdImpl" when giving 9+ simultaneous touch inputs 
    ([UUM-108743](https://issuetracker.unity3d.com/issues/android-crash-on-unitymotioneventcallbacks-getpointeridimpl-when-giving-8-simultaneous-touch-inputs))

- Asset Store / Publisher portal: Accepting Asset Store EULA endless loop in Package Manager window
    ([UUM-83708](https://issuetracker.unity3d.com/issues/accepting-asset-store-eula-endless-loop-in-package-manager-window))

- Cloud Diagnostics: [Android]Crash on lib/arm64/libil2cpp.so when Unity Analytics and Engine Code stripping are enabled
    ([UUM-95408](https://issuetracker.unity3d.com/issues/android-crash-on-lib-slash-arm64-slash-libil2cpp-dot-so-when-unity-analytics-and-engine-code-stripping-are-enabled))

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

- Platform Audio: Android Player freezes when an Audio Source is playing and an incoming call is picked up and then hung up and the Audio Source is started again
    ([UUM-103525](https://issuetracker.unity3d.com/issues/android-player-freezes-when-an-audio-source-is-playing-and-an-incoming-call-is-picked-up-and-then-hung-up-and-the-audio-source-is-started-again))

- SRP XR: GameObjects are transparent when a custom fog renderer feature is enabled
    ([UUM-104832](https://issuetracker.unity3d.com/issues/gameobjects-are-transparent-when-a-custom-fog-renderer-feature-is-enabled))

- SRP XR: The Player renders black on a Quest headset when MSAA, Post Processing, and Spacewarm depth submission are enabled
    ([UUM-84612](https://issuetracker.unity3d.com/issues/the-player-renders-black-on-a-quest-headset-when-msaa-post-processing-and-spacewarm-depth-submission-are-enabled))

- Vulkan: AndroidPlayer selects Vulkan Graphics API over GLES even on devices with limited support
    ([UUM-109250](https://issuetracker.unity3d.com/issues/androidplayer-selects-vulkan-graphics-api-over-gles-even-on-devices-with-limited-support))

- Vulkan: [Android] Runtime performance deteriorates on certain Android devices when Graphics API is set to Vulkan on an upgraded project
    ([UUM-107530](https://issuetracker.unity3d.com/issues/build-performance-deteriorates-on-certain-android-devices-when-graphics-api-is-set-to-vulkan-on-an-upgraded-project))



# 6000.0.53f1 Release Notes

## Improvements

- Documentation: Added keyboard support for copying code examples.

- QNX: Multidisplay monitor commandline argument.

- QNX: Window z-order index setting.



## API Changes

- UI Toolkit: Added: Added two new fields to UxmlElementAttribute:<br>
    - visibility: Defaults to "Default" but can be set to "Visible" or "Hidden" to override the default behavior, which hides elements with namespaces starting with Unity, UnityEngine, and UnityEditor.<br>
    - libraryPath: Allows customization of the path where the element is displayed in the Project Library tab.
    ([UUM-104888](https://issuetracker.unity3d.com/issues/custom-elements-not-visible-in-ui-builder-when-defined-in-a-namespace-starting-with-unity))



## Fixes

- 2D: Fixed an issue in the Shadow Caster 2D shape editor that could cause exceptions to be thrown.
    (UUM-97647)

- 2D: Fixed an issue with the TilemapRenderer when the TilemapRenderer has a Mask Interaction set to None and the user uses a shader which utilises the stencil buffer, and the stencil settings in the shader are not respected.
    ([UUM-109109](https://issuetracker.unity3d.com/issues/tilemap-renderer-does-not-reflect-the-stencil-buffer-when-the-tilemap-renderer-mode-is-set-to-chunk))

- Audio: Fixed an issue that would cause the main thread to stall when loading projects/scenes.
    ([UUM-100966](https://issuetracker.unity3d.com/issues/main-thread-stalling-when-loading-audio-source-asset-asynchronously-while-preloading-another-audio-source-asset))

- Audio: Fixed an issue where the "Audio Resource" field on an Audio Source in some cases wouldn't be properly updated in prefabs.
    ([UUM-104751](https://issuetracker.unity3d.com/issues/overrides-in-nested-prefabs-are-ignored-when-importing))

- DX12: Stencil reference value is applied correctly when using graphics jobs.
    (UUM-92267)

- Editor: Added a message so the macOS Editor can properly ask the user for permission to access the microphone. This fixes a bug where if the Editor was launched via './run', instead of the Unity Hub, the microphone would not work.
    (UUM-109276)

- Editor: Fixed an issue where the Unity Editor would still open after a user terminated the launch screen during project load.
    ([UUM-107863](https://issuetracker.unity3d.com/issues/the-editor-opens-when-the-window-is-closed-right-after-launch))

- Editor: Fixed floating license cleanup and concurrent license update in LicensingClient 1.17.1.

- Editor: Fixed method decorated with HideInCallstack attribute being opened by IDE instead of the caller method.
    ([UUM-99776](https://issuetracker.unity3d.com/issues/hidden-method-is-opened-in-ide-when-double-clicking-the-log-message-in-the-console-that-has-the-hideincallstackattribute))

- Editor: Improved preview window toolbar style so large labels do not take too much space.
    ([UUM-110119](https://issuetracker.unity3d.com/issues/preview-window-buttons-are-pushed-out-by-header-text))

- Editor: Loading RenderDoc in Windows Editor does not crash when GPU skinning\(Batched\) is enabled.
    ([UUM-105820](https://issuetracker.unity3d.com/issues/crash-on-d3dkmtopenresource-when-capturing-with-renderdoc-while-gpu-skinning-is-set-to-gpu-batched))

- Editor: Removed an assert to replace it with a debug assert due to an issue with hierarchical animation component.
    ([UUM-109748](https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-error-occurs-when-multiple-animation-components-are-instantiated-after-changing-the-culling-type))

- Editor: SpeedTree meshes and objects count differs when comparing the numbers in the Player with the Editor.
    ([UUM-105402](https://issuetracker.unity3d.com/issues/speedtree-meshes-and-objects-count-differs-when-comparing-the-numbers-in-the-player-with-the-editor))

- GI: Make APV work with Subscenes in URP.
    (UUM-104165)

- Graphics: Fixed the "get_disableApplyMaterialPropertyDrawers can only be called from the main thread" exception that occurred occasionally with GPU Resident Drawer after a domain reload.
    ([UUM-101193](https://issuetracker.unity3d.com/issues/unityexception-get-disableapplymaterialpropertydrawers-can-only-be-called-from-the-main-thread))

- Input System: Fixed a problem where two devices were detected when connecting a wireless Nintendo Switch Pro controller on Windows.
    (UUM-109997)

- Input System: Resolved an issue with the Siri Remote \(Gen2\) where navigating with the Directional Pad caused `buttonSouth` to become true. This was due to OS propogating A button events after a D-Pad click \(rather than a swipe\).
    (UUM-110170)

- Profiler: Fixed Player hang during Autoconnect on long Player initialization.
    ([UUM-101218](https://issuetracker.unity3d.com/issues/player-unresponsive-when-building-a-specific-project-with-autoconnect-profiler-enabled))

- Scripting: Added warning to tag manager if trying to add the same tag more than once.
    ([UUM-99990](https://issuetracker.unity3d.com/issues/no-error-notification-is-displayed-when-creating-a-tag-with-an-already-existing-name))

- Scripting: Scripting: Prevent recursion when unloading Scriptable Object.
    ([UUM-77941](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-calling-unloadresources-with-the-ondisable-function))

- Search: Support interface filtering for component and asset types.
    ([UUM-109613](https://issuetracker.unity3d.com/issues/search-filtering-by-interface-type-does-not-work))

- UI Toolkit: Fixed the UI Builder New Selector field, changing the insertion point to the end when typing.
    ([UUM-109015](https://issuetracker.unity3d.com/issues/ui-builder-insertion-point-jumps-to-the-end-of-the-string-when-editing-a-new-selector-name))

- Universal RP: Fixed black screen when using lens flare with bloom mip bias 0.
    ([UUM-109463](https://issuetracker.unity3d.com/issues/game-view-fails-to-render-and-becomes-dark-when-the-screen-space-lens-flare-components-intensity-is-set-to-1-and-the-bloom-mip-bias-is-set-to-0))

- Version Control: Added Beyond Compare 5 support to Yaml Merge.
    ([UUM-109861](https://issuetracker.unity3d.com/issues/beyond-compare-5-is-not-supported-by-yaml-merge))

- Video: \[Windows\] Editor no longer crashes when listing webcams whose name is missing or empty. Such cameras are now skipped safely \(with a warning in the Editor\).
    ([UUM-105563](https://issuetracker.unity3d.com/issues/editor-crashes-with-platformwebcamtexture-getdevicenames-when-a-virtual-camera-is-present-and-friendlyname-property-is-deleted-from-registry))




## Package changes in 6000.0.53f1

## Packages updated

- com.unity.2d.animation: [10.1.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.1//changelog/CHANGELOG.html) to [10.2.1](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html)

- com.unity.2d.common: [9.0.7](https://docs.unity3d.com/Packages/com.unity.2d.common@9.0//changelog/CHANGELOG.html) to [9.1.1](https://docs.unity3d.com/Packages/com.unity.2d.common@9.1//changelog/CHANGELOG.html)

- com.unity.2d.psdimporter: [9.0.3](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.0//changelog/CHANGELOG.html) to [9.1.0](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html)

- com.unity.localization: [1.5.2](https://docs.unity3d.com/Packages/com.unity.localization@1.5//changelog/CHANGELOG.html) to [1.5.5](https://docs.unity3d.com/Packages/com.unity.localization@1.5//changelog/CHANGELOG.html)

- com.unity.services.levelplay: [8.6.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.6//changelog/CHANGELOG.html) to [8.9.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.9//changelog/CHANGELOG.html)