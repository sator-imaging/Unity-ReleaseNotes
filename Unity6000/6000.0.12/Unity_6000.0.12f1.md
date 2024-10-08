# Unity 6000.0.12f1
Published at Thu, 25 Jul 2024 16:59:55 GMT  
https://unity.com/releases/editor/whats-new/6000.0.12

# Known Issues in 6000.0.12f1

- Asset - Database: OnAfterDeserialize is not called when Prefabs are instantiated using InstantiateAsync
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- Asset Bundles: The resource is not properly referenced when there is a dependency on another asset bundle
    ([UUM-74871](https://issuetracker.unity3d.com/issues/the-resource-is-not-properly-referenced-when-there-is-a-dependency-on-another-asset-bundle))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Lighting: Block compression leads to lightbaking artifacts in HDRP
    ([UUM-74735](https://issuetracker.unity3d.com/issues/lightmap-has-artifacts-when-generating-lighting))

- Material: Crash on SourceAssetDBReadTxn::SourceAssetDBReadTxn when opening a project after deleting an Asset
    ([UUM-75191](https://issuetracker.unity3d.com/issues/crash-on-sourceassetdbreadtxn-sourceassetdbreadtxn-when-opening-a-project-after-deleting-an-asset))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- SRP Architecture & API: URP internal shader errors when the iOS is selected as a Build Target on the Windows Editor
    ([UUM-75654](https://issuetracker.unity3d.com/issues/urp-internal-shader-errors-when-the-ios-is-selected-as-a-build-target-on-the-windows-editor))

- SRP Templates: A bunch of Shader Warnings are thrown after switching platform to Linux/Linux Server when using Universal 3D Template
    ([UUM-76186](https://issuetracker.unity3d.com/issues/a-bunch-of-shader-warnings-are-thrown-after-switching-platform-to-linux-when-using-universal-3d-template))

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- Vulkan:  Editor crash when changing Vulkan Number of Swapchain Buffers
    ([UUM-60016](https://issuetracker.unity3d.com/issues/vulkan-editor-crash-when-changing-vulkan-number-of-swapchain-buffers))



# 6000.0.12f1 Release Notes

## Improvements

- Graphics: Allowed performing a Submit of Render Request from RenderPipelineManager callbacks.

- Physics 2D: Removed invalid sentence in Scripting documentation for the Collider2D.Overlap methods that accept a List&lt;T&gt; as an argument.



## Changes

- AI: `NavMeshBuilder.CollectSources()` can now return only the physics objects that are within a volume extending `1e9` units in all 3 dimensions.



## Fixes

- 2D: Fixed Gem Hunter sample not working on iOS Simulator.
    (UUM-74000)

- Android: AndroidApplication.onConfigurationChanged will reuse AndroidConfiguration instance for sequential calls, if you want to cache configuration instance, use AndroidConfiguration.CopyFrom function.
    (UUM-75092)

- Android: Location Services will now resume \(if it is enabled\) automatically when app is paused or resumed.

- Android: Reworked `Input.location` so it now work with GameActivity.
    (UUM-74113)

- DX12: Fixed a GPU crash by unbind counter resources.
    ([UUM-75100](https://issuetracker.unity3d.com/issues/dx12-player-crash-on-unitymain-when-building-hdrp-sample-on-windows))

- Editor: Clear culling cache results before rendering selection outlines.
    ([UUM-69725](https://issuetracker.unity3d.com/issues/selection-outline-and-selection-wire-are-not-rendered-in-the-scene-view-when-the-mesh-renderer-components-cast-shadows-field-is-set-to-shadows-only))

- Editor: Fixed an editor crash during import when the project has a saved layout of an open build profile window.
    (UUM-73189)

- Editor: Fixed an issue that would cause a crash when the Editor was exited when GLES is the active graphics API.
    ([UUM-54445](https://issuetracker.unity3d.com/issues/editor-that-is-opened-using-a-command-line-with-a-force-gles-argument-crashes-on-drvpresentbuffers-when-closing-the-editor-on-windows-with-a-nvidia-rtx-a2000-gpu))

- Editor: Fixed an issue with RenderRaph API so when a pass modifies the global rendering state, we should prevent it from being culled.
    (UUM-73906)

- Editor: Fixed issue with Window/Panels menu items.
    ([UUM-74640](https://issuetracker.unity3d.com/issues/test-runner-incorrect-name-under-window-panel-after-project-restart))

- Editor: Fixed registration error being thrown when a UxmlElement has the same name as the class.
    ([UUM-73716](https://issuetracker.unity3d.com/issues/an-error-is-thrown-when-a-custom-class-uxlelement-component-is-derived-from-a-normal-component))

- Editor: Updated the sliders in the ARC window so that users can see visually when the randomisation range is being clipped.
    (UUM-50343)

- Graphics: Bursted culling input creation in OnPerformCulling with GPUResidentDrawer to improve performances.
    (UUM-75306)

- Graphics: Fixed an issue that caused an error and shader to not load and render with GPUResidentDrawer.
    (UUM-75298)

- Graphics: Fixed an issue where DBuffer decals where not applied before sampling GI.
    ([UUM-34259](https://issuetracker.unity3d.com/issues/dbuffer-decals-do-not-affect-ambient-lighting-correctly))

- Graphics: Fixed crash when using SRP, Handle.DrawOutline\(\) and filtering the hierarchy.
    ([UUM-67677](https://issuetracker.unity3d.com/issues/crash-on-camera-releasecamerastackrenderingstate-when-searching-in-hierarchy))

- Graphics: Now correctly handle unsupported shaders on resource change with GPUResidentDrawer.
    (UUM-75302)

- HDRP: Allowed TAAU, CAS, and STP to execute after the DoF or after all the post-processes like the other advanced upsamplers.
    (UUM-75530)

- Kernel: Optimized job allocator with memory synchronization fix to avoid freezes.
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- macOS: Fixed an issue where resolution not resetting to full screen when going to full-screen window by using native MacOS UI controls.
    ([UUM-73633](https://issuetracker.unity3d.com/issues/black-bars-appear-around-the-main-view-when-player-is-in-fullscreen-mode))

- Particles: Fixed a freeze that occurs if user particle system jobs are completed immediately after schedule.
    ([UUM-74409](https://issuetracker.unity3d.com/issues/editor-freezes-when-opening-a-scene-containing-a-timeline))

- Profiler: Fixed a Memory Profiler issue that could cause the total size of a memory root to differ slightly from the sum of its individually reported allocations, as allocation header bytes and unused/fragmentation bytes could be included.
    (UUM-75352)

- Scripting: Fixed issue with an InstantiateAsync which does not invoke OnAfterDeserialize after the prefab was instantiated in Editor.
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- SRP Core: Avoid that the same volume can be registered more than 1 time in the VolumeManager.
    ([UUM-70658](https://issuetracker.unity3d.com/issues/unityengine-dot-rendering-dot-volume-dot-onenable-is-called-twice-before-ondisable-creating-multiple-copies-of-the-same-volume-when-a-volume-is-enabled-right-after-domain-reload-when-entering-play-mode))

- SRP Core: Fixed crash caused by indirect argument buffer being one item too small.
    ([UUM-73969](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-updatecomputeresources-when-in-the-play-mode))

- UI Toolkit: Added an auto-generated tag to UxmlElement and UxmlObject generated code.
    ([UUM-75492](https://issuetracker.unity3d.com/issues/uxmlserializeddata-generated-code-does-not-contain-auto-generated-tag))

- UI Toolkit: Disabled template UxmlObject fields in the UI Builder. Attribute overrides do not currently support UxmlObjects.
    ([UUM-72789](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-overriding-the-uxmlobjectreferences-in-template-instances))

- UI Toolkit: Fixed an issue where setting a field with showMixedValue would cause it to revert to the previous value.
    ([UUM-73855](https://issuetracker.unity3d.com/issues/the-non-zero-value-is-changed-to-0-when-entering-it-for-the-first-time-into-the-integerfield-with-showmixedvalue-set-to-true))

- UI Toolkit: Fixed exception when viewing template UxmlObject attributes in the UI Builder.
    ([UUM-75608](https://issuetracker.unity3d.com/issues/ui-builder-editing-a-template-which-contains-uxmlobjects-throws-null-reference-exceptions-and-breaks-the-inspector))

- URP: Fixed a shader compilation error on Apple platforms without Metal.
    (UUM-75548)

- Video: Memory increases gradually when UWP webcam is opened or closed.
    ([UUM-62347](https://issuetracker.unity3d.com/issues/memory-increases-gradually-when-the-camera-is-opened-and-closed))




## Package changes in 6000.0.12f1

## Packages updated

- com.unity.ide.rider: [3.0.28](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.31](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.8.2](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.8//changelog/CHANGELOG.html) to [1.9.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.9//changelog/CHANGELOG.html)

- com.unity.purchasing: [4.12.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.12//changelog/CHANGELOG.html) to [4.12.1](https://docs.unity3d.com/Packages/com.unity.purchasing@4.12//changelog/CHANGELOG.html)

- com.unity.services.friends: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html)

- com.unity.services.lobby: [1.2.0](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.2//changelog/CHANGELOG.html) to [1.2.2](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.2//changelog/CHANGELOG.html)

- com.unity.learn.iet-framework: [3.1.3](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@3.1//changelog/CHANGELOG.html) to [4.0.0](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@4.0//changelog/CHANGELOG.html)

- com.unity.multiplayer.playmode: [1.2.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.2//changelog/CHANGELOG.html) to [1.2.1](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.2//changelog/CHANGELOG.html)

- com.unity.dedicated-server: [1.2.0](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.2//changelog/CHANGELOG.html) to [1.2.1](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.2//changelog/CHANGELOG.html)

- com.unity.dt.app-ui: [1.0.3](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.1//changelog/CHANGELOG.html)

**Pre-release packages added**

- [com.unity.dt.app-ui@2.0.0-pre.6](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.0//changelog/CHANGELOG.html)