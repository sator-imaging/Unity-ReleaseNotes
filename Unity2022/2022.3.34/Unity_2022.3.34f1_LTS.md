# Unity 2022.3.34f1 LTS
Tue, 18 Jun 2024 11:27:05 GMT  
https://unity.com/releases/editor/whats-new/2022.3.34

# Known Issues in 2022.3.34f1

- 3D Physics:  Crash on ujob_execute_job while using OverlapBoxCommand when collisions are more than maxHits
    ([UUM-71476](https://issuetracker.unity3d.com/issues/crash-on-ujob-execute-job-while-using-overlapboxcommand-when-collisions-are-more-than-maxhits))

- Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode
    ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))

- Asset - Database: Crash on "LMDB_Transaction::AbortAndRestart()" when creating 3D Mobile Template Project
    ([UUM-73995](https://issuetracker.unity3d.com/issues/crash-on-lmdb-transaction-abortandrestart-when-creating-3d-mobile-template-project))

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Asset - Database: OnAfterDeserialize is not called when Prefabs are instantiated using InstantiateAsync
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- Asset Importers: Crash on StackAllocator<0>::GetOverheadSize when importing the “POLYGON City - Low Poly 3D Art by Synty“ asset pack
    ([UUM-55981](https://issuetracker.unity3d.com/issues/crash-on-stackallocator-getoverheadsize-when-importing-the-polygon-city-low-poly-3d-art-by-synty-asset-pack))

- Asset Importers: Unity crashes on strtol_l when importing a specific .obj file
    ([UUM-42697](https://issuetracker.unity3d.com/issues/unity-crashes-on-strtol-l-when-importing-a-specific-obj-file))

- DOTS: Job allocator contention causes slow job execution
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- DOTS: [Android] [Entities] Build fails with the error “Asset has disappeared while building player to 'globalgamemanagers.assets' - path '', instancedID '-xxxxxx'“ when building
    ([UUM-41830](https://issuetracker.unity3d.com/issues/android-entities-build-fails-with-the-error-asset-has-disappeared-while-building-player-to-globalgamemanagers-dot-assets-path-instancedid-xxxxxx-when-building))

- Editor Platform: Building freezes when building Universal 3D Sample/Cinematic Studio Project
    ([UUM-73997](https://issuetracker.unity3d.com/issues/building-freezes-when-building-universal-3d-sample-slash-cinematic-studio-project))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Lighting: [HDRP] Light doesn't bounce off terrains
    ([UUM-71171](https://issuetracker.unity3d.com/issues/hdrp-light-doesnt-bounce-off-terrains))

- Mono: [TypeCache] Crash on RaiseException when opening a specific project
    ([UUM-66498](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-opening-a-specific-project))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Scene Management: Crash on Transform::SetParent when duplicating a Prefab in the Hierarchy
    ([UUM-73287](https://issuetracker.unity3d.com/issues/crash-on-transform-setparent-when-duplicating-a-prefab-in-the-hierarchy))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- SRP XR: [Quest] Error “ArgumentOutOfRangeException: Index was out of range." is present when GameObject with Mesh Renderer component that has Material attached is selected in Hierarchy
    ([UUM-73234](https://issuetracker.unity3d.com/issues/quest-error-argumentoutofrangeexception-index-was-out-of-range-dot-is-present-when-gameobject-with-mesh-renderer-component-that-has-material-attached-is-selected-in-hierarchy))

- Texture: [AsyncLoadInEditor] Crash on memcpy when opening a project that loads TSS files
    ([UUM-71323](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-project-that-loads-tss-files))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Vulkan: [Linux][Vulkan] Crash when using Nvidia drivers >545 and graphics API set to Vulkan
    ([UUM-73447](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-when-using-nvidia-drivers-545-and-graphics-api-set-to-vulkan))



# 2022.3.34f1 Release Notes

## Improvements

- Package: Release Recorder 4.0.3.

- UI Toolkit: UI Elements: Improved performance of MultiColumnListView and MultiColumnTreeView when changing the visibility status of columns.<br>
    A rebuild will now be scheduled instead of performed after each status change.
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))



## Fixes

- 2D: Fixed issue where the outline detail is reset to 0 for a Sprite Rect in the Sprite Editor when an outline is pasted onto a Sprite Rect.
    ([UUM-72965](https://issuetracker.unity3d.com/issues/sprite-editor-reverts-the-outline-detail-parameter-to-0-when-a-copied-outline-is-pasted))

- Android: Fixed audio output underflow on Vivo phones.
    ([UUM-56324](https://issuetracker.unity3d.com/issues/android-audio-clips-are-played-with-audible-glitches-when-playing-through-vivo-model-phones))

- Android: Fixed crash on Xclipse GPU based devices when setting Buffer Debug name on OpenGLES3 and Development build settings.
    ([UUM-65666](https://issuetracker.unity3d.com/issues/android-graphics-the-player-crashes-with-gfxdeviceworker-runcommand-error-when-both-opengles3-and-development-build-are-selected))

- Android: Input.location will work correctly even if old input system disabled.
    ([UUM-73469](https://issuetracker.unity3d.com/issues/android-locationservice-stuck-initializing-with-new-inputsystem))

- Asset Bundles: Don't add hash to the manifest file name when building AssetBundles.
    ([UUM-66821](https://issuetracker.unity3d.com/issues/scene-assetbundle-manifest-file-names-have-hashes-attached-when-assetbundles-are-built))

- Editor: Drag and drop operations performed on files within the currently open projects' folder should now succeed on Windows.
    ([UUM-54537](https://issuetracker.unity3d.com/issues/dragperformevent-is-not-called-when-files-from-the-project-folder-are-used))

- Editor: Fixed a bug where web proxy credentials would not be found when added through a dialog triggered by macOS/Safari after web proxy auto-discovery was enabled.

- Editor: Fixed wireframe not rendering when using Vulkan.
    ([UUM-36914](https://issuetracker.unity3d.com/issues/objects-are-invisible-in-scene-view-when-using-wireframe-shading-mode))

- Editor: Resolved a crash issue arising from the use of a Skinned Mesh Renderer with the DX12 rendering API.
    ([UUM-70289](https://issuetracker.unity3d.com/issues/crash-on-d3d12getinterface-when-enabling-a-gameobject-using-a-sample-skinned-mesh-node))

- GI: Fixed crash when iterating on lights in lightmap Auto baking mode.
    ([UUM-71599](https://issuetracker.unity3d.com/issues/crash-on-replacetexturedata-when-rapidly-changing-light-intensity))

- Graphics: Fixed applying a wrong viewport when a deferred camera uses a modified viewport together with a user-defined render target.
    ([UUM-70711](https://issuetracker.unity3d.com/issues/gameobjects-with-a-material-derived-from-a-custom-lighting-surface-shader-are-displayed-as-skewed-on-quads-when-the-cameras-width-and-height-properties-of-the-viewport-rect-are-lower-than-1))

- Graphics: Fixed by converting any linear format parameter to non linear if there is discrepancy between the actual resource format and what is provided.
    ([UUM-69379](https://issuetracker.unity3d.com/issues/xr-simulation-error-d3d11-failed-to-create-2d-texture-shader-resource-view-id-equals-1324-d3d-error-was-80070057-on-windows-with-directx-graphics-api))

- Graphics: Fixed Deferred Depth texture dimensions mismatch when modifying Camera's Viewport Rect.
    ([UUM-65233](https://issuetracker.unity3d.com/issues/shaders-cameradepthtexture-is-not-read-when-the-camera-is-rendering-to-a-rendertexture-and-has-a-reduced-viewport))

- HDRP: Fixed an issue where the default terrain shader for HDRP was outputting incorrect albedo values to the lightmapper.
    ([UUM-71171](https://issuetracker.unity3d.com/issues/hdrp-light-doesnt-bounce-off-terrains))

- Package Manager: Package Manager: Displaying a console warning when the user attempts to install a git package while another installation is in progress, explaining the reason for the operation's failure.
    ([UUM-63744](https://issuetracker.unity3d.com/issues/just-the-first-package-is-being-installed-and-no-error-slash-warning-message-is-logged-when-installing-two-packages-using-add-package-from-git-url))

- Player: Fixed player memory leak when managed reference registry was destroyed.
    ([UUM-72074](https://issuetracker.unity3d.com/issues/memory-leaks-when-instantiating-objects-with-serializereference))

- Universal RP: Fixed incorrect scaling in copy depth pass when dynamic resolution is enabled.
    ([UUM-60392](https://issuetracker.unity3d.com/issues/scalablebuffermanager-does-not-scale-depth-buffer-correctly-when-using-dynamic-resolution-in-urp))

- VFX Graph: Leak while spamming ReInit.
    ([UUM-71455](https://issuetracker.unity3d.com/issues/vfx-graph-memory-leak-when-calling-the-clearpropertybinders-and-addremovevfxproperty))

- Windows: Fixed a Windows bug, where an audio device that returns a mal-formed UUID string could crash the Windows Editor or player.
    ([UUM-36106](https://issuetracker.unity3d.com/issues/crash-on-fmod-outputwasapi-parseuuidstring-when-changing-sound-input-to-a-misconfigured-microphone))




## Package changes in 2022.3.34f1

## Packages updated

- com.unity.recorder: [4.0.2](https://docs.unity3d.com/Packages/com.unity.recorder@4.0//changelog/CHANGELOG.html) to [4.0.3](https://docs.unity3d.com/Packages/com.unity.recorder@4.0//changelog/CHANGELOG.html)