# Unity 2022.3.51f1 LTS
Published at Tue, 22 Oct 2024 16:55:03 GMT  
https://unity.com/releases/editor/whats-new/2022.3.51

# Known Issues in 2022.3.51f1

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Build Settings Window: "EndLayoutGroup: BeginLayoutGroup must be called first." error is thrown after building the project when Scripting Backend and Api Compatibility Level fields are changed
    ([UUM-84914](https://issuetracker.unity3d.com/issues/endlayoutgroup-beginlayoutgroup-must-be-called-first-dot-error-is-thrown-after-building-the-project-when-scripting-backend-and-api-compatibility-level-fields-are-changed))

- DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when opening a project after changing the Graphics API to DirectX12
    ([UUM-77757](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-opening-a-project-after-changing-the-graphics-api-to-directx12))

- Hybrid Renderer: [Linux] Crash on ScriptableBatchRenderer::GenerateBuiltInCBuffer when adding "PerObjectData.ReflectionProbes"
    ([UUM-79332](https://issuetracker.unity3d.com/issues/linux-crash-on-scriptablebatchrenderer-generatebuiltincbuffer-when-adding-perobjectdata-dot-reflectionprobes))

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Vulkan: [Android] Particles not rendered in the Player on some Android devices with Android 14
    ([UUM-68080](https://issuetracker.unity3d.com/issues/android-particles-not-rendered-in-the-player-on-some-android-devices-with-android-14))



# 2022.3.51f1 Release Notes

## Changes

- Editor: Updated com.unity.openxr package version to 1.13.0.



## Fixes

- Android: Synchronized show-hide softInput operations.
    ([UUM-71798](https://issuetracker.unity3d.com/issues/input-events-are-queued-up-and-virtual-keyboard-opens-and-closes-with-1-input-event))

- Animation: Fixed crash when attempting to recreate the Animator bindings, by enabling a RigBuilder that binds a transform stream handle for example, while the Animator was being evaluated.
    ([UUM-80043](https://issuetracker.unity3d.com/issues/crash-on-unityengine-animation-setgenericfloatpropertyvalues-when-keyframing-the-rigbuilder-component-to-enabled-and-disabled))

- Apple TV: Added support for Siri Remote 2nd Gen.

- Asset Pipeline: Fixed missing assets errors in SubScene importer after domain reload.
    ([UUM-82547](https://issuetracker.unity3d.com/issues/missing-prefab-asset-error-in-a-subscene-after-domain-reload))

- Audio: Fixed race condition causing the audio engine to see a sound as `READY` because it started to load.
    (UUM-36353)

- Editor: Ensure that when opening from Project browser the search window query is correctly populated.
    ([UUM-79369](https://issuetracker.unity3d.com/issues/a-second-search-window-opens-when-one-is-already-opened-from-the-project-window-and-the-search-field-is-populated-with-the-project-search-pill-string))

- Editor: F-key functionality restored, and menu items enable/disable correctly.
    ([UUM-83883](https://issuetracker.unity3d.com/issues/ubuntu-cant-type-the-letter-f))

- Editor: Fixed an issue where Editor menus on macOS could render blank and cause the editor to hang.
    ([UUM-73279](https://issuetracker.unity3d.com/issues/mac-menu-sometimes-renders-empty-when-using-help))

- Editor: Fixed an issue where editor windows would stay on coordinates of a disconnected display, making them inaccessible to the user.
    ([UUM-75313](https://issuetracker.unity3d.com/issues/floating-editor-windows-resize-to-smallest-size-when-disconnecting-monitor-on-multi-monitor-setup))

- Editor: Fixed an issue where the texture size was not reported correctly in the inspector, if "Load texture data on demand" was enabled.
    ([UUM-77739](https://issuetracker.unity3d.com/issues/texture-does-not-display-its-size-when-observing-through-inspector-preview))

- Editor: Fixed crash in Linux when opening recent scenes from the File menu.
    ([UUM-82381](https://issuetracker.unity3d.com/issues/linux-crash-on-menucontroller-executemenuitem-when-selecting-recent-scene))

- Editor: Fixed DeviceSimulator to implement Touch.rawPosition to return the starting position of the simulated touch contact.
    ([UUM-58248](https://issuetracker.unity3d.com/issues/touch-dot-rawposition-always-returns-00-when-clicking-or-dragging-anywhere-on-the-screen-in-the-play-mode))

- Editor: Linux Editor no longer crashes when creating a prefab variant from the context menu in a read-only directory.
    ([UUM-76157](https://issuetracker.unity3d.com/issues/linux-crash-on-createvariant-when-a-prefab-variant-is-created-in-the-packages-folder))

- Editor: Prevent user from deleting a parent material without reparenting its children.
    ([UUM-73507](https://issuetracker.unity3d.com/issues/crash-when-selecting-a-certain-material))

- Editor: Removed default timeout in searchsession.
    ([UUM-81554](https://issuetracker.unity3d.com/issues/infinite-loading-slash-freezing-in-memory-profiler-when-trying-to-view-object-details-from-the-unity-object-tab))

- Editor: SRP Batcher supports Integer type "stencil ref".
    ([UUM-79305](https://issuetracker.unity3d.com/issues/when-the-type-of-the-stencil-ref-property-in-the-shader-is-an-integer-srp-batching-is-not-broken-even-if-the-stencil-ref-values-differ))

- Editor: Windows moved to a different display on Windows upon display disconnect will no longer have the minimum size.

- Graphics: Fixed issue in which raw Image that uses a Material with a custom Shader is invisible in Canvas when "Screen Space - Overlay" is set and the Player is in "Windowed" mode.
    ([UUM-73042](https://issuetracker.unity3d.com/issues/raw-image-that-uses-a-material-with-a-custom-shader-is-invisible-in-canvas-when-screen-space-overlay-is-set-and-the-player-is-in-windowed-mode))

- Graphics: When using the Metal graphics API, SystemInfo.SupportsRandomWriteOnRenderTextureFormat\(\) will now check the Metal device's readWriteTextureSupport tier to check whether a texture format supports simultaneous read and writes in a shader. With this change, this function will now return false for some texture formats that previously made it return true. One example is RenderTextureFormat.RG16 that previously made it return true but now false is returned instead.
    ([UUM-70740](https://issuetracker.unity3d.com/issues/supportsrandomwriteonrendertextureformat-shows-false-when-executed-on-2023-dot-2-and-6000-dot-0-streams))

- IL2CPP: Fixed issue with the wrong calling convention being used on function pointers when two function pointers with the same signature only differed by calling convention.

- iOS: Fixed logging when using "Wait for the executable to be launched".
    ([UUM-78223](https://issuetracker.unity3d.com/issues/ios-logging-does-not-work-when-using-wait-for-the-executable-to-be-launched))

- iOS: Fixed Unity launching in background on background app activation.
    (UUM-82451)

- Linux: Fixed screen resolution does not sync properly with the system's when changing system resolution during runtime.
    (UUM-64956)

- Mono: Fixed JIT trampoline memory leak with Timers and Sockets.
    ([UUM-76306](https://issuetracker.unity3d.com/issues/memory-leak-when-using-net-sockets))

- Particles: Scheduling a Particle System job outside of MonoBehaviour.OnParticleUpdateJobScheduled\(\) will now generate an InvalidOperationException in order to prevent incorrect job schedules which could cause a hang.
    ([UUM-79599](https://issuetracker.unity3d.com/issues/editor-freezes-slash-hangs-when-calling-schedulebatch-for-ijobparticlesystemparallelforbatch))

- Physics: Fixed an issue with the Cloth component's inspector where exiting play-mode with the self and inter collision tool open would cause a null reference exception.
    ([UUM-78853](https://issuetracker.unity3d.com/issues/errors-nullreferenceexception-object-reference-not-set-to-an-instance-of-an-object-and-cannot-modify-overlay-dot-displayed-during-event-of-type-eventtype-dot-layout-shown-when-entering-the-play-mode-with-self-collision-and-inter-collision-window-focused))

- Physics: Revert fix for small body tunnelling at high \(~200Hz\) simulation frequencies. If effected please use recommended workaround \(decrease ccd threshold to slightly under 1/4 of the half-extent of the scene's smallest object\).

- Shadergraph: Added issue where precision mismatch could result in an asset failing to import.
    ([UUM-74920](https://issuetracker.unity3d.com/issues/invalidoperationexception-precision-mismatch-error-is-thrown-in-the-console-when-multiplying-two-half-precision-values-in-a-multiply-node-with-single-precision-in-shader-graph))

- Shadergraph: Fixed a bug that a shader graph is reverted to its last saved state when entering Play Mode without saving changes.
    ([UUM-49399](https://issuetracker.unity3d.com/issues/shader-graph-is-reverted-to-its-primary-state-when-entering-play-mode-without-saving-changes))

- Shaders: Fixed a copy/paste issue when right-clicking on the property of shader created with TexturePropertySingleLine\(\).
    (UUM-78130)

- Shaders: Fixed compute shader compilation variant cache hits to be reported correctly in the editor log.
    ([UUM-75264](https://issuetracker.unity3d.com/issues/shader-cache-is-not-used-when-building-the-player-repeatedly))




## Package changes in 2022.3.51f1

## Packages updated

- com.unity.services.analytics: [5.0.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@5.0//changelog/CHANGELOG.html) to [6.0.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.12.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.12//changelog/CHANGELOG.html) to [1.13.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.13//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.asset-manager-for-unity@1.0.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.0//changelog/CHANGELOG.html)