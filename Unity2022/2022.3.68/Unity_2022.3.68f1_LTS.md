# Unity 2022.3.68f1 LTS
Published at Thu, 23 Oct 2025 09:22:53 GMT  
https://unity.com/releases/editor/whats-new/2022.3.68f1

# Known Issues in 2022.3.68f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DirectX12: The Player hangs when unloading a scene using the UnloadUnusedAssets() method
    ([UUM-79718](https://issuetracker.unity3d.com/issues/the-player-hangs-when-unloading-a-scene-using-the-unloadunusedassets-method))

- Video: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)

- Visual Effects: Memory leak warnings are thrown when creating a Particle System GameObject
    ([UUM-113839](https://issuetracker.unity3d.com/issues/memory-leak-warnings-are-thrown-when-creating-a-particle-system-gameobject-2))

- Vulkan: Crashes in the wild on Vulkan in CreateDepthSurfaceImpl 
    ([UUM-114531](https://issuetracker.unity3d.com/issues/crashes-in-the-wild-on-vulkan-in-createdepthsurfaceimpl))



# 2022.3.68f1 Release Notes

## Features

- Version Control: Added a new Editor Toolbar Button for Unity Version Control that lets you view project status, track changes, and perform key actions with one click.

- Version Control: Added Unity Version Control actions to the prefab and prefab variant header context menus.

- Version Control: Added Unity Version Control status icons to prefab assets in the hierarchy view in "Edit Mode".



## Improvements

- Android: Added an option to Player Settings allowing to disable the automatic creation of a Presentation for rendering camera targeting Display 2 if a presentation display is detected.



## API Changes

- iOS: Added: Added iPhone 17 device generation enums and screen cutouts.



## Changes

- Version Control: Improved overlay icons to align with the Unity Editor design. Added icons for "Controlled" and "Changed" items, removed the icon for "Private" items, and added a "Contains Changes" overlay for directories containing changes.



## Fixes

- AI: A Navigation `Raycast()` was freezing the game when passing through very small NavMesh polygons created by NavMesh Obstacles that carve.
    ([UUM-110863](https://issuetracker.unity3d.com/issues/editor-freezes-after-some-time-when-using-navmeshquery-raycast))

- Android: Enabled Vulkan support for Pixel 10.
    (UUM-120085)

- Android: Fixed possibly missed events in UAAL scenario when calls were made right after instantiating the UnityPlayer.
    (UUM-116775)

- Animation: Fixed issue where transitions with normalized duration and calls to Animator.CrossFade had incorrect duration if the animator speed was not 1 or -1.
    ([UUM-109060](https://issuetracker.unity3d.com/issues/animator-dot-crossfade-normalizedduration-results-in-scaled-clip-advancement-when-animator-dot-speed-is-not-1-dot-0))

- Audio: Fixed OnAudioFilterRead not working when enabling/disabling component.
    ([UUM-114268](https://issuetracker.unity3d.com/issues/audio-low-pass-filter-isnt-working-when-enabled-after-entering-play-mode-or-in-player-via-script))

- Editor: Fixed unwrap crashing, when using bad "min object scale".
    ([UUM-112809](https://issuetracker.unity3d.com/issues/silent-crash-when-generating-lightmap-uvs-for-a-model-with-a-large-object-scale))

- Editor: Fixed Unwrapping.GenerateSecondaryUVSet when used with Mesh have baseVertex tweaked.
    ([UUM-109482](https://issuetracker.unity3d.com/issues/unwrapping-dot-generatesecondaryuvset-does-not-work-with-submeshes-when-they-have-offsets-on-basevertex))

- Editor: Removed the styling causing the misalignment with foldout headers in the prefab override comparison window.
    ([UUM-119442](https://issuetracker.unity3d.com/issues/prefab-source-and-override-content-bounds-are-misaligned))

- Editor: Report Editor architecture information.

- GI: Fixed a bug where the Renderer Light Probe Selection setting malfunctions when set to "Use Ambient Probe". Renderers outside the probe hull would, in fact, not use the ambient probe, but just get black SH data.
    ([UUM-96421](https://issuetracker.unity3d.com/issues/renderers-outside-light-probe-hull-use-incorrect-ambient-probe-values-when-renderer-light-probe-selection-is-set-to-use-ambient-probe-and-light-probes-on-mesh-is-set-to-blend-probes))

- Graphics: Fixed as issue in URP where screen space decals would not render with specific build configurations when using rendering layers.
    ([UUM-108756](https://issuetracker.unity3d.com/issues/decal-not-projected-on-top-of-a-lit-material-when-msaa-is-enabled-and-rendering-path-is-forward-or-forward-plus-in-a-standalone-build))

- Graphics: Fixed occasional null pointer access crash during shutdown.
    (UUM-121178)

- Graphics: Fixed Vulkan crash on Android while switching between scenes.
    ([UUM-82923](https://issuetracker.unity3d.com/issues/android-crash-on-atomicqueue-enqueue-atomicnode-star-plus-12-when-a-scene-transition-happens-in-the-player))

- HDRP: Fixed crash when playing video on a render texture with low-end GPUs.
    ([UUM-108627](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-playing-video-on-a-render-texture-with-low-end-graphics-devices))

- HDRP: Prevent CustomPass using camera depth if the injection point is set to AfterPostprocess. Show a warning in the CustomPass inspector if this configuration is present.
    ([UUM-79283](https://issuetracker.unity3d.com/issues/drawrendererescustompass-onpostprocess-only-draws-within-the-original-render-area-when-dynamic-resolution-is-enabled-and-graphics-api-is-set-to-directx12))

- iOS: Fixed extra repaint call on CADisplayLink.
    ([UUM-119142](https://issuetracker.unity3d.com/issues/ios-time-dot-deltatime-is-switching-between-9-dot-998583e-06-and-approximately-0-dot-01-seconds))

- Particles: Fixed memory leak related to ParticleSystem job fences.
    (UUM-113729)

- Player: The Player no longer becomes unresponsive after resolution switch in Exclusive Fullscreen mode when using the DX12 Graphics API.
    ([UUM-104762](https://issuetracker.unity3d.com/issues/the-player-becomes-unresponsive-after-resolution-switch-in-exclusive-fullscreen-mode-when-using-dx12-graphics-api))

- Player: The Player now restores correctly when using Alt+Tab in the Exclusive Fullscreen mode when using the DX12 Graphics API.
    ([UUM-67373](https://issuetracker.unity3d.com/issues/dx12-exclusive-full-screen-mode-player-window-sometimes-doesnt-restore-correctly-after-using-alt-plus-tab))

- uGUI: Fixed an editor bug where resizing the handle rect of a Slider and then performing an Undo causes its anchors to get reset.
    ([UUM-108288](https://issuetracker.unity3d.com/issues/slider-handle-becomes-a-different-size-than-default-when-undoing-change-to-the-width-parameter))

- Universal RP: Added a missing shader include in Shadows.hlsl, so that the function LerpWhiteTo\(\) is included correctly.
    ([UUM-99304](https://issuetracker.unity3d.com/issues/the-lerpwhiteto-missing-function-displays-an-error-when-the-shadows-dot-hlsl-shader-is-included-in-a-shader-file))

- URP: Fixed screen space shadows artifacts when using Vulkan on some Android devices.
    ([UUM-116048](https://issuetracker.unity3d.com/issues/vulkan-artifacts-appear-in-the-player-when-using-screen-space-shadows-with-orthographic-camera))

- Version Control: Fixed applying shelves when some files cannot be checked out due to exclusive checkout lock rules. These files are now applied as local changes instead of failing the whole operation.

- Version Control: Fixed incorrect tab name showing as "Unity.PlasticSCM.Editor.PlasticW" with no icon when upgrading a project to Unity 6.x.

- Version Control: Fixed issue in UnityYAMLMerge not able to read files under multibyte character paths.
    (UUM-119455)

- Version Control: Fixed the missing "Hide" contextual menu on the Unity Version Control button in the Unity 6.3 Toolbar.

- VFX Graph: Fixed Parallax Occlusion Mapping usage in SG.
    ([UUM-110541](https://issuetracker.unity3d.com/issues/parallax-occlusion-mapping-shadergraph-node-does-not-work-correctly-with-vfx-graph))

- Video: Fixed recording is not created when path containing Japanese characters.
    ([UUM-116121](https://issuetracker.unity3d.com/issues/errors-are-thrown-and-the-recording-file-is-not-created-when-japanese-characters-are-included-in-the-output-file-path))

- Video: Re-importing a WebM file generates an inconsistent result.
    (UUM-113154)

- Web: Fixed an issue where WebGL 1.0 builds were not correctly using the fallback fullscreen mesh with fullscreen blits using URP.
    ([UUM-110571](https://issuetracker.unity3d.com/issues/overlay-camera-is-not-rendered-when-graphics-api-is-set-to-webgl-1-dot-0))




## Package changes in 2022.3.68f1

## Packages updated

- com.unity.addressables: [1.27.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.27//changelog/CHANGELOG.html) to [1.28.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.24](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.25](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.9.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.9//changelog/CHANGELOG.html) to [2.10.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.10//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.37](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.14.2](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.14//changelog/CHANGELOG.html) to [1.15.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.15//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat: [1.4.5](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) to [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.remote-config: [3.3.2](https://docs.unity3d.com/Packages/com.unity.remote-config@3.3//changelog/CHANGELOG.html) to [4.2.2](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html)

- com.unity.remote-config-runtime: [3.1.3](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@3.1//changelog/CHANGELOG.html) to [4.0.2](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@4.0//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.23.0](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) to [1.23.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [2.6.4](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.6//changelog/CHANGELOG.html) to [2.6.5](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.6//changelog/CHANGELOG.html)

- com.unity.services.moderation: [1.0.1](https://docs.unity3d.com/Packages/com.unity.services.moderation@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.moderation@1.1//changelog/CHANGELOG.html)

- com.unity.asset-manager-for-unity: [1.5.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.5//changelog/CHANGELOG.html) to [1.7.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.7//changelog/CHANGELOG.html)