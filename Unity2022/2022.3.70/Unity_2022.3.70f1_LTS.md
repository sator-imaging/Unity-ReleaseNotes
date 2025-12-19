# Unity 2022.3.70f1 LTS
Published at Thu, 18 Dec 2025 09:10:22 GMT  
https://unity.com/releases/editor/whats-new/2022.3.70f1

# Known Issues in 2022.3.70f1

- Video: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)



# 2022.3.70f1 Release Notes

## Improvements

- iOS: Added workaround for ios calling metal displaylink callback recursively on some devices when loading webkit from the \[NSAttributedString initWithData:options:documentAttributes:error:\] call done in plugins inside unity playerloop.



## Changes

- iOS: Changed the way we present frame to make it more robust.

- iOS: Pause/unpause displaylink when going background/foreground.



## Fixes

- Animation: Fixed issue where Animator state normalized time would stop incrementing past a certain normalized time. Now, the state time will be guaranteed to increment \(or decrement\) to the next representable floating point number if the delta time is non-zero.
    (UUM-123305)

- Audio: Fixed bad link when using inspector reference for AudioSnapshot.
    ([UUM-120312](https://issuetracker.unity3d.com/issues/audio-mixer-snapshot-link-to-the-documentation-isnt-working))

- DX12: Fixed broken `IDXGISwapChain::GetFrameStatistics` with cpu-side time sampling.
    (UUM-107892)

- Editor: Asset Bundles: Fixed crash when you call UnloadAllAssetBundles and there are pending AssetBundle.UnloadAsync tasks.
    ([UUM-122776](https://issuetracker.unity3d.com/issues/crash-when-you-call-unloadallassetbundles-and-there-are-pending-assetbundle-dot-unloadasync-tasks))

- Editor: Fixed a bug where accessing an overlay's containerWindow could throw a NullRef Exception.
    ([UUM-127936](https://issuetracker.unity3d.com/issues/nullreferenceexception-occurs-when-accessing-containerwindow-on-a-scene-view-overlay))

- Graphics: Added tracking of memory going into Metal Buffers.
    (UUM-21519)

- Graphics: Fixed Grabpass does not work when the Render Target is set to Camera and specific Viewport values are set \(0,0.5,0.5,0.5\).
    ([UUM-113033](https://issuetracker.unity3d.com/issues/grabpass-does-not-work-when-the-render-target-is-set-to-camera-and-specific-viewport-values-are-set-00-dot-50-dot-50-dot-5))

- HDRP: Fixed custom pass buffers being the wrong size when switching XR On/Off.
    ([UUM-71748](https://issuetracker.unity3d.com/issues/xr-custom-pass-not-working-as-intended-with-single-pass-instanced-when-xr-is-initialized-after-runtime-start))

- iOS: Fixed crash when passing a null pointer as the 3rd argument `param` of `UnitySendMessage`.
    (UUM-126299)

- iOS: Fixed touch keyboard on iOS reporting it is visible after dismiss.
    ([UUM-121639](https://issuetracker.unity3d.com/issues/ios-the-touchscreenkeyboard-dot-visible-reports-true-when-the-on-screen-keyboard-is-hidden))

- Mono: Re-added support for Jetbrains Rider profiling, which had been temporarily removed with a recent security fix.
    ([UUM-126137](https://issuetracker.unity3d.com/issues/mono-profiling-in-jetbrains-rider-is-broken-as-a-result-of-october-3-2025-security-fix))

- Player: Restored shader stage information in a log message reported when compiling shader variants.
    ([UUM-125587](https://issuetracker.unity3d.com/issues/android-stage-information-is-not-logged-when-log-shader-compilation-is-enabled))

- Scripting: Passing a 0 detaTime into Mathf.SmoothDamp would cause a returned velocity of NaN \(0 distance / 0 time\). The returned velocity has been changed to pass back the same velocity that was passed in to the function.
    ([UUM-75577](https://issuetracker.unity3d.com/issues/velocity-is-set-to-nan-when-using-mathf-dot-smoothdamp))

- Shaders: Added word wrapping to the compute shader inspector kernel label field.
    ([UUM-126858](https://issuetracker.unity3d.com/issues/vfx-compute-shader-inspector-fields-are-spaced-far-from-their-labels))

- Shaders: When a standard material's render queue value is set out-of-bounds, clicking the log message that is printed to the console will now highlight the material that triggered it.
    ([UUM-110693](https://issuetracker.unity3d.com/issues/console-message-lacks-information-when-render-queue-is-changed-out-of-bounds-in-the-inspector))

- Universal Windows Platform: Fixed building for Universal Windows Platform when using Visual Studio 2026.
    ([UUM-127114](https://issuetracker.unity3d.com/issues/building-for-uwp-fails-with-visual-studio-2026))

- URP: Save URP asset before starting an asset bundle build.
    ([UUM-126809](https://issuetracker.unity3d.com/issues/urp-is-using-in-memory-assets-without-saving-them))

- Version Control: Fixed package files added by the provider callback are included in paths.
    ([UUM-103738](https://issuetracker.unity3d.com/issues/package-files-do-not-get-checked-out-in-perforce-when-the-project-includes-a-provider-callback))

- Version Control: UnityYAMLMerge tool was adding long path specifiers to the file paths passed to the fallback merge tools, causing p4Merge to fail.
    ([UUM-126068](https://issuetracker.unity3d.com/issues/unityyamlmerge-fails-to-merge-on-some-computers-when-some-specific-files-are-used))

- VisionOS: Fixed visionOS player crash when "Wait for managed debugger" is enabled in build profile.
    (UUM-128044)




## Package changes in 2022.3.70f1

## Packages updated

- com.unity.2d.animation: [9.2.1](https://docs.unity3d.com/Packages/com.unity.2d.animation@9.2//changelog/CHANGELOG.html) to [9.2.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@9.2//changelog/CHANGELOG.html)

- com.unity.2d.psdimporter: [8.1.1](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.1//changelog/CHANGELOG.html) to [8.1.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.1//changelog/CHANGELOG.html)

- com.unity.addressables: [1.28.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) to [1.28.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html)

- com.unity.ads: [4.4.2](https://docs.unity3d.com/Packages/com.unity.ads@4.4//changelog/CHANGELOG.html) to [4.16.4](https://docs.unity3d.com/Packages/com.unity.ads@4.16//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.25](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.26](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.15.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.15//changelog/CHANGELOG.html) to [1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html)

- com.unity.purchasing: [4.11.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.11//changelog/CHANGELOG.html) to [4.14.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.23.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) to [1.23.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- com.unity.services.analytics: [6.1.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.1//changelog/CHANGELOG.html) to [6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- com.unity.services.core: [1.14.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.14//changelog/CHANGELOG.html) to [1.16.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.16//changelog/CHANGELOG.html)

- com.unity.services.vivox: [16.7.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.7//changelog/CHANGELOG.html) to [16.8.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.8//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.7.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) to [1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- com.unity.asset-manager-for-unity: [1.7.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.7//changelog/CHANGELOG.html) to [1.9.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html)

- com.unity.cloud.ktx: [3.6.0](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) to [3.6.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.cloud.gltfast@6.14.1](https://docs.unity3d.com/Packages/com.unity.cloud.gltfast@6.14//changelog/CHANGELOG.html)