# Unity 2022.3.73f1 LTS
Published at Wed, 04 Mar 2026 13:54:00 GMT  
https://unity.com/releases/editor/whats-new/2022.3.73f1

# Known Issues in 2022.3.73f1

- `Metal`: Game freezes after command buffer Timeout error
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: macOS stutters in a minimal project in the Editor in Play Mode
    ([UUM-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Video`: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)

- `Windows`: Player hangs when the "Run in Background" is enabled and active window is switched
    ([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))



# 2022.3.73f1 Release Notes

## Changes

- `Graphics`: Texture importing now strictly adheres to the supported formats in https://docs.unity3d.com/Documentation/Manual/ImportingTextures.html. Circumventing this by changing an image file's extension will no longer work. If a image file format is necessary, please file a feature request so we can look into properly supporting it.



## Fixes

- `Asset Bundles`: Fixed an issue where `AssetBundleUnloadOperation` allocations persist longer than expected and are not cleared until the next `GC.collect()`.
    (UUM-132703)

- `Editor`: Fixed an issue where EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture would interrupt compression to signed EAC formats too late in the process, leaving the texture in a broken state. Note that signed EAC formats are not supported for compression, this has been added to the API docs.

- `Editor`: Fixed an issue with EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture where it was possible to attempt to compress NPOT mipmapped textures to unsupported target formats. Additional details regarding this have been added to the API docs.
    ([UUM-129605](https://issuetracker.unity3d.com/issues/corrupted-mipmaps-are-generated-when-using-editorutility-dot-compresstexture-with-npot-textures))

- `iOS`: Keyboard UI adjusted to better fit with liquid glass.
    (UUM-133464)

- `Package Manager`: Url deep link using a upm package show the package selected if discoverable. Also show Add popup if a version is specified or if the package is not discoverable.
    (PAK-8687)




## Package changes in 2022.3.73f1

## Packages updated

- `com.unity.inputsystem`: [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) to [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) to [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) to [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) to [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.2.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) to [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html)