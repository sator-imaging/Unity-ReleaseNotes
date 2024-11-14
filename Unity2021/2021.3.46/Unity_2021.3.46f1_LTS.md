# Unity 2021.3.46f1 LTS
Published at Wed, 13 Nov 2024 10:48:17 GMT  
https://unity.com/releases/editor/whats-new/2021.3.46

# Known Issues in 2021.3.46f1

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- iOS: iOS Simulator SDK is missing ARM64 Architecture support
    ([UUM-2238](https://issuetracker.unity3d.com/issues/ios-simulator-sdk-is-missing-arm64-architecture-support))

- Vulkan: [Android] Particles not rendered in the Player on some Android devices with Android 14
    ([UUM-68080](https://issuetracker.unity3d.com/issues/android-particles-not-rendered-in-the-player-on-some-android-devices-with-android-14))



# 2021.3.46f1 Release Notes

## Features

- License: Added XLTS entitlement check.



## Fixes

- Android: Editor.log will contain now entry on how the app is launched, for ex., adb.exe -s "FA7A31A08307" shell am start -a android.intent.action.MAIN -c android.intent.category.LAUNCHER -f 0x10200000 -S -n "com.DefaultCompany.GameActivity/com.unity3d.player.UnityPlayerActivity".
    (UUM-84923)

- Android: Fixed an issue where an Android app could freeze, if "Run in Background is false, if the app loses focus, and calls AudioSource::Stop when focus is lost.
    ([UUM-79804](https://issuetracker.unity3d.com/issues/android-the-player-freezes-when-playing-audio-on-focus-loss))

- Android: Ignore harmless warnings coming from sdkmanager - "Errors during XML parse:", "Additionally, the fallback loader failed to parse the XML.".

- Animation: Fixed animations with events at time "1" throw import warnings when using particular animation lengths.
    (UUM-79396)

- Animation: Fixed invalid default values of animated parameters in animator controller.
    ([UUM-73614](https://issuetracker.unity3d.com/issues/the-animation-curve-range-is-not-applied-properly))

- Editor: Added an 'Include all scripts' checkbox option to the export window allows users to choose whether to include all project scripts in the export list. This serves as the initial step before addressing the script dependency issue.
    ([UUM-46345](https://issuetracker.unity3d.com/issues/items-that-are-not-referenced-in-scene-are-selected-when-exporting-scenes-package))

- Editor: Disabled SRP batcher on the AssetImportWorker.
    ([UUM-77344](https://issuetracker.unity3d.com/issues/prefab-previews-in-the-project-window-sometimes-show-incorrectly))

- Editor: Editor: Fixes a crashing bug caused by a \(rare\) failure to initialize NetworkListManager COM interface.
    (UUM-83823)

- Editor: Fixed a bug that tree wireframe is incorrectly rendered outside of Scene view when editing a tree.
    ([UUM-82833](https://issuetracker.unity3d.com/issues/branch-editing-tools-draw-flashing-lines-with-black-backgrounds-in-editor-ui-windows))

- Editor: Fixed a crash when sequentially setting values in a managed reference array of strings.
    ([UUM-73968](https://issuetracker.unity3d.com/issues/crash-on-serializedproperty-custom-setstringvalueinternal-when-setting-serializedproperty-string-value))

- Editor: Fixed DeviceSimulator to implement Touch.rawPosition to return the starting position of the simulated touch contact.
    ([UUM-58248](https://issuetracker.unity3d.com/issues/touch-dot-rawposition-always-returns-00-when-clicking-or-dragging-anywhere-on-the-screen-in-the-play-mode))

- Editor: Fixed the over-clamping of delta time value applied to "unity_DeltaTime".
    ([UUM-35772](https://issuetracker.unity3d.com/issues/the-global-shader-variable-unity-deltatime-dot-x-value-does-not-match-the-time-dot-deltatime-value-when-compared-via-script))

- Editor: Libcurl used by Unity update to version 8.10.1.

- iOS: Fixed the character limit of the keyboard shown with TouchScreenKeyboard.Open.
    ([UUM-77509](https://issuetracker.unity3d.com/issues/ios-touchscreenkeyboard-allows-an-extra-character-when-characterlimit-is-set))

- Linux: Fixed screen resolution does not sync properly with the system's when changing system resolution during runtime.
    (UUM-64956)

- macOS: Fixed Application.targetFrameRate not being ignored when QualitySettings.vSyncCount &gt; 0.
    ([UUM-83568](https://issuetracker.unity3d.com/issues/vsynccount-is-ignored-on-macos-standalone-player))

- Networking: Fixed an issue where TLS connections would fail to be established after a certain time/number.
    ([UUM-83744](https://issuetracker.unity3d.com/issues/tlsexception-handshake-failed-error-code-unitytls-internal-error-error-when-a-lot-of-web-requests-are-sent-within-a-few-minutes))

- Shaders: Fixed a crash that could occur when a shadow caster pass is deleted due to shader errors.
    (UUM-82622)

- Shaders: Fixed compute shader compilation variant cache hits to be reported correctly in the editor log.
    ([UUM-75264](https://issuetracker.unity3d.com/issues/shader-cache-is-not-used-when-building-the-player-repeatedly))

- SpeedTree: Importer error for .st files when there are special characters in the file path.
    ([UUM-83783](https://issuetracker.unity3d.com/issues/speedtree-importer-fails-to-import-st-files-when-path-to-the-project-includes-a-special-character))

- Universal RP: Fixed a redundant empty line in a tooltip for Cast Shadows toggle in the URP Asset for Additional lights.
    ([UUM-83534](https://issuetracker.unity3d.com/issues/redundant-empty-space-on-tooltip-for-cast-shadows-option-for-additional-lights))

- URP: Stop spamming about c-buffer layout mispatch in GPU-instancing-enabled speed tree materials when enabling Rendering Layers.
    ([UUM-64059](https://issuetracker.unity3d.com/issues/speedtree-error-is-thrown-when-rendering-layers-for-lights-are-enabled))

- Version Control: UnityYAMLMerge is now able to open files when using long file paths on Windows.
    ([UUM-77908](https://issuetracker.unity3d.com/issues/unityyamlmerge-cannot-open-files-when-using-long-file-paths-on-windows))

- Web: Improved error message in abort handler.
    ([UUM-83890](https://issuetracker.unity3d.com/issues/webgl-unclear-error-when-gzip-compressed-data-or-webassembly-dont-have-correct-http-headers))

- WebGL: Fixed choppy video playback when using more than one Render Texture to play a video in Linear Color Space.
    ([UUM-79894](https://issuetracker.unity3d.com/issues/only-the-first-video-in-webgl-plays-smoothly-when-linear-color-space-is-used))

- XR: Fixed crash on Meta Quest 2 when using Vulkan.
    ([UUM-83776](https://issuetracker.unity3d.com/issues/crash-on-meta-quest-2-when-using-vulkan))




## Package changes in 2021.3.46f1

## Packages updated

- com.unity.2d.animation: [7.1.1](https://docs.unity3d.com/Packages/com.unity.2d.animation@7.1//changelog/CHANGELOG.html) to [7.1.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@7.1//changelog/CHANGELOG.html)

- com.unity.2d.common: [6.0.7](https://docs.unity3d.com/Packages/com.unity.2d.common@6.0//changelog/CHANGELOG.html) to [6.0.8](https://docs.unity3d.com/Packages/com.unity.2d.common@6.0//changelog/CHANGELOG.html)

- com.unity.2d.tilemap.extras: [2.2.7](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@2.2//changelog/CHANGELOG.html) to [2.2.8](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@2.2//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.31](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.34](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.mobile.notifications: [2.3.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.3//changelog/CHANGELOG.html) to [2.4.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- com.unity.services.deployment: [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.3//changelog/CHANGELOG.html) to [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.4//changelog/CHANGELOG.html)

- com.unity.services.deployment.api: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.0//changelog/CHANGELOG.html) to [1.1.2](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.1//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.services.moderation@1.0.1](https://docs.unity3d.com/Packages/com.unity.services.moderation@1.0//changelog/CHANGELOG.html)