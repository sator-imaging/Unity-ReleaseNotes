# Unity 6000.0.67f1 LTS
Published at Wed, 04 Feb 2026 11:53:51 GMT  
https://unity.com/releases/editor/whats-new/6000.0.67f1

# Known Issues in 6000.0.67f1

- `6000.0.55f1,6000.3.0a4`: Crash on RaiseException when creating a multiplayer room while toggling UI
    ([UUM-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.1.0a2,6000.0.64f1`: Single-pass stereo rendering shows only Skybox when entering Play mode
    ([UUM-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.3.0b1,6000.0.65f1`: Editor freezes when QualitySettings.maxQueuedFrames is set to 1 and DX12 is used
    ([UUM-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `6000.5.0a4`: Profiler (Standalone) window doesn’t open
    ([UUM-131071](https://issuetracker.unity3d.com/issues/profiler-standalone-window-doesnt-open))

- `IL2CPP`: [iOS] [Android] External library generics fail during IL2CPP build
    ([UUM-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `iOS`:  Rendering freezes and UnityGfxDeviceWorker crash when Show Splash Screen is enabled and Project is built using Unity as a Library
    ([UUM-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- `Metal`:  Game freezes after command buffer Timeout error
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: macOS stutters in a minimal project in the Editor in Play Mode
    ([UUM-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Metal`: [iOS] Screen flashing after the iOS splash screen
    ([UUM-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- `Platform Audio`: [Windows] Crash on AudioManager::InitFMOD when performing various actions in the Editor
    ([UUM-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- : Editor memory leak when entering and exiting Play Mode in a blank URP project
    ([UUM-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))



# 6000.0.67f1 Release Notes

## Improvements

- `Shadergraph`: Added an issue where the swizzle node's input slot could end up in a bad state. Changed behavior so that the node's input and output slot always reflect the swizzle mask.
    ([UUM-120808](https://issuetracker.unity3d.com/issues/shader-graph-swizzle-node-input-slash-output-and-mask-update-incorrectly-after-undo))



## Fixes

- `2D`: Fixed issue where the user paints with an empty brush at any position and clears the Tile at \(0, 0, 0\).
    ([UUM-128709](https://issuetracker.unity3d.com/issues/painting-on-a-tilemap-erases-random-tile-when-an-empty-tile-was-selected-in-the-tilemap-palette))

- `2D`: Fixed issue with the Tile Palette window where a user can continue panning the Tile Palette window if the user's pointer leaves the Tile Palette window while panning and deactivates panning outside of the Tile Palette window.
    ([UUM-128466](https://issuetracker.unity3d.com/issues/tile-palette-grid-keeps-panning-when-the-mouse-click-is-released-outside-of-the-grid))

- `Documentation`: Fixed links to the Create a Profiler module page.

- `Editor`: Improved description of `worldToGUIPoint` and `OnDrawGizmos` API behavior.

- `Graphics`: Fixed crash with Metal Validation error on resolving MSAA memoryless depth buffer.
    (UUM-125478)

- `uGUI`: Fixed masking for UI elements orphaned by destroying a Canvas with overrideSorting=true.
    ([UUM-127287](https://issuetracker.unity3d.com/issues/canvas-masking-is-not-updated-when-destroying-the-canvas-component-with-an-overridesorting))

- `Version Control`: Fixed a compilation error caused by an invalid duplicated GUID in WaitForPendingOperations.cs.meta in 2.11.2.

- `Version Control`: Fixed accessing Editor internals directly on versions below Unity 6.3.




## Package changes in 6000.0.67f1

## Packages updated

- `com.unity.charactercontroller`: [1.4.1](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html) to [1.4.2](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html)

- `com.unity.animation.rigging`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html) to [1.4.1](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) to [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.ide.rider`: [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: [1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) to [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html)

- `com.unity.mobile.android-logcat`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) to [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) to [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) to [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- `com.unity.testtools.codecoverage`: [1.2.6](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.3//changelog/CHANGELOG.html)

- `com.unity.xr.hands`: [1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) to [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- `com.unity.profiling.systemmetrics.mali`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) to [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: [2.2.6](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) to [2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.9](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) to [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)