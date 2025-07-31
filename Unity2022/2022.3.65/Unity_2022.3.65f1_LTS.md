# Unity 2022.3.65f1 LTS
Published at Wed, 30 Jul 2025 10:57:20 GMT  
https://unity.com/releases/editor/whats-new/2022.3.65

# Known Issues in 2022.3.65f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DirectX12: The Player hangs when unloading a scene using the UnloadUnusedAssets() method
    ([UUM-79718](https://issuetracker.unity3d.com/issues/the-player-hangs-when-unloading-a-scene-using-the-unloadunusedassets-method))

- Scene Management: Editor hangs when cutting and pasting a Script to another folder during Play Mode
    ([UUM-104031](https://issuetracker.unity3d.com/issues/editor-hangs-when-cutting-and-pasting-a-script-to-another-folder-during-play-mode))

- Texture: Crash on PersistentManager::GetSerializedFileIfObjectAvailable when opening a specific project
    ([UUM-101784](https://issuetracker.unity3d.com/issues/crash-on-persistentmanager-getserializedfileifobjectavailable-when-opening-a-specific-project))

- Video: Editor crashes with PlatformWebCamTexture::GetDeviceNames when a Virtual Camera is present and FriendlyName property is deleted from Registry
    ([UUM-105563](https://issuetracker.unity3d.com/issues/editor-crashes-with-platformwebcamtexture-getdevicenames-when-a-virtual-camera-is-present-and-friendlyname-property-is-deleted-from-registry))

- Video: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)

- Video: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    ([UUM-111599](https://issuetracker.unity3d.com/issues/videoplayer-freezes-or-stops-on-certain-android-devices-when-enabling-and-disabling-the-video-multiple-times))



# 2022.3.65f1 Release Notes

## Improvements

- Documentation: Added keyboard support for copying code examples.

- DX12: Set ID3D12GraphicsCommandList::IASetVertexBuffers once instead of several times in a loop inside GfxDeviceD3D12Base::DrawBuffersCommon.
    (UUM-109282)



## Changes

- XR: Updated com.unity.xr.openxr package version to 1.15.0.



## Fixes

- 2D: Fixed issue with the TilemapRenderer when the TilemapRenderer has a Mask Interaction set to None and the user uses a shader which utilises the stencil buffer, and the stencil settings in the shader are not respected.
    ([UUM-109109](https://issuetracker.unity3d.com/issues/tilemap-renderer-does-not-reflect-the-stencil-buffer-when-the-tilemap-renderer-mode-is-set-to-chunk))

- 2D: Improved validation of RefreshTile Tilemap argument signature in Editor.
    ([UUM-109125](https://issuetracker.unity3d.com/issues/crash-on-tilemap-gettileasset-when-calling-tilemap-dot-gettile-in-new-refreshtile-method-for-tilebase-class))

- Android: Fixed warning showing libraries as not 16 KB page aligned when they have been updated externally.
    ([UUM-111393](https://issuetracker.unity3d.com/issues/android-native-libraries-dot-so-are-not-checked-for-16kb-alignment-when-modified-externally))

- Asset Import: Asset Import: Fixed indeterminism of artifact ids which could occur when importers set dependencies to other assets.
    (UUM-107448)

- Audio: Fixed a sudden dropout of high priority sounds in the game under rare circumstances, when playing multiple new Audio Sources on the same frame as having stopped Audio Sources whilst exceeding the number of real voices available in the system.
    (UUM-101807)

- DX12: Fixed for crash when running with Native Jobs.
    (UUM-110198)

- Editor: Added a message so the macOS Editor can properly ask the user for permission to access the microphone. This fixes a bug where if the Editor was launched via './run', instead of the Unity Hub, the microphone would not work.
    (UUM-109276)

- Editor: Added warning to tag manager if trying to add the same tag more than once.
    ([UUM-99990](https://issuetracker.unity3d.com/issues/no-error-notification-is-displayed-when-creating-a-tag-with-an-already-existing-name))

- Editor: Fixed a bug where ctrl + left click would not open the contextual menu for the Orientation Gizmo and added support for Mac's two-finger click.
    (UUM-102749)

- Editor: Fixed a crash that occurred after resetting packages while prefabs from those packages are open in the active scene.
    ([UUM-97847](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-virtualredirecttransfer-when-closing-editor-after-removing-hdpr-and-importing-water-samples-before))

- Editor: Fixed a slight performance regression in build pipeline.
    (UUM-108628)

- Editor: Fixed changes to fields that used delayed fields not being saved in prefab scenes.
    ([UUM-107890](https://issuetracker.unity3d.com/issues/values-in-rect-transform-component-are-only-partially-updated-when-changing-values-in-prefab-mode))

- Editor: Fixed Cursor.visible ignoring CursorLockMode.Locked.
    ([UUM-85853](https://issuetracker.unity3d.com/issues/mouse-pointer-remains-visible-on-screen-when-cursor-dot-lockstate-is-set-to-cursorlockmode-dot-locked-and-cursor-dot-visible-gets-set-to-true-in-update))

- Editor: Fixed floating license cleanup and concurrent license update in LicensingClient 1.17.1.

- Editor: Fixed IMGUI EditorGUIUtility.labelWidth value being changed by the Scene View UI. This could impact other windows drawn afterwards.
    ([UUM-110450](https://issuetracker.unity3d.com/issues/editorguilayout-dot-toggle-clickable-area-is-shifted-when-using-built-in-render-pipeline))

- Editor: Fixed issue where the Unity Editor would still open after a user terminated the launch screen during project load.
    ([UUM-107863](https://issuetracker.unity3d.com/issues/the-editor-opens-when-the-window-is-closed-right-after-launch))

- Editor: Fixed method decorated with HideInCallstack attribute being opened by IDE instead of the caller method.
    ([UUM-99776](https://issuetracker.unity3d.com/issues/hidden-method-is-opened-in-ide-when-double-clicking-the-log-message-in-the-console-that-has-the-hideincallstackattribute))

- Editor: Fixed prefab stage applying changes too early.
    ([UUM-107890](https://issuetracker.unity3d.com/issues/values-in-rect-transform-component-are-only-partially-updated-when-changing-values-in-prefab-mode))

- Editor: Fixed SerializedProperty errors that could occur when editing and canceling the edit for an int2 followed by float2.
    ([UUM-110524](https://issuetracker.unity3d.com/issues/serializedproperty-errors-are-thrown-when-pressing-the-esc-key-to-cancel-the-modification-of-int-or-float-values))

- Editor: Fixed the method to get object picker control ID while avoiding creating a new instance.
    ([UUM-110121](https://issuetracker.unity3d.com/issues/invalid-editor-window-of-type-unityeditor-dot-objectselector-error-message-is-thrown-when-maximizing-any-editor-window))

- Editor: Fixed VFX not repainted when changing some asset properties.
    ([UUM-99917](https://issuetracker.unity3d.com/issues/vfx-are-not-reinit-immediatly-when-changing-properties-in-asset-inspector))

- Editor: Updated 7-Zip to 25.00.

- Graphics: Fixed issue that may cause redundant clear-only renderpass when using Vulkan.
    ([UUM-100540](https://issuetracker.unity3d.com/issues/urp-vulkan-vkcmdbeginrenderpass-is-called-twice-with-the-same-framebuffer))

- Graphics: Fixed Vulkan performance decrease from redundant clear-only renderpass.
    ([UUM-107530](https://issuetracker.unity3d.com/issues/build-performance-deteriorates-on-certain-android-devices-when-graphics-api-is-set-to-vulkan-on-an-upgraded-project))

- Graphics: Speculative fix for potential race conditions in CalculateSkinningMatrices by ensuring direct job completion for improved safety.
    ([UUM-111486](https://issuetracker.unity3d.com/issues/android-crash-on-skinnedmeshrenderermanager-calculateskinningmatrices))

- Input System: Fixed a problem where two devices were detected when connecting a wireless Nintendo Switch Pro controller on Windows.
    (UUM-109997)

- Linux: Fixed Linux runtime not respecting popupwindow argument.
    ([UUM-105221](https://issuetracker.unity3d.com/issues/desktop-linux-runtime-does-not-respect-popupwindow-command-line-argument))

- Mono: Fixed issue where mono's debugger agent thread would not restart when a connection issue was encountered.
    (UUM-107431)

- Package Manager: Fixed the issue where the selection system throws exception when handling null package unique ids.
    ([UUM-110109](https://issuetracker.unity3d.com/issues/argumentnullexception-value-cannot-be-null-dot-error-is-thrown-after-pressing-go-to-settings-button-in-the-no-adaptive-performance-provider-found-pop-up-window))

- Player: The DeveloperConsole now correctly opens after being re-enabled, fixing an issue where it would remain stuck in a closed state.
    ([UUM-109718](https://issuetracker.unity3d.com/issues/debug-console-does-not-reappear-when-disabling-and-re-enabling-debug-dot-developerconsoleenabled))

- uGUI: Updated Image raycast behavior to ensure consistent handling of screenPoints outside bounds, preventing parent Images from blocking child Images.
    ([UUM-110769](https://issuetracker.unity3d.com/issues/child-image-does-not-trigger-an-event-when-the-parent-image-is-using-alphahittestminimumthreshold-0))

- UI Toolkit: Fixed an exceptions when displaying PropertyFields bound to an array named "Array" in the inspector.
    ([UUM-110573](https://issuetracker.unity3d.com/issues/binding-listview-failed-warning-is-thrown-when-a-gameobject-with-an-attached-script-containing-an-array-or-list-named-array-is-selected))

- UI Toolkit: Fixed an issue with PropertyFields bound to an array named "Array" throwing an exception when the add button was clicked.
    ([UUM-110572](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-attempting-to-add-an-element-to-an-array-or-list-named-array-in-the-inspector))

- UI Toolkit: Fixed crash when stroking rounded joins with Painter2D.
    ([UUM-110455](https://issuetracker.unity3d.com/issues/crash-on-uitoolkit-uipainter2d-strokeroundedcap-when-drawing-an-arc-with-painter2d-on-specific-progress-value-using-linecap-dot-round))

- UI Toolkit: Fixed intermittent crash on AppleTV on Painter2D.ClosePath\(\) call.
    ([UUM-105548](https://issuetracker.unity3d.com/issues/tvos-exc-bad-access-error-is-thrown-when-painter2d-dot-closepath-is-called))

- UI Toolkit: Fixed property field indentation.
    ([UUM-108741](https://issuetracker.unity3d.com/issues/header-attribute-is-misaligned-when-placed-before-an-inputactionproperty-field))

- URP: Fixed yflip issue when depth intermediate texture is required and non-RG is in use.
    ([UUM-108074](https://issuetracker.unity3d.com/issues/depth-texture-is-flipped-when-specific-urp-rendering-settings-are-applied))

- Video: \[Android\] VideoPlayer leaks memory when repeating Play and Stop on a Video.
    ([UUM-77668](https://issuetracker.unity3d.com/issues/android-videoplayer-leaks-memory-when-repeating-play-and-stop-on-a-video))

- Video: \[Windows\] Editor no longer crashes when listing webcams whose name is missing or empty. Such cameras are now skipped safely \(with a warning in the Editor\).
    ([UUM-105563](https://issuetracker.unity3d.com/issues/editor-crashes-with-platformwebcamtexture-getdevicenames-when-a-virtual-camera-is-present-and-friendlyname-property-is-deleted-from-registry))




## Package changes in 2022.3.65f1

## Packages updated

- com.unity.inputsystem: [1.14.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.14//changelog/CHANGELOG.html) to [1.14.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.14//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.14.3](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html) to [1.15.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.15//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.13//changelog/CHANGELOG.html) to [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.13//changelog/CHANGELOG.html)

- com.unity.ai.navigation: [1.1.6](https://docs.unity3d.com/Packages/com.unity.ai.navigation@1.1//changelog/CHANGELOG.html) to [1.1.7](https://docs.unity3d.com/Packages/com.unity.ai.navigation@1.1//changelog/CHANGELOG.html)

- com.unity.services.levelplay: [8.6.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.6//changelog/CHANGELOG.html) to [8.10.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html)