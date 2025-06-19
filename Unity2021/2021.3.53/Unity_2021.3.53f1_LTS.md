# Unity 2021.3.53f1 LTS
Published at Wed, 18 Jun 2025 05:11:24 GMT  
https://unity.com/releases/editor/whats-new/2021.3.53

# Known Issues in 2021.3.53f1

- : Garbage Collector memory leak when allocating and deallocating memory in Web builds
    ([UUM-86352](https://issuetracker.unity3d.com/issues/garbage-collector-memory-leak-when-allocating-and-deallocating-memory-in-web-builds))

- : Graphics.RenderMeshIndirect does not issue multi-draw rendering commands when using a graphics API capable of multi-draw commands
    ([UUM-91617](https://issuetracker.unity3d.com/issues/graphics-dot-rendermeshindirect-does-not-issue-multi-draw-rendering-commands-when-using-a-graphics-api-capable-of-multi-draw-commands))

- : Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))



# 2021.3.53f1 Release Notes

## Changes

- Build Pipeline: Build Pipeline: Allow building AssetBundles with both the DisableTypeTree and StripUnityVersion flags. Fix the ability to load these AssetBundles in the Runtime.
    ([UUM-102575](https://issuetracker.unity3d.com/issues/an-error-is-thrown-when-building-assetbundles-with-disablewritetypetree-and-stripunityversion-flags))

- XR: Updated com.unity.xr.openxr package version to 1.15.0-pre.2.



## Fixes

- 2D: Fixed normal map preview in Sprite Editor Window's Secondary Texture module.
    ([UUM-99022](https://issuetracker.unity3d.com/issues/normal-maps-are-rendered-differently-in-sprite-editor-when-compared-to-the-inspector-preview))

- Android: Fixed AndroidJNI.ToBooleanArray not returning 0 when null.
    ([UUM-90092](https://issuetracker.unity3d.com/issues/android-androidjni-dot-tobooleanarray-returns-a-random-non-zero-value-instead-of-intptr-dot-zero-when-the-method-argument-is-null))

- iOS: Fixed QualitySettings handling \(when AA is involved\) in Split View.
    ([UUM-61559](https://issuetracker.unity3d.com/issues/ios-game-view-resolution-is-altered-when-changing-between-quality-levels-that-have-a-different-anti-aliasing-setting-on-ipad-with-split-view-active))

- Package Manager: Fixed an issue where installing a git package using Git LFS would not work with Git LFS 3.6.0 and higher.
    (UUM-91342)

- Package Manager: Make GetPatckagesPath thread/serialization safe.
    (UUM-104998)




## Package changes in 2021.3.53f1

## Packages updated

- com.unity.scriptablebuildpipeline: [1.22.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html) to [1.22.5](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html)