# Unity 2021.3.48f1 LTS
Published at Wed, 22 Jan 2025 09:38:12 GMT  
https://unity.com/releases/editor/whats-new/2021.3.48

# Known Issues in 2021.3.48f1

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))



# 2021.3.48f1 Release Notes

## Improvements

- Tests: Replaced the RecipeEngine.Modules.UnityCI dependency with UnityCI.Common.



## Fixes

- 2D: Fixed a sorting issue when a lower sorted mesh in a chunk are unable to fit in lower sorted Tile due to vertex or index limit, but are able to fit in a future higher sorted Tile.
    ([UUM-86981](https://issuetracker.unity3d.com/issues/isometric-tiles-are-flickering-and-overlapping-each-other-when-entering-play-mode-with-tilemap-renderer-mode-set-to-chunk))

- Android: Added dotnet webrequest feature for auto internet access permission.
    ([UUM-83355](https://issuetracker.unity3d.com/issues/android-error-nameresolutionfailure-when-internet-access-is-set-to-auto))

- Android: Added support for 16KB page sizes.

- Android: Bump Android Logcat Package to 1.4.4.

- Android: Fixed Android 15 keyboard Edit Field overlapping into cutoff area.
    ([UUM-77367](https://issuetracker.unity3d.com/issues/android-while-in-landscape-orientation-the-mobile-input-is-bigger-than-the-keyboard-when-building-for-android-15-beta-device))

- Android: Fixed issue where user installed certificates directly to an Android device wouldn't show up in the trusted_ca list.
    ([UUM-73839](https://issuetracker.unity3d.com/issues/android-error-curl-error-60-cert-verify-failed-certificate-is-not-correctly-signed-by-a-trusted-ca-unitytls-error-code-7-when-using-unitywebrequest-to-connect-to-the-server-with-a-self-signed-certificate))

- Android: Updated BundleTool to version 1.17.2.
    (UUM-90609)

- Asset Import: Fixed FBX import errors when importing models using the IndexToDirect format for normals.
    (UUM-74806)

- Audio: Fixed the 3D audio pan where right audio channel is completely cutoff at specific position.
    ([UUM-82903](https://issuetracker.unity3d.com/issues/the-right-audio-channel-completely-cuts-out-in-a-specific-position-with-the-3d-audio-when-the-audio-should-be-playing-from-both-speaker-in-that-position))

- Editor: Fixed CPU architecture in the plugin inspector resetting after applying changes.
    ([UUM-91926](https://issuetracker.unity3d.com/issues/changes-are-not-applied-when-selecting-platform-settings-for-plugins))

- Editor: Fixed CPU architecture in the plugin inspector resetting after applying changes.
    ([UUM-91926](https://issuetracker.unity3d.com/issues/changes-are-not-applied-when-selecting-platform-settings-for-plugins))

- Editor: Fixed the issue where licensing modals was printing an error message in Editor console:<br>
    "Layout update is struggling to process current layout".
    (UUM-86833)

- Graphics: Fixed a crash when importing a 16K normal map texture from gray scale.
    ([UUM-79322](https://issuetracker.unity3d.com/issues/crash-on-miniheightmap-extractnormalmap-00-when-16k-map-size-is-applied-with-create-from-grayscale-enabled))

- Graphics: Graphics: r8_srgb is now \(correctly\) marked as unsupported on intel mac.

- HDRP: Added clamp to HairAngleWorld to prevent nan from FastASin.
    ([UUM-72279](https://issuetracker.unity3d.com/issues/the-scene-view-flickers-when-moving-around-if-there-are-visible-hair-shaders))

- HDRP: Fixed an issue where cascade shadows and distance shadowmask were not blended properly.
    ([UUM-78038](https://issuetracker.unity3d.com/issues/theres-a-gap-between-the-last-cascade-and-the-baked-shadow-map-when-distance-shadowmasks-are-enabled))

- HDRP: Fixed wrong SSR when using a shader graph with a clear coat value of 0.
    ([UUM-84980](https://issuetracker.unity3d.com/issues/hdrp-clear-coat-materials-produce-screen-space-reflections-when-the-clear-coat-value-is-0-in-forward-only-lit-shader-mode))

- IL2CPP: Fixed fields of field types on serialized types being stripped in some cases.
    (UUM-90024)

- iOS: Fixed WebCamDevice.availableResolutions returning \[0;0\] on some devices.
    ([UUM-87792](https://issuetracker.unity3d.com/issues/ios-webcamdevice-dot-availableresolutions-returns-a-single-resolution-with-width-and-height-both-0-on-some-ios-devices))

- Linux: Fixed Input.mouseScrollDelta which could be inconsistent depending on the framerate.
    ([UUM-88049](https://issuetracker.unity3d.com/issues/linux-input-dot-mousescrolldelta-is-inconsistent-when-limiting-framerate))

- Mono: Added support for 16kb page sizes.

- Mono: Changed to prevent crash for MONO_TYPE_FNPTR cases in mono_field_get_value_object_checked.
    ([UUM-79025](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-using-the-default-equals-object-implementation-in-a-value-type-containing-a-function-pointer))

- Package Manager: Switch project when importing a full project asset package is fixed for mac users.
    ([UUM-87430](https://issuetracker.unity3d.com/issues/macos-switching-project-functionality-when-importing-a-complete-project-is-broken))

- Profiler: Fixed "System Used Memory" counter on Android potentially returning a value in Bytes instead of MB.

- Scripting: Fixed RuntimeInitializeOnLoad invoking the wrong method overload.
    ([UUM-53659](https://issuetracker.unity3d.com/issues/method-ran-with-runtimeinitializeonload-is-executed-last-when-running-an-overload-of-the-method-and-declaring-it-above-the-runtimeinitializeonload-method))

- Shadergraph: Fixed Shader warnings in URP ShaderGraph when using the Normal From Texture node.
    ([UUM-90053](https://issuetracker.unity3d.com/issues/shader-warnings-in-urp-shadergraph-when-using-the-normal-from-texture-node))

- Terrain: Changed to use hierarchical transform for tree representation matrix.
    ([UUM-78866](https://issuetracker.unity3d.com/issues/shadows-of-trees-painted-on-the-terrain-are-incorrectly-placed-when-the-lighting-is-baked))

- uGUI: Fixed incorrect sorting when viewing nested canvases in prefab mode.
    ([UUM-86544](https://issuetracker.unity3d.com/issues/nested-canvases-do-not-inherit-sorting-layer-of-parent-when-viewed-in-prefab-mode))

- UI Toolkit: Fixed layout issues that sometimes occurred between scene changes.
    ([UUM-87950](https://issuetracker.unity3d.com/issues/ui-elements-shrinking-misaligned-buttons-swapped-icons-or-incorrect-styles-when-rapidly-cycling-through-scenes-in-the-player))

- Universal RP: Universal RP: Fixed an issue where Camera view is not rendered on PowerVR Rogue GE8320 GPU'S if Shadows are enabled in URP Asset and Camera stack contains Overlay Camera's.
    ([UUM-82949](https://issuetracker.unity3d.com/issues/camera-view-is-not-rendered-on-powervr-rogue-ge8320-gpus-if-shadows-are-enabled-in-urp-asset-and-camera-stack-contains-overlay-cameras))

- Version Control: By default, the additional line breaks are not getting added to asset files when merging with UnityYAMLMerge with an extra option for user to get the line breaks.
    ([UUM-72934](https://issuetracker.unity3d.com/issues/additional-line-breaks-are-added-to-asset-files-when-merging-with-unityyamlmerge))

- Web: Fixed the mouse scrolling sensitivity in Web.
    ([UUM-84978](https://issuetracker.unity3d.com/issues/scrolling-on-a-default-scrollview-in-a-webgl-build-is-too-sensitive-when-compared-to-other-platform-builds-and-the-editor))

- XR: Fixed tracking origin mode validation logic.
    (UUM-90392)




## Package changes in 2021.3.48f1

## Packages updated

- com.unity.2d.aseprite: [1.1.6](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) to [1.1.7](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat: [1.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.performance.profile-analyzer: [1.2.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) to [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.4//changelog/CHANGELOG.html) to [2.5.1](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.13.2](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.13//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.11.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.11//changelog/CHANGELOG.html) to [1.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.12//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.microsoft.gdk.discovery@1.0.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.0//changelog/CHANGELOG.html)