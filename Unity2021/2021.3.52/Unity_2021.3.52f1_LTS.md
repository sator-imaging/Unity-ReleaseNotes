# Unity 2021.3.52f1 LTS
Published at Thu, 22 May 2025 11:54:25 GMT  
https://unity.com/releases/editor/whats-new/2021.3.52

# Known Issues in 2021.3.52f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Graphics Device Features: Graphics.RenderMeshIndirect does not issue multi-draw rendering commands when using a graphics API capable of multi-draw commands
    ([UUM-91617](https://issuetracker.unity3d.com/issues/graphics-dot-rendermeshindirect-does-not-issue-multi-draw-rendering-commands-when-using-a-graphics-api-capable-of-multi-draw-commands))



# 2021.3.52f1 Release Notes

## Improvements

- Graphics: Improved CopyTexture documentation \(warning about using Apply, mentions of the readability property, and general improvements\).



## Changes

- XR: The Unity XR SDK is no longer available as we have focused our investments towards OpenXR.

- XR: Updated com.unity.xr.openxr package version to 1.14.3.

- XR: Updated com.unity.xr.openxr package version to 1.15.0-pre.1.



## Fixes

- 2D: Fixed Sprite Editor Window settings text alignment in Preference Window.
    ([UUM-100716](https://issuetracker.unity3d.com/issues/misaligned-text-in-preferences-window-2d-animation-asperite-and-sprite-editor-preferences))

- Android: Fixed gradle-wrapper.properties not getting updated when modifying Gradle path in "Preferences -&gt; External Tools".
    (UUM-103233)

- Editor: Fixed a crash when 0 vertex skinmesh.
    ([UUM-93061](https://issuetracker.unity3d.com/issues/crash-on-skinnedmeshrenderer-updateskinnedmeshes-when-interacting-with-the-editor-in-a-specific-scene))

- Editor: Fixed a runtime crash when changing MSAA levels on OpenGL.

- Editor: Fixed dropdown rendering problem when opening from the Prefab Overrides Comparison window.
    (UUM-97349)

- Editor: Fixed freeze within cyclic compositions where internal depth limit was not being observed.
    ([UUM-49767](https://issuetracker.unity3d.com/issues/unity-freezes-when-opening-a-project))

- Graphics: Fixed a crash when using legacy image effects with Metal stereo rendering \(visionOS\).
    (UUM-103020)

- Graphics: Fixed the CustomRenderTexture Shader Properties array size warning.
    ([UUM-96096](https://issuetracker.unity3d.com/issues/property-exceeds-previous-array-size-2-vs-1-warnings-are-thrown-making-it-impossible-to-work-with-the-update-zones-of-the-customrendertexture-when-updating-the-script))

- Graphics: Replaced costly WMI videocontroller query.
    (UUM-102971)

- iOS: Changed Device.advertisingTrackingEnabled to report status from AppTrackingTransparency on iOS 14+.
    (UUM-101288)

- License: Updated error message when the Editor is attempted to be launched without an xLTS entitlement.
    (UUM-103361)

- Mono: Fixed Process.Start hangs on intel mac editors running on apple silicon.
    (UUM-101541)

- Networking: Updated our version of MbedTLS to 3.6.3 to address possible security vulnerabilities.
    (UUM-103889)

- Universal Windows Platform: Fixed audio playback when minimized, when Application.runInBackground is set to true.
    ([UUM-79675](https://issuetracker.unity3d.com/issues/audio-is-paused-when-the-player-is-minimized-and-application-dot-runinbackground-is-true))

- Version Control: Fixed false positive error showing in console if creating a workspace from the Hub with a version of the Unity Editor shipping with a default Version Control package older than version 2.7.1.

- Web: Corrected the name of the background image file in the output directory when using "Name Files as Hashes".
    ([UUM-96178](https://issuetracker.unity3d.com/issues/background-image-name-is-not-being-hashed-when-using-a-webgl-build-with-the-hashed-names-option))

- XR: Fixed issue where Quest Link would fail when using DX12 and single pass rendering.




## Package changes in 2021.3.52f1

## Packages updated

- com.unity.2d.animation: [7.1.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@7.1//changelog/CHANGELOG.html) to [7.2.0](https://docs.unity3d.com/Packages/com.unity.2d.animation@7.2//changelog/CHANGELOG.html)

- com.unity.2d.common: [6.0.8](https://docs.unity3d.com/Packages/com.unity.2d.common@6.0//changelog/CHANGELOG.html) to [6.1.0](https://docs.unity3d.com/Packages/com.unity.2d.common@6.1//changelog/CHANGELOG.html)

- com.unity.2d.psdimporter: [6.0.9](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@6.0//changelog/CHANGELOG.html) to [6.1.0](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@6.1//changelog/CHANGELOG.html)

- com.unity.2d.spriteshape: [7.0.7](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@7.0//changelog/CHANGELOG.html) to [7.1.0](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@7.1//changelog/CHANGELOG.html)

- com.unity.addressables: [1.19.19](https://docs.unity3d.com/Packages/com.unity.addressables@1.19//changelog/CHANGELOG.html) to [1.24.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.24//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.20](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.21](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.7.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.7//changelog/CHANGELOG.html) to [2.8.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.8//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.35](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.36](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat: [1.4.4](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) to [1.4.5](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.20.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.20//changelog/CHANGELOG.html) to [1.22.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.14.2](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html) to [1.14.3](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.12//changelog/CHANGELOG.html) to [1.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.13//changelog/CHANGELOG.html)

**Pre-release packages added**

- [com.unity.xr.openxr@1.15.0-pre.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.15//changelog/CHANGELOG.html)