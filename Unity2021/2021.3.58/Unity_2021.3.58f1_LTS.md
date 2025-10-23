# Unity 2021.3.58f1 LTS
Published at Wed, 22 Oct 2025 09:39:32 GMT  
https://unity.com/releases/editor/whats-new/2021.3.58f1

# Known Issues in 2021.3.58f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))



# 2021.3.58f1 Release Notes

## Features

- Version Control: Added a new Editor Toolbar Button for Unity Version Control that lets you view project status, track changes, and perform key actions with one click.

- Version Control: Added Unity Version Control actions to the prefab and prefab variant header context menus.

- Version Control: Added Unity Version Control status icons to prefab assets in the hierarchy view in "Edit Mode".



## Changes

- Version Control: Improved overlay icons to align with the Unity Editor design. Added icons for "Controlled" and "Changed" items, removed the icon for "Private" items, and added a "Contains Changes" overlay for directories containing changes.



## Fixes

- Android: Enabled Vulkan support for Pixel 10.
    (UUM-120085)

- Player: The Player now restores correctly when using Alt+Tab in the Exclusive Fullscreen mode when using the DX12 Graphics API.
    ([UUM-67373](https://issuetracker.unity3d.com/issues/dx12-exclusive-full-screen-mode-player-window-sometimes-doesnt-restore-correctly-after-using-alt-plus-tab))

- uGUI: Fixed an editor bug where resizing the handle rect of a Slider and then performing an Undo causes its anchors to get reset.
    ([UUM-108288](https://issuetracker.unity3d.com/issues/slider-handle-becomes-a-different-size-than-default-when-undoing-change-to-the-width-parameter))

- Version Control: Fixed applying shelves when some files cannot be checked out due to exclusive checkout lock rules. These files are now applied as local changes instead of failing the whole operation.

- Version Control: Fixed incorrect tab name showing as "Unity.PlasticSCM.Editor.PlasticW" with no icon when upgrading a project to Unity 6.x.

- Version Control: Fixed issue in UnityYAMLMerge not able to read files under multibyte character paths.
    (UUM-119455)

- Version Control: Fixed the missing "Hide" contextual menu on the Unity Version Control button in the Unity 6.3 Toolbar.




## Package changes in 2021.3.58f1

## Packages updated

- com.unity.2d.animation: [7.0.12](https://docs.unity3d.com/Packages/com.unity.2d.animation@7.0//changelog/CHANGELOG.html) to [7.2.0](https://docs.unity3d.com/Packages/com.unity.2d.animation@7.2//changelog/CHANGELOG.html)

- com.unity.2d.common: [6.0.6](https://docs.unity3d.com/Packages/com.unity.2d.common@6.0//changelog/CHANGELOG.html) to [6.1.0](https://docs.unity3d.com/Packages/com.unity.2d.common@6.1//changelog/CHANGELOG.html)

- com.unity.2d.pixel-perfect: [5.0.3](https://docs.unity3d.com/Packages/com.unity.2d.pixel-perfect@5.0//changelog/CHANGELOG.html) to [5.1.0](https://docs.unity3d.com/Packages/com.unity.2d.pixel-perfect@5.1//changelog/CHANGELOG.html)

- com.unity.2d.psdimporter: [6.0.7](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@6.0//changelog/CHANGELOG.html) to [6.1.0](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@6.1//changelog/CHANGELOG.html)

- com.unity.2d.spriteshape: [7.0.7](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@7.0//changelog/CHANGELOG.html) to [7.1.0](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@7.1//changelog/CHANGELOG.html)

- com.unity.2d.tilemap.extras: [2.2.7](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@2.2//changelog/CHANGELOG.html) to [2.2.8](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@2.2//changelog/CHANGELOG.html)

- com.unity.2d.aseprite: [1.0.1](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.0//changelog/CHANGELOG.html) to [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.addressables: [1.19.19](https://docs.unity3d.com/Packages/com.unity.addressables@1.19//changelog/CHANGELOG.html) to [1.28.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.11](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.25](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.cinemachine: [2.8.9](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.8//changelog/CHANGELOG.html) to [2.10.3](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.2.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.2//changelog/CHANGELOG.html) to [2.10.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.10//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.26](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat: [1.3.2](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.3//changelog/CHANGELOG.html) to [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.mobile.notifications: [2.3.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.3//changelog/CHANGELOG.html) to [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- com.unity.performance.profile-analyzer: [1.2.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) to [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html)

- com.unity.postprocessing: [3.2.2](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.2//changelog/CHANGELOG.html) to [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- com.unity.probuilder: [5.2.0](https://docs.unity3d.com/Packages/com.unity.probuilder@5.2//changelog/CHANGELOG.html) to [5.2.4](https://docs.unity3d.com/Packages/com.unity.probuilder@5.2//changelog/CHANGELOG.html)

- com.unity.recorder: [3.0.3](https://docs.unity3d.com/Packages/com.unity.recorder@3.0//changelog/CHANGELOG.html) to [3.0.4](https://docs.unity3d.com/Packages/com.unity.recorder@3.0//changelog/CHANGELOG.html)

- com.unity.remote-config: [3.3.2](https://docs.unity3d.com/Packages/com.unity.remote-config@3.3//changelog/CHANGELOG.html) to [4.2.2](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html)

- com.unity.remote-config-runtime: [3.1.3](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@3.1//changelog/CHANGELOG.html) to [4.0.2](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@4.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.core: [12.1.13](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@12.1//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition: [12.1.13](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@12.1//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition-config: [12.1.13](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@12.1//changelog/CHANGELOG.html)

- com.unity.render-pipelines.universal: [12.1.13](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@12.1//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.20.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.20//changelog/CHANGELOG.html) to [1.23.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- com.unity.services.analytics: [5.0.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@5.0//changelog/CHANGELOG.html) to [6.1.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.1//changelog/CHANGELOG.html)

- com.unity.services.authentication: [2.7.2](https://docs.unity3d.com/Packages/com.unity.services.authentication@2.7//changelog/CHANGELOG.html) to [2.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@2.7//changelog/CHANGELOG.html)

- com.unity.services.core: [1.12.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.12//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.14//changelog/CHANGELOG.html)

- com.unity.services.friends: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html)

- com.unity.services.lobby: [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.1//changelog/CHANGELOG.html) to [1.2.2](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.2//changelog/CHANGELOG.html)

- com.unity.services.multiplay: [1.0.3](https://docs.unity3d.com/Packages/com.unity.services.multiplay@1.0//changelog/CHANGELOG.html) to [1.2.5](https://docs.unity3d.com/Packages/com.unity.services.multiplay@1.2//changelog/CHANGELOG.html)

- com.unity.services.qos: [1.2.1](https://docs.unity3d.com/Packages/com.unity.services.qos@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.qos@1.3//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.2.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html) to [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- com.unity.shadergraph: [12.1.13](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.1//changelog/CHANGELOG.html)

- com.unity.testtools.codecoverage: [1.2.4](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html) to [1.2.6](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html)

- com.unity.visualeffectgraph: [12.1.13](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@12.1//changelog/CHANGELOG.html)

- com.unity.visualscripting: [1.9.1](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) to [1.9.4](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- com.unity.xr.arcore: [4.2.9](https://docs.unity3d.com/Packages/com.unity.xr.arcore@4.2//changelog/CHANGELOG.html) to [4.2.10](https://docs.unity3d.com/Packages/com.unity.xr.arcore@4.2//changelog/CHANGELOG.html)

- com.unity.xr.arfoundation: [4.2.9](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@4.2//changelog/CHANGELOG.html) to [4.2.10](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@4.2//changelog/CHANGELOG.html)

- com.unity.xr.arkit: [4.2.9](https://docs.unity3d.com/Packages/com.unity.xr.arkit@4.2//changelog/CHANGELOG.html) to [4.2.10](https://docs.unity3d.com/Packages/com.unity.xr.arkit@4.2//changelog/CHANGELOG.html)

- com.unity.xr.arkit-face-tracking: [4.2.9](https://docs.unity3d.com/Packages/com.unity.xr.arkit-face-tracking@4.2//changelog/CHANGELOG.html) to [4.2.10](https://docs.unity3d.com/Packages/com.unity.xr.arkit-face-tracking@4.2//changelog/CHANGELOG.html)

- com.unity.xr.arsubsystems: [4.2.9](https://docs.unity3d.com/Packages/com.unity.xr.arsubsystems@4.2//changelog/CHANGELOG.html) to [4.2.10](https://docs.unity3d.com/Packages/com.unity.xr.arsubsystems@4.2//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.2.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.2//changelog/CHANGELOG.html) to [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.3.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.3//changelog/CHANGELOG.html) to [1.4.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.4//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [2.5.1](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.5//changelog/CHANGELOG.html) to [2.6.5](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.6//changelog/CHANGELOG.html)

- com.unity.xr.legacyinputhelpers: [2.1.10](https://docs.unity3d.com/Packages/com.unity.xr.legacyinputhelpers@2.1//changelog/CHANGELOG.html) to [2.1.12](https://docs.unity3d.com/Packages/com.unity.xr.legacyinputhelpers@2.1//changelog/CHANGELOG.html)

- com.unity.xr.management: [4.4.0](https://docs.unity3d.com/Packages/com.unity.xr.management@4.4//changelog/CHANGELOG.html) to [4.5.0](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html)

- com.unity.xr.oculus: [3.3.0](https://docs.unity3d.com/Packages/com.unity.xr.oculus@3.3//changelog/CHANGELOG.html) to [3.4.1](https://docs.unity3d.com/Packages/com.unity.xr.oculus@3.4//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.9.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.9//changelog/CHANGELOG.html) to [1.15.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.15//changelog/CHANGELOG.html)

- com.unity.transport: [1.4.0](https://docs.unity3d.com/Packages/com.unity.transport@1.4//changelog/CHANGELOG.html) to [1.5.0](https://docs.unity3d.com/Packages/com.unity.transport@1.5//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.7.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.7//changelog/CHANGELOG.html) to [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.14//changelog/CHANGELOG.html)

- com.unity.services.deployment: [1.2.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.2//changelog/CHANGELOG.html) to [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.4//changelog/CHANGELOG.html)

- com.unity.services.deployment.api: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.0//changelog/CHANGELOG.html) to [1.1.2](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.1//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.services.vivox@16.6.2](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.6//changelog/CHANGELOG.html)

- [com.unity.services.apis@1.1.0](https://docs.unity3d.com/Packages/com.unity.services.apis@1.1//changelog/CHANGELOG.html)

- [com.unity.dt.app-ui@1.0.2](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.0//changelog/CHANGELOG.html)

- [com.unity.services.moderation@1.0.1](https://docs.unity3d.com/Packages/com.unity.services.moderation@1.0//changelog/CHANGELOG.html)

- [com.unity.microsoft.gdk@1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html)

- [com.unity.microsoft.gdk.tools@1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html)

- [com.unity.microsoft.gdk.discovery@1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html)

- [com.unity.services.levelplay@8.10.1](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html)

**Packages deprecated**

- com.unity.purchasing.udp

**Pre-release packages added**

- [com.unity.xr.hands@1.5.0-pre.1](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.5//changelog/CHANGELOG.html)