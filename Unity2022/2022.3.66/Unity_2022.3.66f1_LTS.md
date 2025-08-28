# Unity 2022.3.66f1 LTS
Published at Wed, 27 Aug 2025 08:35:21 GMT  
https://unity.com/releases/editor/whats-new/2022.3.66f1

# Known Issues in 2022.3.66f1

- 2D: Crash on "TransferPixelDataForMaskTemplate<_sprite_packing_char2>" when building for Android
    ([UUM-113215](https://issuetracker.unity3d.com/issues/crash-on-transferpixeldataformasktemplate-when-building-for-android))



# 2022.3.66f1 Release Notes

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



## Improvements

- Documentation: Clarified Application.PersistentDataPath documentation regarding MacOS Editor and MacOS Player paths.
    ([UUM-109747](https://issuetracker.unity3d.com/issues/macos-persistentdatapath-uses-old-path-when-built-compared-to-editor-play-mode))



## Fixes

- 2D: Fixed Blurry and Stretched Light Type Icons in Global Light 2D Inspector.
    (UUM-111256)

- 2D: Fixed Light2D issue on certain android devices.
    ([UUM-112716](https://issuetracker.unity3d.com/issues/android-light2d-with-light-type-spot-does-not-work-in-the-player-on-some-pixel-devices))

- Animation: Added an error to explain why AnimatorController states stop working when they reach a normalized time which is too large \(100,000+loops\).
    ([UUM-111056](https://issuetracker.unity3d.com/issues/animation-playback-and-transitions-start-being-erratic-when-state-normalized-time-gets-too-large-with-no-indication-what-is-the-problem))

- Audio: Fixed native memory of first loaded AudioClip being reported incorrectly in profiler.
    ([UUM-103201](https://issuetracker.unity3d.com/issues/allocated-memory-size-of-the-first-loaded-audioclip-is-much-higher-when-compared-to-the-rest-of-the-audioclips-memory-allocations))

- Editor: Fixed BRG raw buffer binding when no metadata.
    (UUM-110313)

- Editor: Fixed crash in GameObject::IsActiveIgnoreImplicitPrefab\(\).
    ([UUM-92622](https://issuetracker.unity3d.com/issues/crash-on-gameobject-isactiveignoreimplicitprefab-when-opening-a-specific-project))

- Editor: Fixed Editor hangs when cutting and pasting a Script to another folder during Play Mode.
    ([UUM-104031](https://issuetracker.unity3d.com/issues/editor-hangs-when-cutting-and-pasting-a-script-to-another-folder-during-play-mode))

- Editor: Fixed IME on Blur\(\) for UIToolkit.
    ([UUM-102003](https://issuetracker.unity3d.com/issues/textfield-in-uitoolkit-is-not-cleared-when-entering-korean-characters))

- Editor: Fixed Windows Editor command line launch issue when there is a -logfile arg with no log file path after.
    (UUM-112532)

- Editor: Mac: Fix issue that when loading a multi-monitor window layout on Mac then all Unity windows would be clamped to the same screen where the mouse is, instead of keeping their positions on the various monitors.
    ([UUM-110840](https://issuetracker.unity3d.com/issues/the-editor-window-does-not-appear-in-the-monitor-where-it-was-previously-closed-when-launching-the-editor))

- Editor: No longer assert in the Editor when calling InstantiateAsync on a prefab that contains a sub emitter.
    ([UUM-112023](https://issuetracker.unity3d.com/issues/error-persistentmanager-readobject-must-be-called-from-the-main-thread-when-using-async-addressable-loading-with-async-instantiation-for-prefabs-that-contain-a-particle-system-with-a-sub-emitter))

- Editor: Updated 7-Zip to 25.01.

- Graphics: Fixed crash after disconnecting an external display on Android.
    ([UUM-110456](https://issuetracker.unity3d.com/issues/android-crash-or-freeze-when-disconnecting-an-external-monitor-from-an-android-device))

- Graphics: Fixed flickering of gpu instanced particle system in linux when using OpenGL.
    ([UUM-100915](https://issuetracker.unity3d.com/issues/linux-gpu-instanced-particles-rendering-issue-when-using-opengl))

- Graphics: Fixed flickering of gpu instanced particle system when using OpenGL.
    ([UUM-98222](https://issuetracker.unity3d.com/issues/particle-systems-that-use-meshes-flicker-in-player-when-gpu-instancing-is-enabled-on-older-adreno-gpus))

- License: Bundle Licensing Client 1.17.2.
    (UUM-113543)

- Linux: Fixed Linux runtime window unexpectedly resizes to monitor dimensions when calling "Screen.SetResolution" function with hardcoded resolution matching current display's width or height.
    ([UUM-107466](https://issuetracker.unity3d.com/issues/linux-player-window-unexpectedly-resizes-to-monitor-dimensions-when-calling-screen-dot-setresolution-function-with-hardcoded-resolution-matching-current-displays-width-or-height))

- Networking: Updated our copy of MbedTLS to version 3.6.4 to address some security vulnerabilities.
    (UUM-114079)

- Package Manager: Removed retry option from PackageManager error during project creation.
    (UUM-111460)

- Particles: Fixed crash in trail geometry job.
    ([UUM-103773](https://issuetracker.unity3d.com/issues/crash-on-writeparticlelinevertex-when-particle-systems-are-rendered-in-a-specific-project))

- Particles: Prevent TempJob memory leak warning when playing Particle Systems in Edit mode.
    ([UUM-103773](https://issuetracker.unity3d.com/issues/crash-on-writeparticlelinevertex-when-particle-systems-are-rendered-in-a-specific-project))

- Profiler: Fixed invalid Mesh indices appearing in Memory Profiler metadata when read/write is disabled on standalone builds.
    ([UUM-107356](https://issuetracker.unity3d.com/issues/mesh-object-has-an-invalid-indices-value-in-a-memory-snapshot-of-a-player-build-when-the-read-slash-write-option-of-the-mesh-is-disabled))

- Scripting: Fixed ObjectPool clear timing in no domain reload environment.
    ([UUM-111093](https://issuetracker.unity3d.com/issues/objectpools-pool-is-destroyed-when-entering-play-mode-without-reloading-domain))

- Scripting: RoslynAnalyzersShouldNotReferenceNetStandard2_1 test instability fixed.
    (UUM-110692)

- uGUI: Disabled culling of empty Rects in the Editor to avoid false positives in the Scene View.
    ([UUM-100206](https://issuetracker.unity3d.com/issues/ui-elements-are-not-visible-on-certain-x-axis-positions-when-the-rotation-of-the-y-axis-is-90-or-90-degrees))

- uGUI: Nested canvases utilizing the Screen Space - Camera rendering mode will now fall back to sorting based on distance to their assigned camera. This fallback is used when Override Sorting is enabled, and only after first comparing sorting layer and sorting order values.
    ([UUM-100599](https://issuetracker.unity3d.com/issues/nested-canvases-with-the-same-order-in-layer-ignore-z-position-for-render-order-when-sharing-parent-canvas))

- uGUI: Revised an outdated editor warning that previously advised users to "clear the Packing tag." Since Packing tags are now obsolete, the message has been updated to reflect current best practices.
    ([UUM-103962](https://issuetracker.unity3d.com/issues/warning-about-an-obsolete-feature-appears-when-image-type-is-set-to-tiled))

- UI Toolkit: Fixed the IndexOutOfRangeException when redoing elements that came after the styled visual element in the UI Builder.
    ([UUM-109157](https://issuetracker.unity3d.com/issues/ui-builder-performing-redo-action-for-creating-a-nested-element-throws-nvalid-uxml-or-uss-system-dot-indexoutofrangeexception-and-corrupts-the-opened-document-causing-data-loss))

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

- Video: Fixed freezing video playback on Galaxy S25 and similar Android devices.
    ([UUM-111599](https://issuetracker.unity3d.com/issues/videoplayer-freezes-or-stops-on-certain-android-devices-when-enabling-and-disabling-the-video-multiple-times))

- Video: Fixed inconsistent imports of video files on MacOS.
    ([UUM-104688](https://issuetracker.unity3d.com/issues/new-artifact-generated-for-video-when-reimporting-with-identical-settings))

- VisionOS: Fixed crash when using WebCamTexture in visionOS builds.

- VisionOS: Fixed Xcode build failure when advertising APIs are used from scripts.
    ([UUM-113817](https://issuetracker.unity3d.com/issues/visionos-building-visionos-app-in-xcode-fails-with-error-adsupport-slash-asidentifiermanager-dot-h-file-not-found))




## Package changes in 2022.3.66f1

## Packages updated

- com.unity.2d.aseprite: [1.1.9](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) to [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.addressables: [1.25.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.25//changelog/CHANGELOG.html) to [1.27.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.27//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.23](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.24](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.8.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.8//changelog/CHANGELOG.html) to [2.9.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.9//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.14.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.14//changelog/CHANGELOG.html) to [1.14.2](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.14//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.22.5](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html) to [1.23.0](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- com.unity.services.analytics: [6.0.3](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html) to [6.1.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.1//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.3//changelog/CHANGELOG.html) to [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- com.unity.memoryprofiler: [1.1.6](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.8](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.13//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.14//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk: [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.3//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk.tools: [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.3//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk.discovery: [1.0.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html)

- com.unity.services.levelplay: [8.10.0](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html) to [8.10.1](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html)