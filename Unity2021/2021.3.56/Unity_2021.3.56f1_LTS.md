# Unity 2021.3.56f1 LTS
Published at Wed, 03 Sep 2025 11:26:12 GMT  
https://unity.com/releases/editor/whats-new/2021.3.56f1

# Known Issues in 2021.3.56f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))



# 2021.3.56f1 Release Notes

## Features

- Version Control: Added a new view to control labels.

- Version Control: Added empty states for different scenarios.

- Version Control: Added extra icons for known Unity file extensions.

- Version Control: Added the diff panel in the branches view.

- Version Control: Added tutorial link for Smart Locks in empty state for locks view.

- Version Control: Added Version Control actions to sub scenes menu in the hierarchy view.

- Version Control: Added Version Control actions to the scene header menu in the hierarchy view.

- Version Control: Enriched scene assets in the hierarchy view with status overlay icon.

- Version Control: Enriched sub scene assets in the hierarchy view with status overlay icon.

- Version Control: Implemented double-click action for pending changes view.

- Version Control: Implemented double-click action for the diff panel.

- Version Control: Implemented double-click action for the history view.

- Version Control: Improved checkout speed for thousands of files.

- Version Control: New feature to inform users about available updates in the package.

- Version Control: New feature to recommend to enable Manual Checkout for Unity Assets when there are Lock Rules configured for the project.

- Version Control: Updated all usages of TreeView to the new generic version in Unity 6000.2.



## Fixes

- 2D: Fixed Blurry and Stretched Light Type Icons in Global Light 2D Inspector.
    (UUM-111256)

- Editor: Fixed Awaitables that use main thread affinity logic for continuations so they are not hanging when paused in play mode.
    (UUM-110950)

- Editor: Fixed crash in GameObject::IsActiveIgnoreImplicitPrefab\(\).
    ([UUM-92622](https://issuetracker.unity3d.com/issues/crash-on-gameobject-isactiveignoreimplicitprefab-when-opening-a-specific-project))

- Editor: Updated 7-Zip to 25.01.

- Graphics: Fixed flickering of gpu instanced particle system in linux when using OpenGL.
    ([UUM-100915](https://issuetracker.unity3d.com/issues/linux-gpu-instanced-particles-rendering-issue-when-using-opengl))

- License: Bundle Licensing Client 1.17.2.
    (UUM-113543)

- Linux: Fixed Linux runtime window unexpectedly resizes to monitor dimensions when calling "Screen.SetResolution" function with hardcoded resolution matching current display's width or height.
    ([UUM-107466](https://issuetracker.unity3d.com/issues/linux-player-window-unexpectedly-resizes-to-monitor-dimensions-when-calling-screen-dot-setresolution-function-with-hardcoded-resolution-matching-current-displays-width-or-height))

- Networking: Updated our copy of MbedTLS to version 3.6.4 to address some security vulnerabilities.
    (UUM-114079)

- Package: Version Control: Fixed obsolete references to TreeViewState.
    (VCS-1007414)

- Version Control: Fixed aesthetic shaking issue when the package view is re-dimensioned.

- Version Control: Fixed an issue in the Login process not allowing to retry.
    (VCS-1007152)

- Version Control: Fixed an issue provoked by the auto-refresh of the Pending changes view.
    (VCS-1007328)

- Version Control: Fixed error message when clicking the 'Incoming changes' tab.
    (VCS-1006281)

- Version Control: Fixed some empty states that flickered when resizing the splitter or scrolling the table.
    (VCS-1007258)

- Version Control: Fixed the error 'EndLayoutGroup: BeginLayoutGroup must be called first' in different scenarios.
    (VCS-1006653)

- Version Control: Fixed undo shortcut for the PendingChanges view comments TextBox.

- Version Control: Updated LoadingSpinner to fix VisualElement.transform becoming obsolete.

- Version Control: Updated the Perforce client with P4 API 2021.2/2201121 to support Perforce P4 Cloud \(Helix Core Cloud\).
    ([UUM-113016](https://issuetracker.unity3d.com/issues/perforce-client-does-not-support-p4-helix-core-cloud-upgrade-to-version-2021-dot-2-slash-2201121-or-later))




## Package changes in 2021.3.56f1

## Packages updated

- com.unity.2d.aseprite: [1.1.9](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) to [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.addressables: [1.25.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.25//changelog/CHANGELOG.html) to [1.27.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.27//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.23](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.24](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.8.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.8//changelog/CHANGELOG.html) to [2.9.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.9//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.22.5](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html) to [1.23.0](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- com.unity.services.analytics: [6.0.3](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html) to [6.1.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.1//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.3//changelog/CHANGELOG.html) to [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.14//changelog/CHANGELOG.html) to [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.14//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk: [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.3//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk.tools: [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.3//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk.discovery: [1.0.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html)

- com.unity.services.levelplay: [8.10.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html) to [8.10.1](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html)