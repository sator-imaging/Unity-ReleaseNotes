# Unity 2022.3.71f1 LTS
Published at Wed, 14 Jan 2026 15:42:53 GMT  
https://unity.com/releases/editor/whats-new/2022.3.71f1

# Known Issues in 2022.3.71f1

- 6000.0.64f1: [DX12] [Win11 ARM64] Machine crashes and restarts while trying to create a new project
    ([UUM-131104](https://issuetracker.unity3d.com/issues/dx12-win11-arm64-machine-crashes-and-restarts-while-trying-to-create-a-new-project))

- Metal:  Game freezes after command buffer Timeout error
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- Video: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)

- Vulkan: Crashes in the wild on Vulkan in CreateDepthSurfaceImpl 
    ([UUM-114531](https://issuetracker.unity3d.com/issues/crashes-in-the-wild-on-vulkan-in-createdepthsurfaceimpl))



# 2022.3.71f1 Release Notes

## Features

- Version Control: Added a cset by cset diff panel in the branches view.

- Version Control: Added a properties panel for the selected changeset/shelveset.

- Version Control: Added branch name\(s\) to the branch deletion dialog.

- Version Control: Added empty state in the history view.

- Version Control: Added specific empty states for Pending/Incoming Changes with filters.



## Improvements

- Graphics: Handle case where vulkan pipeline cache file could be corrupted and cause vkCreatePipelineCache to fail.



## Changes

- Editor: Changed previous fix to only happen in Editor outside of Play Mode.

- Version Control: Displayed progress indicator overlaying the view.

- Version Control: Implemented a "clever" truncation of paths.

- Version Control: Moved incoming and shelves notifications to the top bar.

- Version Control: Redesigned all the views and dialogs.

- Version Control: Redesigned the main panel to include a top breadcrumb.

- Version Control: Renamed toolbar dropdown to comply with a 120px max width limit in 6.5.

- Version Control: Show real indeterminate progress bar.

- Version Control: Updated deleted and moved overlay icons.



## Fixes

- Asset Bundles: Fixed cache-related crash on iOS when loading assets.
    (UUM-120877)

- Documentation: Fixed documentation on GetPixelBilinear describing the behavior in detail.
    (UUM-78472)

- Editor: Fixed potentiel heap-buffer-overflow when applying prefabs modifications.
    (UUM-131207)

- Editor: Fixed Unity Editor not detecting Unity Hub installation on Linux. The Editor now correctly checks both user-local \(~/.local/share/applications/\) and system-wide \(/usr/share/applications/\) locations for the Hub desktop file, and properly respects the XDG_DATA_HOME environment variable.
    (UUM-96606)

- Graphics: Fallback to main-thread skin matrix calculation for non-optimized SkinnedMeshRenderers when serialized with "m_DirtyAABB" set to true and "Update When Offscreen" is enabled.
    ([UUM-128966](https://issuetracker.unity3d.com/issues/crash-on-skinnedmeshrenderermanager-when-interacting-with-a-prefab-generated-with-uncombined-meshes-using-synty-sidekick-character-creator))

- Version Control: Added instructions on how to disable the deep scan of local packages when a timeout occurs and the setting is enabled.
    ([UUM-128080](https://issuetracker.unity3d.com/issues/unity-perforce-connection-is-extremely-slow-or-times-out-when-scan-local-packages-on-connect-is-enabled-in-version-control-while-the-project-has-many-local-packages))

- Version Control: Fixed Editor freezes/hangs on "Reloading Domain" when entering Play Mode.

- Version Control: Fixed Project Settings window moving to background when enabling or disabling Unity VCS in the Unity Version Control Settings.

- Version Control: Fixed the delete shortcut not working on macOS.

- Version Control: Fixed the menu references to Explorer instead of Finder when running on macOS.

- Version Control: Fixed Version control icon disappearing when opening a scene or switching Play Mode.




## Package changes in 2022.3.71f1

## Packages updated

- com.unity.burst: [1.8.26](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.10.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.10//changelog/CHANGELOG.html) to [2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- com.unity.services.vivox: [16.8.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.8//changelog/CHANGELOG.html) to [16.9.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.9//changelog/CHANGELOG.html)

- com.unity.timeline: [1.7.7](https://docs.unity3d.com/Packages/com.unity.timeline@1.7//changelog/CHANGELOG.html) to [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- com.unity.xr.management: [4.5.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) to [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.15.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.15//changelog/CHANGELOG.html) to [1.16.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.16//changelog/CHANGELOG.html)

- com.unity.cloud.draco: [5.4.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) to [5.4.2](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- com.unity.cloud.ktx: [3.6.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) to [3.6.2](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)