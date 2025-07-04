# Unity 2022.3.64f1 LTS
Published at Wed, 02 Jul 2025 17:03:17 GMT  
https://unity.com/releases/editor/whats-new/2022.3.64

# Known Issues in 2022.3.64f1

- DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when opening a project after changing the Graphics API to DirectX12
    ([UUM-77757](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-opening-a-project-after-changing-the-graphics-api-to-directx12))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DirectX12: The Player hangs when unloading a scene using the UnloadUnusedAssets() method
    ([UUM-79718](https://issuetracker.unity3d.com/issues/the-player-hangs-when-unloading-a-scene-using-the-unloadunusedassets-method))

- Graphics Device Features: Graphics.RenderMeshIndirect does not issue multi-draw rendering commands when using a graphics API capable of multi-draw commands
    ([UUM-91617](https://issuetracker.unity3d.com/issues/graphics-dot-rendermeshindirect-does-not-issue-multi-draw-rendering-commands-when-using-a-graphics-api-capable-of-multi-draw-commands))

- Scene Management: Editor hangs when cutting and pasting a Script to another folder during Play Mode
    ([UUM-104031](https://issuetracker.unity3d.com/issues/editor-hangs-when-cutting-and-pasting-a-script-to-another-folder-during-play-mode))

- Video: Editor crashes with PlatformWebCamTexture::GetDeviceNames when a Virtual Camera is present and FriendlyName property is deleted from Registry
    ([UUM-105563](https://issuetracker.unity3d.com/issues/editor-crashes-with-platformwebcamtexture-getdevicenames-when-a-virtual-camera-is-present-and-friendlyname-property-is-deleted-from-registry))

- Vulkan: [Android] Runtime performance deteriorates on certain Android devices when Graphics API is set to Vulkan on an upgraded project
    ([UUM-107530](https://issuetracker.unity3d.com/issues/build-performance-deteriorates-on-certain-android-devices-when-graphics-api-is-set-to-vulkan-on-an-upgraded-project))

- Web Platform: Garbage Collector memory leak when allocating and deallocating memory in Web builds
    ([UUM-86352](https://issuetracker.unity3d.com/issues/garbage-collector-memory-leak-when-allocating-and-deallocating-memory-in-web-builds))



# 2022.3.64f1 Release Notes

## Improvements

- Shadergraph: Added an issue where the far right toolbar dropdown was sometimes difficult to interact with.
    ([UUM-105177](https://issuetracker.unity3d.com/issues/shader-graph-more-options-dropdown-button-does-not-open-the-dropdown-when-clicked-all-the-way-to-the-right-of-the-button))

- Shadergraph: Added both preference and setting path for variant limit exceeded warning message.
    ([UUM-104591](https://issuetracker.unity3d.com/issues/shadergraph-wrong-setting-path-in-tooltip-for-exceeded-variant-limit))

- Shadergraph: Improved resizing behavior for custom property and function inspectors.
    ([UUM-103867](https://issuetracker.unity3d.com/issues/custom-property-and-function-labels-at-the-top-of-the-graph-inspector-go-out-of-bounds-and-are-not-truncated-when-string-is-long))

- Shadergraph: Improved shader variant exceeded message to direct users to both project settings and preferences.
    ([UUM-104591](https://issuetracker.unity3d.com/issues/shadergraph-wrong-setting-path-in-tooltip-for-exceeded-variant-limit))

- Shadergraph: Improved spacing of a certain toggle on the shader graph preferences page.
    ([UUM-104088](https://issuetracker.unity3d.com/issues/checkbox-collides-with-text-in-shader-graph-preferences-settings))



## Changes

- Build Pipeline: Build Pipeline: Allow building AssetBundles with both the DisableTypeTree and StripUnityVersion flags. Fix the ability to load these AssetBundles in the Runtime.
    ([UUM-102575](https://issuetracker.unity3d.com/issues/an-error-is-thrown-when-building-assetbundles-with-disablewritetypetree-and-stripunityversion-flags))



## Fixes

- Android: Enforcing to use Streaming Assets extensions for noCompress string in Android Gradle project to avoid problem with too many entries in the list, which may cause Gradle build fail.
    ([UUM-105133](https://issuetracker.unity3d.com/issues/android-build-fails-when-streamingassets-contains-998-or-more-files))

- Android: Fixed Integer input field allowing multiple "-" symbols under certain conditions \(on non TMP platforms\).
    ([UUM-103402](https://issuetracker.unity3d.com/issues/multiple-symbols-are-allowed-to-appear-in-a-row-when-inputting-dot-into-a-non-decimal-numeric-field))

- Android: Fixed issue where RenderBufferLoadAction.DontCare is ignored in some situation when switching between use of RenderPass API and SetRenderTarget.
    ([UUM-104821](https://issuetracker.unity3d.com/issues/vulkan-dont-care-loadaction-resets-to-load-when-running-on-mali-devices))

- Animation: Fixed an issue where disabling an Animator would stop the Animator from evaluating.
    ([UUM-107650](https://issuetracker.unity3d.com/issues/animator-does-not-continue-animation-indefinitely-when-toggling-animator-dot-enabled-through-code))

- Audio: Fixed an issue on macOS where recording from a Bluetooth microphone could fail or produce corrupted audio. Audio input now correctly handles variable frame counts and uses a dedicated buffer to ensure all recorded data is captured reliably.
    ([UUM-403](https://issuetracker.unity3d.com/issues/audio-becomes-mono-and-voice-recording-is-chopped-when-recording-audio-using-bluetooth-headphones-with-integrated-microphone))

- Burst: Fixed that player builds using IL2CPP on Linux would have truncated stacktraces if Burst was in the callstack.
    ([BUR-2858](https://issuetracker.unity3d.com/issues/linux-truncated-stack-traces-when-logging-from-managed-code-in-burst))

- DX12: Fixed a memory leak in tests.
    (UUM-78511)

- Editor: Added new callback `onDeleteArrayElementCallback ` to `ReorderableList`. This is called from the "Delete Array Element" context menu to let you control the removal, like `onRemoveCallback`.
    ([UUM-104534](https://issuetracker.unity3d.com/issues/onremovecallback-is-not-called-when-removing-an-element-from-the-reoderablelist-using-contextmenu))

- Editor: Fixed an issue where Scene view gizmo icons were not loaded properly if "Load textures on demand" was enabled in project settings.
    ([UUM-104825](https://issuetracker.unity3d.com/issues/load-texture-data-on-demand-corrupts-unitys-packages-gizmos-in-scene-view))

- Editor: Fixed by displaying more details in the log message and displaying them only once to avoid spam.
    ([UUM-77757](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-opening-a-project-after-changing-the-graphics-api-to-directx12))

- Editor: Random crash in BatchRendererGroup rendering fixed.
    (UUM-105252)

- Editor: Removed the "Check for Updates" window.
    ([UUM-102388](https://issuetracker.unity3d.com/issues/check-for-updates-fails-to-connect-to-update-server))

- Editor: The Frame value field does not update when using the increment/decrement arrows in the Frame Debugger if the value has been manually inputted.
    ([UUM-107394](https://issuetracker.unity3d.com/issues/the-frame-value-field-does-not-update-when-using-the-increment-slash-decrement-arrows-in-the-frame-debugger-if-the-value-has-been-manually-inputted))

- Graphics: Fixed a validation warning on DirectX by changing the fake input layout format.
    ([UUM-105001](https://issuetracker.unity3d.com/issues/a-vertex-stream-with-a-stride-of-1-is-bound-to-the-gpu-in-player-when-mesh-is-compressed))

- Graphics: Fixed D3D12 crash on integrated GPU due to missing constant buffer binding.
    (UUM-69598)

- Kernel: JobHandle.Complete\(\) goes to sleep sooner when there is no work to steal. This allows the waiting thread to give up the CPU core sooner to allow another thread to perform work or to preserve battery life.
    (UUM-83082)

- Mono: Fixed GC Handle leak that would happen every time a new function pointer was returned for a managed delegate.
    ([UUM-105139](https://issuetracker.unity3d.com/issues/unmanagedreadorwrite-objects-are-not-disposed-off-when-gzipstream-is-used-in-the-using-statement))

- Package Manager: Fixed an issue where installing a git package using Git LFS would not work with Git LFS 3.6.0 and higher.
    (UUM-91342)

- Package Manager: Fixed the issue where Assets cannot be imported when the Asset package contains project settings and all project settings are unchanged.
    ([UUM-100078](https://issuetracker.unity3d.com/issues/assets-do-not-get-imported-from-an-asset-package-when-library-assets-in-the-asset-package-are-unchanged))

- Package Manager: UnityEditor.PackageManager.UI.Sample.FindByPackage will no longer throw an exception when passed an unknown package.
    (UUM-86326)

- Physics 2D: Fixed memory leak when reporting 2D physics collision callbacks.
    ([UUM-108093](https://issuetracker.unity3d.com/issues/memory-leak-when-using-rigidbody2d-physics-in-webgl))

- Shadergraph: Added wrapping to the custom function node's label and fixed an issue where it would not update immediately.
    ([UUM-103861](https://issuetracker.unity3d.com/issues/custom-function-nodes-label-and-name-field-is-not-limited-to-the-graph-inspectors-bounds))

- Shadergraph: Float node documentation link now resolves correctly.
    ([UUM-103781](https://issuetracker.unity3d.com/issues/a-404-page-is-opened-when-selecting-open-documentation-on-the-float-node-in-shader-graph))

- Shadergraph: Shader Graph Asset help button now redirects to the correct URL.
    ([UUM-103777](https://issuetracker.unity3d.com/issues/shader-graph-importers-documentation-reference-button-leads-to-a-404-page))

- Shadergraph: Speed Tree subgraphs documentation link now resolves correctly.
    ([UUM-103972](https://issuetracker.unity3d.com/issues/a-404-page-is-opened-when-selecting-open-documentation-for-any-speedtree-sub-graph-asset))

- Shadergraph: Sub Graph Asset help button now redirects to the correct URL.
    ([UUM-105173](https://issuetracker.unity3d.com/issues/shader-graph-import-settings-documentation-leads-to-sorry-dot-dot-dot-that-page-seems-to-be-missing-page-when-opened-through-the-documentation-button-in-the-inspector-window))

- Shadergraph: Sub Graph node documentation link now redirects to the correct URL.
    ([UUM-103971](https://issuetracker.unity3d.com/issues/a-404-page-is-opened-when-selecting-open-documentation-for-any-custom-sub-graph-in-shader-graph))

- Text: Improved WeakReference handling to protect against the \(extremely unlikely, but still possible\) event that the GC runs between checking that the handle is alive and dereferencing it.
    (UUM-86325)

- Text: Removed redundant check for null SpriteCharacters when generating text meshes.
    (UUM-86328)

- UI Toolkit: Fixed an issue where debug names would not appear when pressing the Alt key in debug inspector mode.
    ([UUM-18712](https://issuetracker.unity3d.com/issues/uitoolkit-inspector-property-names-dont-show-up-correctly-when-inspector-is-in-debug-mode))

- UI Toolkit: Fixed highlight color of the uxml header when doing a drag and drop from the Library.
    ([UUM-76953](https://issuetracker.unity3d.com/issues/dragging-any-ui-element-under-the-uxml-file-in-the-ui-builder-hierarchy-doesnt-highlight-it))

- Video: Fixed double invocation of onLoopPoint callback when `skipOnDrop` is false and codec is decoding to memory.
    ([UUM-97953](https://issuetracker.unity3d.com/issues/videoplayer-dot-looppointreached-invokes-twice-when-waitforfirstframe-is-enabled))

- Video: Fixed sporadic crash of video player on iOS when app is brought from background to foreground.
    (UUM-93765)

- XR: Fixed an issue where the XrDisplaySubsystem tries to destroy textures that are still being used by other processes. This fix uses FinishRendering\(\) to block the simulation thread until those resources are no longer in use before trying to destroy them.
    (UUM-109086)

- XR: Fixed and issue where deployed URP Quest Applications throw Vulkan Errors on App Exit.
    (UUM-109083)




## Package changes in 2022.3.64f1

## Packages updated

- com.unity.2d.animation: [9.2.0](https://docs.unity3d.com/Packages/com.unity.2d.animation@9.2//changelog/CHANGELOG.html) to [9.2.1](https://docs.unity3d.com/Packages/com.unity.2d.animation@9.2//changelog/CHANGELOG.html)

- com.unity.2d.common: [8.1.0](https://docs.unity3d.com/Packages/com.unity.2d.common@8.1//changelog/CHANGELOG.html) to [8.1.1](https://docs.unity3d.com/Packages/com.unity.2d.common@8.1//changelog/CHANGELOG.html)

- com.unity.2d.psdimporter: [8.1.0](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.1//changelog/CHANGELOG.html) to [8.1.1](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.1//changelog/CHANGELOG.html)

- com.unity.2d.spriteshape: [9.1.0](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@9.1//changelog/CHANGELOG.html) to [9.1.1](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@9.1//changelog/CHANGELOG.html)

- com.unity.addressables: [1.22.3](https://docs.unity3d.com/Packages/com.unity.addressables@1.22//changelog/CHANGELOG.html) to [1.25.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.25//changelog/CHANGELOG.html)

- com.unity.burst: [1.8.21](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.23](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.cinemachine: [2.10.3](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) to [2.10.4](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.mobile.notifications: [2.4.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) to [2.4.1](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- com.unity.postprocessing: [3.4.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.4//changelog/CHANGELOG.html) to [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.22.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html) to [1.22.5](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html)

- com.unity.services.vivox: [16.6.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.6//changelog/CHANGELOG.html) to [16.6.2](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.6//changelog/CHANGELOG.html)

- com.unity.asset-manager-for-unity: [1.2.2](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.2//changelog/CHANGELOG.html) to [1.5.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.5//changelog/CHANGELOG.html)