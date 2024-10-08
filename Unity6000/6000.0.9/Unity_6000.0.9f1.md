# Unity 6000.0.9f1
Published at Wed, 03 Jul 2024 14:22:27 GMT  
https://unity.com/releases/editor/whats-new/6000.0.9

# Known Issues in 6000.0.9f1

- Asset - Database: OnAfterDeserialize is not called when Prefabs are instantiated using InstantiateAsync
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- Asset Bundles: The resource is not properly referenced when there is a dependency on another asset bundle
    ([UUM-74871](https://issuetracker.unity3d.com/issues/the-resource-is-not-properly-referenced-when-there-is-a-dependency-on-another-asset-bundle))

- Audio Random Container: Play on awake does not work with an audio random container when instantiating a game object
    ([UUM-74723](https://issuetracker.unity3d.com/issues/play-on-awake-does-not-work-with-an-audio-random-container-when-instantiating-a-game-object))

- Build Settings Window: [Windows] Hold on is being shown after switching platform and only disappears after hovering on the window 
    ([UUM-74797](https://issuetracker.unity3d.com/issues/windows-hold-on-is-being-shown-after-switching-platform-and-only-disappears-after-hovering-on-the-window))

- DirectX12: Crash on D3D12 when entering Play Mode in High Definition 3D Core project's Environment scene
    ([UUM-74769](https://issuetracker.unity3d.com/issues/crash-on-d3d12-when-entering-play-mode-in-high-definition-3d-core-projects-environment-scene))

- DOTS: Job allocator contention causes slow job execution
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- Editor Platform: The "Hold On" dialog box persists when entering the Play Mode
    ([UUM-74916](https://issuetracker.unity3d.com/issues/the-hold-on-dialog-box-persists-when-entering-the-play-mode))

- Hybrid Renderer: Crash when loading RenderDoc in a specific Scene
    ([UUM-73405](https://issuetracker.unity3d.com/issues/crash-when-loading-renderdoc-in-a-specific-scene))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Lighting: Lightmap has artifacts when Generating Lighting
    ([UUM-74735](https://issuetracker.unity3d.com/issues/lightmap-has-artifacts-when-generating-lighting))

- Menu Management: Custom and built-in menu items stop working when a project has lots of menu items
    ([UUM-73047](https://issuetracker.unity3d.com/issues/custom-and-built-in-menu-items-stop-working-when-a-project-has-lots-of-menu-items))

- Mono: [TypeCache] Crash on RaiseException when opening a specific project
    ([UUM-66498](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-opening-a-specific-project))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Vulkan:  Editor crash when changing Vulkan Number of Swapchain Buffers
    ([UUM-60016](https://issuetracker.unity3d.com/issues/vulkan-editor-crash-when-changing-vulkan-number-of-swapchain-buffers))

- Vulkan: [Linux][Vulkan] Crash when using Nvidia drivers >545 and graphics API set to Vulkan
    ([UUM-73447](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-when-using-nvidia-drivers-545-and-graphics-api-set-to-vulkan))



# 6000.0.9f1 Release Notes

## Improvements

- Editor: Added details to the "incompatible keyword space" error message which is occasionally generated by shaders.
    ([UUM-58563](https://issuetracker.unity3d.com/issues/state-comes-from-incompatible-keyword-space-error-not-very-informative))

- Editor: Compute buffer bindings and textures are now maintained when hot reloading assets.
    ([UUM-70123](https://issuetracker.unity3d.com/issues/graphicsbuffer-unbinds-from-materials-registered-with-entitiesgraphicssystem-at-runtime-when-the-subscene-is-saved))

- Editor: Improving Splashscreen code.

- Graphics: Improved CPU performance of Native Render Pass path in GfxDevice to speed up URP RenderGraph.

- UI Toolkit: Added UX improvement for missing workflow when extracting inline value to selector.



## API Changes

- GI: Added: Added an API for getting the associated shadowmask channels of lights retrieved from the InputExtraction.ComputeOcclusionLightIndicesFromBakeInput function.
    ([UUM-44229](https://issuetracker.unity3d.com/issues/adaptive-probe-volume-is-incorrectly-baked-when-using-mixed-mode-light))



## Changes

- Version Control: Added "Undo unchanged" and "Undo checkouts keeping changes" options to pending changes view.

- Version Control: Changed the default ignore.conf to not ignore itself anymore.

- Version Control: Removed focus redirection after Check-in.



## Fixes

- Audio: Fixed an issue where alternating between the AudioSource.clip and AudioSource.resource setters would cause the AudioSource.volume setter to have no effect.
    ([UUM-71884](https://issuetracker.unity3d.com/issues/using-audiosource-dot-clip-to-change-from-audio-random-container-when-play-on-awake-is-enabled-some-audio-source-apis-broken))

- Build System: Fixed a potential crash when building.
    ([UUM-72309](https://issuetracker.unity3d.com/issues/crash-on-mono-array-length-when-building-a-project))

- Editor: Fixed a crash when interacting with a shader variant collection containing shaders with dynamic branch keywords after de-/serializing the collection.
    ([UUM-73491](https://issuetracker.unity3d.com/issues/crash-on-free-alloc-internal-when-clearing-shader-variants-in-certain-projects))

- Editor: Fixed docked Build Profiles window becomes messy during the resizing.
    ([UUM-62193](https://issuetracker.unity3d.com/issues/build-profiles-window-becomes-messy-during-the-resizing))

- Editor: Fixed long build profile names are not shortened properly in Build Profile Editor.
    ([UUM-60859](https://issuetracker.unity3d.com/issues/longer-build-profile-titles-are-not-compatible-with-the-resized-window))

- Editor: Fixed Platform title is displayed twice in the "Build Profiles" section.
    ([UUM-60699](https://issuetracker.unity3d.com/issues/platform-title-is-displayed-twice-in-the-build-profiles-section))

- Editor: Fixed profile list section grows bigger according to the longest build profile name.
    ([UUM-61844](https://issuetracker.unity3d.com/issues/build-profiles-add-build-profile-section-grows-slash-becomes-bigger-according-to-the-longest-build-profile-title))

- Editor: Fixed unexpected error while switching between branches.

- Editor: Hide a RenderMode field from Light Component in URP and removed related documentation.
    ([UUM-70283](https://issuetracker.unity3d.com/issues/important-slash-unimportant-setting-on-lights-doesnt-take-effect))

- Editor: Updated 7-Zip to 24.07.

- GI: Changed Adaptive Probe Volumes to store occlusion values for each light when using Mixed Lighting modes. This allows static objects to cast shadows onto dynamic objects by sampling the probe volume.
    ([UUM-44229](https://issuetracker.unity3d.com/issues/adaptive-probe-volume-is-incorrectly-baked-when-using-mixed-mode-light))

- Graphics: Added validation that SetVertexAttribute\(\) streams doesnt create gaps.
    ([UUM-72229](https://issuetracker.unity3d.com/issues/no-error-is-logged-when-calling-the-setvertexbufferparams-incorrectly))

- Graphics: Fixed a bug where material property block allocations were reported as "Unknown".
    ([UUM-71008](https://issuetracker.unity3d.com/issues/materialpropertyblocks-allocated-memory-is-displayed-under-unknown-when-observed-through-the-memory-profiler))

- Graphics: Fixed an issue where TextureImporter swizzling was applied later than expected during processing.
    ([UUM-46557](https://issuetracker.unity3d.com/issues/srgb-lineartogamma-is-only-applied-when-srgb-gammatolinear-unorm8tofloat-applies-linearisation-to-rgb-channels-before-swizzling))

- Graphics: Fixed crash on metal with depth-only clears coupled with hdr under some circumstances.
    ([UUM-73624](https://issuetracker.unity3d.com/issues/unity-crashes-or-an-error-metal-grabintorendertexture-mismatched-grab-pass-80-slash-92-is-thrown-and-the-game-view-becomes-corrupted-when-hdr-is-enabled-in-an-ios-module-after-enabling-and-disabling-the-frame-debugger-with-clear-flags-set-to-depth-only))

- Graphics: Fixed crash when opening a project that loads TSS files, if texture data is loaded on demand.
    ([UUM-71323](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-project-that-loads-tss-files))

- Graphics: \[Graphics\] Emit UI geometry when rendering to cube maps, while using mono camera, to match 2d render target behavior.
    ([UUM-2710](https://issuetracker.unity3d.com/issues/canvas-components-are-ignored-when-using-camera-dot-rendertocubemap))

- HDRP: Fixed a crash in HDRP when reaching the max amount of shadows on screen.
    ([UUM-73832](https://issuetracker.unity3d.com/issues/crash-on-burst-dot-initialize-dot-statics-when-exceeding-the-maximum-shadows-on-screen-value-in-player))

- HDRP: Fixed an out of range exception in HDRP when reaching the max amount of shadows on screen.
    ([UUM-73485](https://issuetracker.unity3d.com/issues/system-dot-indexoutofrangeexception-index-1-is-out-of-range-in-container-of-128-length-is-thrown-when-zooming-out-in-the-scene-view))

- iOS: Fixed release build failing to link if Debug.CheckIntegrity is used.
    ([UUM-73288](https://issuetracker.unity3d.com/issues/ios-undefined-symbol-error-is-thrown-in-xcode-when-using-debug-dot-checkintegrity))

- Kernel: Revert job system allocator optimization which could cause freezes.
    ([UUM-74556](https://issuetracker.unity3d.com/issues/quest-apps-lose-head-and-controller-tracking))

- Package Manager: Fixed the issue where incorrect reverse dependencies were shown in the Package Manager window.
    (UUM-72079)

- Physics: Fixed an issue where all Joint component types apart from HingeJoint would be treated as having their limit ranges \(-tau,+tau\) rather than \(-pi,+pi\) by default. This issue manifested as unstable/explosive initial motion of any joint system not using HingeJoint components.
    ([UUM-72854](https://issuetracker.unity3d.com/issues/jerky-initialization-of-joints-occurs-when-configurable-joint-limits-are-used))

- Physics: Fixed an issue where Colliders would skip over the root ArticulationBody due to initialization order. This would end up forcing the colliders to remain static and be ignored by the ArticulationBody components that they should be attached to.
    ([UUM-72958](https://issuetracker.unity3d.com/issues/the-parent-gameobject-in-the-articulation-body-tree-does-not-abide-by-the-box-collider-and-stops-the-movement-of-the-gameobject-before-the-collision-when-the-articulation-joint-type-is-prismatic))

- Physics 2D: Rigidbody2D.Slide now correctly uses the specified Physics2D.IgnoreCollision controls.
    ([UUM-59578](https://issuetracker.unity3d.com/issues/physics2d-dot-ignorecollision-does-not-ignore-collision-when-using-rigidbody2d-dot-slide-to-move))

- Prefabs: Ensure Awake is called after SetParent and MergePrefabInstances for all objects on duplicate.
    ([UUM-56488](https://issuetracker.unity3d.com/issues/changes-made-in-awake-function-with-executealways-attribute-are-overwritten-when-duplicating-prefab-with-a-parent))

- Scripting: Fixed an issue where code generated by MonoScriptInfoImporter was not considered generated by Roslyn analyzers.
    ([UUM-72953](https://issuetracker.unity3d.com/issues/failure-to-skip-analysis-of-code-generated-by-monoscriptinfogenerator-when-the-roslyn-analyzer-that-inherits-from-diagnosticanalyzer-is-used))

- Shadergraph: Fixed an issue where an HDRP fullscreen shader graph imported into a URP project would fail to import under some circumstances.
    ([UUM-55703](https://issuetracker.unity3d.com/issues/fullscreen-shader-graph-assets-are-unusable-when-imported-into-a-urp-project-and-have-both-urp-and-hdrp-as-active-targets-as-well-as-material-set-to-fullscreen))

- Shadergraph: Fixed shader graph built-in pipeline variants not getting stripped when an SRP is active.
    (UUM-69319)

- Shaders: Fixed a runtime crash that could occur when loading shader sub-program parameters.
    ([UUM-70213](https://issuetracker.unity3d.com/issues/linux-player-crash-on-shader-srpbatcherinfosetup-when-opening-player-build))

- SRP Core: Fixed _FOVEATED_RENDERING_NON_UNIFORM_RASTER shader compilation errors.
    ([UUM-67560](https://issuetracker.unity3d.com/issues/undeclared-identifier-foveated-rendering-non-uniform-raster-error-is-thrown-when-the-foveatedrenderingkeywords-dot-hlsl-file-is-not-included-in-a-custom-shader-and-the-rendering-path-is-set-to-forward-plus))

- Universal RP: Fixed an issue with enabling instancing at runtime for a Decal material.
    ([UUM-72363](https://issuetracker.unity3d.com/issues/urp-decal-instanced-rendering-breaks-and-spams-warnings-when-it-is-enabled-at-runtime))

- Version Control: Fixed "Collection was modified" error when doing multiple renames in a row.

- Version Control: Fixed "item with the same key has already been added" error.

- Version Control: Fixed check in error if nothing is selected in the pending changes tree.

- Version Control: Fixed column sorting in pending changes view.

- Version Control: Fixed error after renaming a parent branch of the working branch.

- Version Control: Fixed failure to delete a .meta file when deleting a private folder from the pending changes.

- Version Control: Fixed hang on domain reload.

- Version Control: Fixed missing incoming changes after removing a branch.

- Version Control: Fixed text cut-off in filter rules dialog.

- Version Control: Fixed undo &amp; check-in operations not working when the current scene was never saved.

- Version Control: Fixed variables's value becoming clear after resolving conflict in inspector.

- Version Control: Moving folders in the Editor now correctly use the UVCS "Move" operation.

- Version Control: Removed misleading indication about shelves.

- Version Control: Supported workspace name with non-latin characters in Pending Changes.

- Web: Fixed the Web platform name in Build Profiles window from WebGL to Web.
    (UUM-73258)

- WebGL: \[WebGPU\] Fixed error for a filtering sampler being incompatible with non-filtering binding.

- XR: Updating XR Interaction Toolkit \(com.unity.xr.interaction.toolkit\) to version 3.0.4.




## Package changes in 6000.0.9f1

## Packages updated

- com.unity.collab-proxy: [2.3.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.3//changelog/CHANGELOG.html) to [2.4.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.4//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [3.0.3](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html) to [3.0.4](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html)

- com.unity.transport: [2.1.0](https://docs.unity3d.com/Packages/com.unity.transport@2.1//changelog/CHANGELOG.html) to [2.3.0](https://docs.unity3d.com/Packages/com.unity.transport@2.3//changelog/CHANGELOG.html)