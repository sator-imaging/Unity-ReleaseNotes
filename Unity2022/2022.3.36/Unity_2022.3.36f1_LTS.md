# Unity 2022.3.36f1 LTS
Published at Tue, 02 Jul 2024 17:23:09 GMT  
https://unity.com/releases/editor/whats-new/2022.3.36

# Known Issues in 2022.3.36f1

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

- Asset Bundles: The resource is not properly referenced when there is a dependency on another asset bundle
    ([UUM-74871](https://issuetracker.unity3d.com/issues/the-resource-is-not-properly-referenced-when-there-is-a-dependency-on-another-asset-bundle))

- Asset Importers: Crash on StackAllocator<0>::GetOverheadSize when importing the “POLYGON City - Low Poly 3D Art by Synty“ asset pack
    ([UUM-55981](https://issuetracker.unity3d.com/issues/crash-on-stackallocator-getoverheadsize-when-importing-the-polygon-city-low-poly-3d-art-by-synty-asset-pack))

- Asset Importers: Unity crashes on strtol_l when importing a specific .obj file
    ([UUM-42697](https://issuetracker.unity3d.com/issues/unity-crashes-on-strtol-l-when-importing-a-specific-obj-file))

- DirectX12: Editor crashes when starting a new game session using Direct3D12 Graphics API
    ([UUM-74726](https://issuetracker.unity3d.com/issues/editor-crashes-when-starting-a-new-game-session-using-direct3d12-graphics-api))

- DOTS: Job allocator contention causes slow job execution
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- DOTS: [Android] [Entities] Build fails with the error “Asset has disappeared while building player to 'globalgamemanagers.assets' - path '', instancedID '-xxxxxx'“ when building
    ([UUM-41830](https://issuetracker.unity3d.com/issues/android-entities-build-fails-with-the-error-asset-has-disappeared-while-building-player-to-globalgamemanagers-dot-assets-path-instancedid-xxxxxx-when-building))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Menu Management: Custom and built-in menu items stop working when a project has lots of menu items
    ([UUM-73047](https://issuetracker.unity3d.com/issues/custom-and-built-in-menu-items-stop-working-when-a-project-has-lots-of-menu-items))

- Mono: [TypeCache] Crash on RaiseException when opening a specific project
    ([UUM-66498](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-opening-a-specific-project))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Scene Management: Crash on Transform::SetParent when duplicating a Prefab in the Hierarchy
    ([UUM-73287](https://issuetracker.unity3d.com/issues/crash-on-transform-setparent-when-duplicating-a-prefab-in-the-hierarchy))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- Texture: [AsyncLoadInEditor] Crash on memcpy when opening a project that loads TSS files
    ([UUM-71323](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-project-that-loads-tss-files))

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Vulkan: [Linux][Vulkan] Crash when using Nvidia drivers >545 and graphics API set to Vulkan
    ([UUM-73447](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-when-using-nvidia-drivers-545-and-graphics-api-set-to-vulkan))



# 2022.3.36f1 Release Notes

## Changes

- Entities Graphics: Added support for BRG LOD cross fade in the URP shaders.

- Version Control: Added "Undo unchanged" and "Undo checkouts keeping changes" options to pending changes view.

- Version Control: Changed the default ignore.conf to not ignore itself anymore.

- Version Control: Removed focus redirection after Check-in.



## Fixes

- Build System: Fixed a potential crash when building.
    ([UUM-72309](https://issuetracker.unity3d.com/issues/crash-on-mono-array-length-when-building-a-project))

- Editor: Fixed a crash when interacting with a shader variant collection containing shaders with dynamic branch keywords after de-/serializing the collection.
    ([UUM-73491](https://issuetracker.unity3d.com/issues/crash-on-free-alloc-internal-when-clearing-shader-variants-in-certain-projects))

- Editor: Fixed a log error when falling back to CPU Lightmapping in Editor NoGraphics mode.
    ([UUM-68496](https://issuetracker.unity3d.com/issues/builds-in-strict-mode-fail-when-lightmapper-falls-back-to-cpu))

- Editor: Fixed an issue where Texture.SetTextureSetting would take invalid values.
    ([UUM-63703](https://issuetracker.unity3d.com/issues/sprite-is-not-generated-when-its-texture-settings-are-changed-via-textureimportersettings))

- Editor: Fixed crash in LMDB_Transaction::AbortAndRestart\(\).
    (UUM-70115)

- Editor: Fixed LinuxEditor crash calling WarpCursorPosition outside of PlayMode.
    ([UUM-71828](https://issuetracker.unity3d.com/issues/linux-crash-on-newinput-mousecallbacks-ioctl-when-warpcursorposition-function-is-called))

- Editor: Fixed the issue where deleting a symlink removes the target file.
    (UUM-35170)

- Editor: Fixed the serialized property becoming invalid whilst changing prefab fields via dropdown.
    ([UUM-72761](https://issuetracker.unity3d.com/issues/nulleferenceexception-serializedobject-of-serializedproperty-has-been-disposed-dot-is-thrown-when-changing-layermask-in-the-inspector))

- Editor: Fixed unexpected error while switching between branches.

- Editor: Improved setlocale LC_NUMERIC guards.
    (UUM-58980)

- Editor: Revert job system allocator optimization which could cause freezes.
    ([UUM-74556](https://issuetracker.unity3d.com/issues/quest-apps-lose-head-and-controller-tracking))

- Graphics: Fixed a bug where material property block allocations were reported as "Unknown".
    ([UUM-71008](https://issuetracker.unity3d.com/issues/materialpropertyblocks-allocated-memory-is-displayed-under-unknown-when-observed-through-the-memory-profiler))

- Graphics: Fixed crash when opening a project that loads TSS files, if texture data is loaded on demand.
    ([UUM-71323](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-project-that-loads-tss-files))

- Graphics: Fixed Vulkan native rendering plugin returning an invalid texture when sampler configuration is updated.
    ([UUM-73757](https://issuetracker.unity3d.com/issues/nativeplugin-vulkan-image-gets-deleted-while-in-use-and-accesstexture-returns-an-invalid-texture-causing-a-crash-or-corruption-when-qualitysettings-dot-anisotropicfiltering-is-called))

- Prefabs: Disabled Show Overrides reference patching.
    ([UUM-71887](https://issuetracker.unity3d.com/issues/the-serialized-array-of-serializereference-objects-is-missing-entry-for-refid-2-error-is-thrown-when-saving-a-prefab-with-serializereference-overrides-and-showoverrides-is-enabled))

- Scripting: Fixed an issue where code generated by MonoScriptInfoImporter was not considered generated by Roslyn analyzers.
    ([UUM-72953](https://issuetracker.unity3d.com/issues/failure-to-skip-analysis-of-code-generated-by-monoscriptinfogenerator-when-the-roslyn-analyzer-that-inherits-from-diagnosticanalyzer-is-used))

- Serialization: Fixed Inspector window with scrollbar is unworkable when modifying and saving the material's property.
    ([UUM-58151](https://issuetracker.unity3d.com/issues/inspector-with-the-scrollbar-is-unusable-when-material-properties-are-edited-and-the-scene-is-saved))

- Shadergraph: Added support for perceptual color mode for gradients in shader graph.
    ([UUM-72278](https://issuetracker.unity3d.com/issues/the-gradient-shader-is-inverted-when-using-the-perceptual-blend-mode))

- Shaders: Fixed a runtime crash that could occur when loading shader sub-program parameters.
    ([UUM-70213](https://issuetracker.unity3d.com/issues/linux-player-crash-on-shader-srpbatcherinfosetup-when-opening-player-build))

- SRP Core: Fixed _FOVEATED_RENDERING_NON_UNIFORM_RASTER shader compilation errors.
    ([UUM-67560](https://issuetracker.unity3d.com/issues/undeclared-identifier-foveated-rendering-non-uniform-raster-error-is-thrown-when-the-foveatedrenderingkeywords-dot-hlsl-file-is-not-included-in-a-custom-shader-and-the-rendering-path-is-set-to-forward-plus))

- UI Toolkit: Slider element was not controlled correctly in players when navigating in the same direction as the element.
    ([UUM-74257](https://issuetracker.unity3d.com/issues/ui-toolkit-slider-element-is-not-controlled-correctly-when-using-a-gamepad-controller-1))

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

- Video: Editor freezes when playing videos with playback speed value &lt;1 and setting time via started callback.
    ([UUM-73115](https://issuetracker.unity3d.com/issues/editor-freezes-when-playing-videos-from-url-with-playback-speed-value-1-and-setting-time-via-started-callback))




## Package changes in 2022.3.36f1

## Packages updated

- com.unity.collab-proxy: [2.3.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.3//changelog/CHANGELOG.html) to [2.4.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.4//changelog/CHANGELOG.html)