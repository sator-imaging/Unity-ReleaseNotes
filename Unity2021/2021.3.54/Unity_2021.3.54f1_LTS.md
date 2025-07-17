# Unity 2021.3.54f1 LTS
Published at Tue, 15 Jul 2025 14:38:16 GMT  
https://unity.com/releases/editor/whats-new/2021.3.54

# Known Issues in 2021.3.54f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Graphics Device Features: Graphics.RenderMeshIndirect does not issue multi-draw rendering commands when using a graphics API capable of multi-draw commands
    ([UUM-91617](https://issuetracker.unity3d.com/issues/graphics-dot-rendermeshindirect-does-not-issue-multi-draw-rendering-commands-when-using-a-graphics-api-capable-of-multi-draw-commands))



# 2021.3.54f1 Release Notes

## Improvements

- Documentation: Added keyboard support for copying code examples.

- DX12: Set ID3D12GraphicsCommandList::IASetVertexBuffers once instead of several times in a loop inside GfxDeviceD3D12Base::DrawBuffersCommon.
    (UUM-109282)



## Changes

- XR: Updated com.unity.xr.openxr package version to 1.15.0.



## Fixes

- Android: Enforcing to use Streaming Assets extensions for noCompress string in Android Gradle project to avoid problem with too many entries in the list, which may cause Gradle build fail.
    ([UUM-105133](https://issuetracker.unity3d.com/issues/android-build-fails-when-streamingassets-contains-998-or-more-files))

- Android: Fixed Integer input field not allowing negative integers to be entered \(on non-tmp text fields\).
    ([UUM-85618](https://issuetracker.unity3d.com/issues/android-the-symbol-is-not-allowed-to-be-entered-when-entering-a-negative-number-in-an-inputfield-when-the-content-type-is-set-to-integer-number))

- Burst: Fixed that player builds using IL2CPP on Linux would have truncated stacktraces if Burst was in the callstack.
    ([BUR-2858](https://issuetracker.unity3d.com/issues/linux-truncated-stack-traces-when-logging-from-managed-code-in-burst))

- Editor: Fixed Cursor.visible ignoring CursorLockMode.Locked.
    ([UUM-85853](https://issuetracker.unity3d.com/issues/mouse-pointer-remains-visible-on-screen-when-cursor-dot-lockstate-is-set-to-cursorlockmode-dot-locked-and-cursor-dot-visible-gets-set-to-true-in-update))

- Editor: Fixed IMGUI EditorGUIUtility.labelWidth value being changed by the Scene View UI. This could impact other windows drawn afterwards.
    ([UUM-110450](https://issuetracker.unity3d.com/issues/editorguilayout-dot-toggle-clickable-area-is-shifted-when-using-built-in-render-pipeline))

- Editor: Fixed implicit truncation shader warnings when using the multiplayer VR template.
    (UUM-84269)

- Editor: Removed the "Check for Updates" window.
    ([UUM-102388](https://issuetracker.unity3d.com/issues/check-for-updates-fails-to-connect-to-update-server))

- Graphics: Fixed a validation warning on DirectX by changing the fake input layout format.
    ([UUM-105001](https://issuetracker.unity3d.com/issues/a-vertex-stream-with-a-stride-of-1-is-bound-to-the-gpu-in-player-when-mesh-is-compressed))

- XR: Fixed an issue where the XrDisplaySubsystem tries to destroy textures that are still being used by other processes. This fix uses FinishRendering\(\) to block the simulation thread until those resources are no longer in use before trying to destroy them.
    (UUM-109086)

- XR: Fixed and issue where deployed URP Quest Applications throw Vulkan Errors on App Exit.
    (UUM-109083)




## Package changes in 2021.3.54f1

## Packages updated

- com.unity.addressables: [1.24.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.24//changelog/CHANGELOG.html) to [1.25.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.25//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.21](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.23](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.mobile.notifications: [2.4.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) to [2.4.1](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- com.unity.postprocessing: [3.4.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.4//changelog/CHANGELOG.html) to [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- com.unity.services.vivox: [16.6.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.6//changelog/CHANGELOG.html) to [16.6.2](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.6//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.14.3](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html) to [1.15.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.15//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.services.levelplay@8.10.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html)