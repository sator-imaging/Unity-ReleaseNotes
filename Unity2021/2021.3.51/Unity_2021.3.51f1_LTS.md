# Unity 2021.3.51f1 LTS
Published at Wed, 16 Apr 2025 09:43:10 GMT  
https://unity.com/releases/editor/whats-new/2021.3.51

# Known Issues in 2021.3.51f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Graphics Device Features: Graphics.RenderMeshIndirect does not issue multi-draw rendering commands when using a graphics API capable of multi-draw commands
    ([UUM-91617](https://issuetracker.unity3d.com/issues/graphics-dot-rendermeshindirect-does-not-issue-multi-draw-rendering-commands-when-using-a-graphics-api-capable-of-multi-draw-commands))

- Vulkan:  Application crashes with Vulkan when restoring from background on Linux
    ([UUM-90287](https://issuetracker.unity3d.com/issues/vulkan-android-application-crashes-on-android-devices-with-vulkan-when-restoring-from-background))



# 2021.3.51f1 Release Notes

## Improvements

- Shadergraph: Removed duplicate LIGHTMAP_ON and DIRLIGHTMAP_COMBINED variants when generating shaders for builtin-deferred.

- TLS: Updated our internal version of MbedTLS to version 3.6. This version brings new and improved security features to network communications in the engine, but also means that unsecure and deprecated protocols are now unsupported. Notably, support for TLS 1.0 and 1.1 was removed.



## Changes

- Android: Added Android SDK 36 support.

- Android: Predictive Back Support is now enabled by default on new projects.

- XR: Updated com.unity.xr.openxr package version to 1.14.2.



## Fixes

- 2D: Fixed missing fog parameters in sprite subtargets.
    ([UUM-85456](https://issuetracker.unity3d.com/issues/fog-density-value-is-not-returned-when-using-the-fog-node-in-a-sprite-shader-graph))

- Android: Fixed an issue where StartActivityIndicator is displayed outside of safe area.
    (UUM-82238)

- Android: Fixed an issue where the AndroidActivityIndicatorStyle enum did not change.
    (UUM-79911)

- Android: Fixed an issue where the Player lost focus when UnityEngine.Handheld.StartActivityIndicator\(\) was used with the Facebook SDK.
    ([UUM-87564](https://issuetracker.unity3d.com/issues/android-the-player-loses-focus-when-using-unityengine-dot-handheld-dot-startactivityindicator-with-facebook-sdk))

- Android: Fixed dialog input field not getting dismissed after back gesture.
    (UUM-99637)

- Asset Pipeline: Fixed problem with main thread potentially being blocked, while doing async asset loads.
    ([UUM-95528](https://issuetracker.unity3d.com/issues/loading-animations-are-hitching-or-stopping-when-using-scenemanager-dot-loadsceneasync-to-load-new-scenes))

- Editor: Changed made to Static Emissives in Light Explorer do not add to Undo History.
    ([UUM-83357](https://issuetracker.unity3d.com/issues/changes-made-to-static-emissives-in-light-explorer-do-not-add-to-undo-history))

- Editor: Fixed an issue where the Device Simulator's scale would not persist when maximizing then minimizing another window.
    ([UUM-78562](https://issuetracker.unity3d.com/issues/the-simulator-tab-scale-is-reset-when-using-double-click-to-maximize-and-then-shrink-another-window))

- Editor: Fixed crash when class id in scene file does not match expected type e.g. Component as GameObject.
    ([UUM-91352](https://issuetracker.unity3d.com/issues/crash-on-malloc-internal-when-opening-a-project-after-reloading-a-scene))

- Editor: Fixed the `EditorStyles.whiteBoldLabel` style so the text is white.
    ([UUM-84114](https://issuetracker.unity3d.com/issues/editorguilayout-dot-labelfield-displays-black-text-when-the-editorstyles-dot-whiteboldlabel-parameter-is-passed-in))

- Graphics: Fixed ScalableBufferManager.ResizeBuffers not working with MSAA RTs.
    ([UUM-24634](https://issuetracker.unity3d.com/issues/ios-game-view-becomes-black-or-pink-when-using-scalablebuffermanager-dot-resizebuffers-with-msaa))

- iOS: Fixed soft keyboard Done/Cancel buttons truncating \(to "..."\) in languages like Korean due to decimal font width.
    ([UUM-97527](https://issuetracker.unity3d.com/issues/ios-hwagin-done-and-cwiso-cancel-text-is-displayed-as-dot-dot-dot-in-the-on-screen-keyboard-when-the-system-preferred-language-is-set-to-korean))

- UI Elements: Updated the pointer counter logic for collection views.
    ([UUM-82931](https://issuetracker.unity3d.com/issues/android-itemschosen-event-is-not-triggered-when-double-clicking-an-item-in-treeview-on-specific-devices))

- Windows: Fixed monitor handle association with the display details, for all resolutions.
    ([UUM-78860](https://issuetracker.unity3d.com/issues/screen-api-breaks-when-setting-resolution-below-1280x720-in-an-exclusive-fullscreen-player-on-a-specific-monitor))




## Package changes in 2021.3.51f1

## Packages updated

- com.unity.2d.pixel-perfect: [5.0.3](https://docs.unity3d.com/Packages/com.unity.2d.pixel-perfect@5.0//changelog/CHANGELOG.html) to [5.1.0](https://docs.unity3d.com/Packages/com.unity.2d.pixel-perfect@5.1//changelog/CHANGELOG.html)

- com.unity.2d.aseprite: [1.1.8](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) to [1.1.9](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.19](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.20](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.34](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.35](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.probuilder: [5.2.3](https://docs.unity3d.com/Packages/com.unity.probuilder@5.2//changelog/CHANGELOG.html) to [5.2.4](https://docs.unity3d.com/Packages/com.unity.probuilder@5.2//changelog/CHANGELOG.html)

- com.unity.services.analytics: [6.0.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html) to [6.0.3](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html)

- com.unity.services.vivox: [16.5.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.5//changelog/CHANGELOG.html) to [16.6.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.6//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.5.1](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) to [2.5.2](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.14.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html) to [1.14.2](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html)