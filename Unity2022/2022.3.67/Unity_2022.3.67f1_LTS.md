# Unity 2022.3.67f1 LTS
Published at Thu, 25 Sep 2025 09:30:33 GMT  
https://unity.com/releases/editor/whats-new/2022.3.67f1

# Known Issues in 2022.3.67f1

- AI Navigation Core: NavMeshSurface ignores convex Mesh Colliders when using Physics Colliders
    ([UUM-102676](https://issuetracker.unity3d.com/issues/navmeshsurface-ignores-convex-mesh-colliders-when-using-physics-colliders))

- Audio Authoring: Audio Low Pass Filter isn't working when enabled after entering Play Mode or in Player via Script
    ([UUM-114268](https://issuetracker.unity3d.com/issues/audio-low-pass-filter-isnt-working-when-enabled-after-entering-play-mode-or-in-player-via-script))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DirectX12: The Player hangs when unloading a scene using the UnloadUnusedAssets() method
    ([UUM-79718](https://issuetracker.unity3d.com/issues/the-player-hangs-when-unloading-a-scene-using-the-unloadunusedassets-method))

- Video: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)

- Vulkan:  Artifacts appear in the Player when using Screen Space shadows with orthographic camera
    ([UUM-116048](https://issuetracker.unity3d.com/issues/vulkan-artifacts-appear-in-the-player-when-using-screen-space-shadows-with-orthographic-camera))

- Vulkan: Crashes in the wild on Vulkan in CreateDepthSurfaceImpl 
    ([UUM-114531](https://issuetracker.unity3d.com/issues/crashes-in-the-wild-on-vulkan-in-createdepthsurfaceimpl))



# 2022.3.67f1 Release Notes

## Improvements

- Android: Added an option to be able to force the use of the internal storage for persistent and cache files.

- GI: Changed behavior of light probe loading such that, when unloading the last scene that contains light probes, you don't need to call LightProbes.Tetrahedralize\(\) to apply the changes anymore.
    ([UUM-116318](https://issuetracker.unity3d.com/issues/baked-gi-loaded-by-loadscene-call-with-additive-mode-is-not-cleaned-up-when-unloading-the-scene))

- iOS: Added support for CAMetalDisplayLink. It is enabled by default on ios \(when built with xcode15+ and run ios17+\). It can be overriden at runtime by tweaking/overriding \[UnityAppController shouldUseMetalDisplayLink\] method. By default it is disabled on tvos, since most of them are slow, and failing to catch up with target FPS \(on complex scenes\) will result in confusing GPU hang messages.
    ([UUM-66493](https://issuetracker.unity3d.com/issues/ios-framerate-drops-when-screen-is-touched-on-promotion-devices))



## Fixes

- 2D: Added warning when Sprite Outline is set to beyond the boundary of Sprite.
    ([UUM-107991](https://issuetracker.unity3d.com/issues/textures-from-other-sprites-in-the-assets-leak-into-sprite-renderer-sprites-when-sprite-atlas-v2-is-used))

- 2D: Fixed case where crash on BlockMask::FillSpriteData when building the Android Player.
    ([UUM-112926](https://issuetracker.unity3d.com/issues/crash-on-blockmask-fillspritedata-when-building-the-android-player))

- 2D: Fixed default name for Light2D on game object creation.
    ([UUM-116587](https://issuetracker.unity3d.com/issues/default-name-of-manually-created-global-light-2d-gameobject-differs-from-the-one-included-in-the-initial-project-scene))

- 2D: Fixed Light Batching Debugger constantly refreshing list to 0.
    ([UUM-116583](https://issuetracker.unity3d.com/issues/lights-in-batch-keep-resetting-to-0-in-the-light-batching-debugger-when-a-new-gameobject-is-created-and-the-mouse-cursor-is-hovered-over-the-inspector-window))

- 2D: Fixed Light Batching Debugger UI constantly refreshing.
    (UUM-101919)

- Android: Forward AKEYCODE_MEDIA_PLAY_PAUSE, AKEYCODE_MEDIA_REWIND, AKEYCODE_MEDIA_FAST_FORWARD to input system Keyboard device. See https://github.com/Unity-Technologies/InputSystem/pull/2212/files for more details.
    ([UUM-113004](https://issuetracker.unity3d.com/issues/android-tv-some-of-the-remote-controls-not-detected-with-inputsystem-dot-devices))

- Android: When input field is hidden, text input no longer introduces previously deleted characters when using Vietnamese keyboard on certain devices.
    ([UUM-110122](https://issuetracker.unity3d.com/issues/vietnamese-keyboard-inputs-duplicate-symbols-in-android-player-when-hide-mobile-input-is-turned-on-for-a-text-field))

- Build Pipeline: Fixed issue where build report output paths are incorrect for asset bundle build.
    (UUM-116222)

- Editor: Check duplication for both customer and built-in tags in TagManager.
    ([UUM-99990](https://issuetracker.unity3d.com/issues/no-error-notification-is-displayed-when-creating-a-tag-with-an-already-existing-name))

- Editor: Fixed Awaitables that use main thread affinity logic for continuations so they are not hanging when paused in play mode.
    (UUM-110950)

- Graphics: Fixed Cubemap mipmaps display differently between Editor and Player when using custom mipmaps.
    ([UUM-104071](https://issuetracker.unity3d.com/issues/cubemap-mipmaps-display-differently-between-editor-and-player-when-using-custom-mipmaps))

- Graphics: Fixed MeshFilter excessively logging SendMessage warnings when used in Prefab.
    ([UUM-114459](https://issuetracker.unity3d.com/issues/sendmessage-warning-is-thrown-when-selecting-a-prefab))

- Graphics: Fixed Vulkan Validation error in vkQueueSubmit.
    (UUM-110090)

- iOS: Improved keyboard input field toolbar positioning by using inputAccessoryView, especially for floating keyboards.
    (UUM-100139)

- macOS: Added a warning dialog to alert users that all files will be deleted when building Apple platforms using the Replace option.<br>
    Added restricted directories when building Apple platforms.
    ([UUM-109815](https://issuetracker.unity3d.com/issues/files-in-the-target-folder-are-deleted-without-a-proper-warning-when-building-an-ios-project))

- macOS: Fixed mouse delta spike when cursor is set to the center of the screen.
    ([UUM-112550](https://issuetracker.unity3d.com/issues/the-camera-abruptly-jumps-after-resuming-the-game-when-the-mouse-is-moved-slightly))

- Package: Version Control: Fixed obsolete references to TreeViewState.
    (VCS-1007414)

- Particles: Fixed jittering of particle editor when the window is made too small.
    ([UUM-105164](https://issuetracker.unity3d.com/issues/particle-effect-window-tab-slider-is-jittery-and-not-smooth-when-resizing-the-docked-particle-effect-window))

- SRP Core: Fixed an Issue where the MaterialUpgrader in URP wouldnt enable Alpha Clipping on Materials that started out using Render Mode Cutout.
    ([UUM-99709](https://issuetracker.unity3d.com/issues/urp-material-upgrade-utility-does-not-enable-alpha-clipping-when-material-had-rendering-mode-set-to-cutout))

- UI Toolkit: Fixed scale and crop VectorImage clipping issue.
    ([UUM-104608](https://issuetracker.unity3d.com/issues/image-is-distorted-when-visualelement-is-scaled-and-scale-mode-set-to-scale-and-crop))

- Version Control: Fixed the error that was thrown when the "Configure Unity Version Control" button is pressed in the Build Automation settings in Build Profiles.
    ([UUM-115391](https://issuetracker.unity3d.com/issues/failed-to-open-uvcs-window-error-is-thrown-when-the-configure-unity-version-control-button-is-pressed-in-the-build-automation-settings-in-build-profiles))

- VFX Graph: Fixed usability when setting prewarm values in visual effect asset inspector
    ([UUM-114276](https://issuetracker.unity3d.com/issues/setting-the-the-prewarm-delta-time-to-the-smallest-value-always-sets-the-prewarm-step-count-to-the-different-random-values))




## Package changes in 2022.3.67f1

## Packages updated

- com.unity.collab-proxy: [2.9.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.9//changelog/CHANGELOG.html) to [2.9.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.9//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.36](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.37](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.mobile.notifications: [2.4.1](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) to [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- com.unity.services.vivox: [16.6.2](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.6//changelog/CHANGELOG.html) to [16.7.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.7//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.5.2](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) to [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.memoryprofiler: [1.1.8](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.14//changelog/CHANGELOG.html) to [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.14//changelog/CHANGELOG.html)