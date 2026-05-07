# Unity 2022.3.76f1 LTS
Published at Wed, 06 May 2026 09:39:50 GMT  
https://unity.com/releases/editor/whats-new/2022.3.76f1

# Known Issues in 2022.3.76f1

- `Metal`: Game freezes after command buffer Timeout error
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: macOS stutters in a minimal project in the Editor in Play Mode
    ([UUM-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 2022.3.76f1 Release Notes

## Fixes

- `Asset Pipeline`: Updated Accelerator download links in Unity Manual to latest version.
    (EAD-2077)

- `Editor`: Fixed deadlock race condition when loading and unloading content files in the editor.
    (UUM-137677)

- `Editor`: Workaround crash when using stencil-only format on Mali GPUs with OpenGL ES.
    ([UUM-111344](https://issuetracker.unity3d.com/issues/android-crash-on-startup-when-depth-stencil-format-is-set-to-s8-uint))

- `Engine Diagnostics`: Added retry logic when uploading stack traces to Engine Diagnostics.
    (UUM-137962)

- `Engine Diagnostics`: Fixed Editor exceptions not being reported to Engine Diagnostics when CrashReportingSettings.captureEditorExceptions is enabled.
    ([UUM-136672](https://issuetracker.unity3d.com/issues/diagnostics-does-not-report-editor-exceptions-when-using-crashreportingsettings-dot-captureeditorexceptions))

- `Graphics`: Added a preventive measure to the JPEG decoder used by the "ImageConversion" class to prevent denial-of-service through the exploitation of the LJT-01-003 vulnerability. Unity will now automatically abort the decoding of JPEG files after decoding 1000 progressive scans.
    (UUM-129186)

- `Graphics`: Fixed a crash when using GPU skinning on Adreno devices.
    ([UUM-93243](https://issuetracker.unity3d.com/issues/crash-on-apigles-clearbuffersubdata-when-running-the-player-a-second-time-on-meta-quest-2))

- `Graphics`: Fixed an issue where MSAA CameraDepthTexture resizing was inconsistent when using the ScalableBufferManager in DX12, Metal, and legacy Vulkan device and Fixed an issue where an implicit truncation of vector type shader warning was thrown when building standalone or Android player.
    ([UUM-100367](https://issuetracker.unity3d.com/issues/android-ios-macos-inconsistent-cameradepthtexture-behavior-when-using-scalablebuffermanager-across-devices))

- `Graphics`: Fixed OpenGLES crash when invalid binding slot is passed for uniform buffer binding.
    (UUM-138897)

- `IL2CPP`: Corrected C++ warnings in libil2cpp code.
    (UUM-138294)

- `IL2CPP`: Fixed C++ pointer aliasing issue that could cause invalid code generation.
    ([UUM-132447](https://issuetracker.unity3d.com/issues/ios-stripping-issue-on-xcode-26-when-use-incremental-gc-is-disabled))

- `iOS`: Further improvements to UIScene lifecycle events - universal deep link handling, moved AbsoluteURL set earlier to not miss it in Awake\(\).
    (UUM-140746)

- `Networking`: Fixed a regression in MbedTLS that would result in TLS handshake errors when trying to download assets from the Asset Store from the package manager. Potentially other HTTPS endpoints could have been impacted by this regression.
    (UUM-141298)

- `Networking`: Updated MbedTLS to version 3.6.6 to address some \(minor and likely unexploitable\) security vulnerabilities.
    (UUM-140908)

- `Scripting`: Added main-thread guard in ScriptingCoverage::FilterRecordedMethods for thread safety during script reload.
    ([UUM-137724](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-disabling-the-debug-mode-with-the-code-coverage-enabled))




## Package changes in 2022.3.76f1

## Packages updated

- `com.unity.ide.rider`: [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.40](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.services.user-reporting`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) to [2.0.15](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- `com.unity.xr.core-utils`: [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) to [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.6//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) to [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html)