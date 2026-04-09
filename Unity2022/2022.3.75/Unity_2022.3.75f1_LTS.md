# Unity 2022.3.75f1 LTS
Published at Wed, 08 Apr 2026 06:21:50 GMT  
https://unity.com/releases/editor/whats-new/2022.3.75f1

# Known Issues in 2022.3.75f1

- `Metal`: Game freezes after command buffer Timeout error
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: macOS stutters in a minimal project in the Editor in Play Mode
    ([UUM-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 2022.3.75f1 Release Notes

## Features

- `Version Control`: Added "Add to Source Control" and "Undo Changes" actions for folders from the Project browser and Inspector.

- `Version Control`: Added a new Branch Explorer to visualize and navigate branches.

- `Version Control`: Added persistence for all splitter positions across window reloads and sessions.

- `Version Control`: Added support in the merge view to partially apply a shelve.

- `Version Control`: Added the F2 keyboard shortcut to rename branches and labels.



## Changes

- `Version Control`: Added changeset and label icons to the status bar.

- `Version Control`: Delayed workspace creation when opening projects from the Unity Hub.

- `Version Control`: Improved text field focus behavior across dialogs for more consistent keyboard workflows.

- `Version Control`: Improved the empty state in the Pending Changes view.

- `Version Control`: Prevented connecting a project to a different organization by mistake.

- `Version Control`: Updated new project initialization to perform a full initial checkin.

- `Version Control`: Updated the macOS hide shortcut to Cmd+Shift+H.



## Fixes

- `DX12`: Fixed missing resource barrier after resuming drawing to the render target previously bound as a compute shader SRV.
    (UUM-127520)

- `Graphics`: Make sure that builtinRP blit copy does output float4 color \(as opposed to fxed4, which is translated to half4 on metal, resulting in data truncation for u16 or f32 data\).
    ([UUM-128591](https://issuetracker.unity3d.com/issues/terrain-heightmap-loses-precision-on-android-and-ios-when-the-heightmap-texture-is-blitted-to-a-rendertexture-using-the-default-blit-shader))

- `IL2CPP`: Fixed invalid MethodsToPreserve entries for lambda expressions.
    ([UUM-124814](https://issuetracker.unity3d.com/issues/unity-cil-linker-fails-on-player-build-when-persistent-listeners-have-and-in-their-xml-attribute-names))

- `Input`: Fixed invalid long buffer pointer in IOHIDDevice_GetUsage.
    ([UUM-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))

- `iOS`: Bump iOS/tvOS minspec from 12.0 to 13.0.
    (UUM-136440)

- `iOS`: Fixed Application.deepLinkActivated not being invoked when the app was opened via a custom URL scheme or Universal Link while the app was already running, or in some cases when the app was launched from a cold start via a deep link.
    ([UUM-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `Physics`: Prevented stack overflow when raycasting on a `MeshCollider` with the `Use Fast Midphase` cooking option.
    ([UUM-110564](https://issuetracker.unity3d.com/issues/silent-crash-when-raycasting-on-a-specific-dense-mesh))

- `Version Control`: Fixed a layout exception when right-clicking Pending Changes in the side bar.

- `Version Control`: Fixed a NullReferenceException when opening history from a branch diff.

- `Version Control`: Fixed a potential NullReferenceException in the changeset-by-changeset diff panel.

- `Version Control`: Fixed and localized the Checkin dialog progress label.

- `Version Control`: Fixed blurry icons in the Explore Repositories window.

- `Version Control`: Fixed button capitalization in the Unity Version Control window to match Unity standards.

- `Version Control`: Fixed deprecated instanceID API usages for Unity 6.4 and later.

- `Version Control`: Fixed issues in the changeset-by-changeset diff from the branches view.

- `Version Control`: Fixed the branches context menu not opening when the table is empty.

- `Version Control`: Fixed the Checkin dialog not auto-focusing the comment field.

- `Version Control`: Fixed the labels context menu not opening when the table is empty.

- `Version Control`: Fixed the New Branch button failing when the current selection is a changeset or label.

- `Version Control`: Fixed the status bar turning gray after exiting Play Mode.

- `Version Control`: Fixed the Unity Version Control window during Create Workspace to refresh without requiring mouse movement.

- `Version Control`: Fixed validation messages alignment in the Unity Version Control window.

- `Video`: Fixed failure to play Video on specific mobile devices with Vulkan Graphics API.
    ([UUM-133914](https://issuetracker.unity3d.com/issues/video-player-renders-no-video-on-specific-devices-when-using-vulkan))




## Package changes in 2022.3.75f1

## Packages updated

- `com.unity.2d.aseprite`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) to [1.1.11](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- `com.unity.addressables`: [1.28.2](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) to [1.29.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.29//changelog/CHANGELOG.html)

- `com.unity.ads`: [4.16.4](https://docs.unity3d.com/Packages/com.unity.ads@4.16//changelog/CHANGELOG.html) to [4.17.0](https://docs.unity3d.com/Packages/com.unity.ads@4.17//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) to [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) to [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.postprocessing`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html) to [3.5.4](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [1.23.3](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) to [1.23.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) to [6.3.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.3//changelog/CHANGELOG.html)

- `com.unity.services.vivox`: [16.9.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.9//changelog/CHANGELOG.html) to [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) to [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) to [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: [5.4.2](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) to [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.6.2](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) to [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)