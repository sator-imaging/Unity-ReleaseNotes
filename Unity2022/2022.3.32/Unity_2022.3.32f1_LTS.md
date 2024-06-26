# Unity 2022.3.32f1 LTS
Tue, 04 Jun 2024 17:45:52 GMT  
https://unity.com/releases/editor/whats-new/2022.3.32

### Known Issues in 2022.3.32f1

- 3D Physics:  Crash on ujob_execute_job while using OverlapBoxCommand when collisions are more than maxHits
    ([UUM-71476](https://issuetracker.unity3d.com/issues/crash-on-ujob-execute-job-while-using-overlapboxcommand-when-collisions-are-more-than-maxhits))

- Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode
    ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Asset Importers: Crash on StackAllocator<0>::GetOverheadSize when importing the “POLYGON City - Low Poly 3D Art by Synty“ asset pack
    ([UUM-55981](https://issuetracker.unity3d.com/issues/crash-on-stackallocator-getoverheadsize-when-importing-the-polygon-city-low-poly-3d-art-by-synty-asset-pack))

- Asset Importers: Unity crashes on strtol_l when importing a specific .obj file
    ([UUM-42697](https://issuetracker.unity3d.com/issues/unity-crashes-on-strtol-l-when-importing-a-specific-obj-file))

- DOTS: [Android] [Entities] Build fails with the error “Asset has disappeared while building player to 'globalgamemanagers.assets' - path '', instancedID '-xxxxxx'“ when building
    ([UUM-41830](https://issuetracker.unity3d.com/issues/android-entities-build-fails-with-the-error-asset-has-disappeared-while-building-player-to-globalgamemanagers-dot-assets-path-instancedid-xxxxxx-when-building))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Lighting: [HDRP] Light doesn't bounce off terrains
    ([UUM-71171](https://issuetracker.unity3d.com/issues/hdrp-light-doesnt-bounce-off-terrains))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Scene Management: Crash on Transform::SetParent when duplicating a Prefab in the Hierarchy
    ([UUM-73287](https://issuetracker.unity3d.com/issues/crash-on-transform-setparent-when-duplicating-a-prefab-in-the-hierarchy))

- Texture: [AsyncLoadInEditor] Crash on memcpy when opening a project that loads TSS files
    ([UUM-71323](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-project-that-loads-tss-files))

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Universal RP: Objects are invisible in Scene view when using Wireframe Shading Mode
    ([UUM-36914](https://issuetracker.unity3d.com/issues/objects-are-invisible-in-scene-view-when-using-wireframe-shading-mode))



### 2022.3.32f1 Release Notes

#### API Changes

- Editor: Added: Exposed constructor of PooledObject.
    ([UUM-64168](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-implementing-iobjectpool-interface))

- URP: Added: RenderPipelineManager callbacks are raised from UniversalRenderPipeline.SingleCameraRequest.
    ([UUM-69268](https://issuetracker.unity3d.com/issues/urp-universalrenderpipeline-dot-singlecamerarequests-does-not-trigger-renderpipelinemanager-dot-endcontextrendering-for-cameras-rendered-with-the-request))



#### Fixes

- 2D: Fixed Case where there is high memory usage and crash on DynamicHeapAllocator::CreateTLSFBlock when opening project with Sprite Atlas V2 enabled.
    ([UUM-43709](https://issuetracker.unity3d.com/issues/high-memory-usage-and-crash-on-dynamicheapallocator-createtlsfblock-when-opening-project-with-sprite-atlas-v2-enabled))

- Android: Fixed issues where calling Cursor.visible on Android API 23 would cause a runtime error. Since https://developer.android.com/reference/android/view/PointerIcon is only available on API 24 or higher. Cursor.visible won't do anything in API 23.
    (UUM-72191)

- Android: Updated AndroidNativePlugin example in docs for all Android architectures.
    (UUM-72369)

- Android: WebcamTexture on android requires camera permission granted.
    ([UUM-45900](https://issuetracker.unity3d.com/issues/android-webcam-doesnt-render-when-the-app-is-launched-for-the-first-time-on-android))

- Animation: Fixed PlayableDirector fields that were not being updated when the Bindings section was expanded.
    ([UUM-71674](https://issuetracker.unity3d.com/issues/the-playabledirector-component-properties-are-not-being-updated-when-the-bindings-section-is-expanded))

- Audio: Fixed a bug that would cause the editor to crash if you delete and then re-add an audio listener component.
    ([UUM-61733](https://issuetracker.unity3d.com/issues/crash-adding-audiolistener-component-with-onaudiofilterread-crashes-the-editor))

- DX12: ComputeBuffer CopyCount returns correct value following multiple compute dispatches.
    ([UUM-66900](https://issuetracker.unity3d.com/issues/directx-12-copycomputebuffercount-is-getting-a-wrong-value-when-the-resource-transition-is-missing))

- Editor: 2D: Updated 2D Feature documentation link.
    ([UUM-70575](https://issuetracker.unity3d.com/issues/package-manager-feature-quick-start-links-open-up-old-documentation))

- Editor: Added rosbutness to splitter ControlId so it works with DataMode ui \(used in entity\).
    (UUM-67862)

- Editor: All indexes are created with Temp and External as exclude.
    (UUM-70905)

- Editor: Fixed both bugs related to PropertyEditor and Debug mode.
    (UUM-64257)

- Editor: Fixed issue where building in batch mode can open file explorer unexpectedly and cause a hang when running on headless windows servers.
    ([UUM-68288](https://issuetracker.unity3d.com/issues/crash-on-revealinfinder-when-building-a-project-in-headless-mode))

- Editor: Fixed not raising RenderPipelineTypeChanged callback if only scene view is active.
    ([UUM-70198](https://issuetracker.unity3d.com/issues/renderpipelinemanager-dot-activerenderpipelinetypechanged-does-not-detect-changes-when-changing-the-render-pipeline-asset-outside-of-play-mode))

- Editor: Fixed Project Advanced Search filtering if the user picked the Type selector.
    ([UUM-71128](https://issuetracker.unity3d.com/issues/macos-project-browsers-search-by-type-stops-working-after-importing-assets-into-a-project-and-searching-for-types-in-assets))

- Editor: Fixed saving layout will crash the linux editor.
    ([UUM-70626](https://issuetracker.unity3d.com/issues/linux-crash-on-guiview-processinputevent-when-editing-a-gameobject-slash-vfx-graph-or-saving-a-layout))

- Editor: Fixed thumbnail generation for assets who can be casted to texture.
    (UUM-70573)

- Editor: If multiple CustomEditor are registered for the same type only a single one gets instantiated \(still the case\). But the order of which CustomEditor gets instantiated is stable even if scripts are added or removed from the project.
    ([UUM-67599](https://issuetracker.unity3d.com/issues/custom-buttons-of-a-script-in-the-inspector-disappear-when-an-unrelated-script-is-deleted))

- Editor: IME input does not work with Input System when using Chinese \(Simplified\) input bug resolution.
    ([UUM-61922](https://issuetracker.unity3d.com/issues/ime-input-does-not-work-with-input-system-when-using-chinese-simplified-input))

- Editor: UnityEditor.Build.Content.ObjectIdentifier comparison operators have been changed to be more consistent and use all of the fields. This improves determinism for asset bundle builds.
    (UUM-71772)

- Graphics: Fixed depthrnormals render issue with a grabpass as the first pass on shader.
    (UUM-71175)

- Graphics: Fixed IUnityGraphicsMetal.CurrentCommandEncoder returning nil when there were no draw calls issued yet with current RenderTarget.
    (UUM-71813)

- iOS: Fixed view briefly distorting when rotating device with auto-rotation enabled.
    ([UUM-63417](https://issuetracker.unity3d.com/issues/visual-jumps-slash-screen-stretching-occurs-during-rotation-when-using-unityframework))

- Linux: Fixed touch freezes in Player when any mouse button is clicked.
    ([UUM-70659](https://issuetracker.unity3d.com/issues/linux-touch-freezes-in-player-when-any-mouse-button-is-clicked))

- Package Manager: Fixed Import Error Code: \(4\) warnings when a local package.json file is modified in the Editor.
    ([UUM-40830](https://issuetracker.unity3d.com/issues/import-error-code-4-warnings-are-infinitely-thrown-when-selecting-local-packages-modified-json-file))

- Shadergraph: Fixed an issue where the Baked GI Node was not displaying correctly after initially adding it to a graph.
    ([UUM-72436](https://issuetracker.unity3d.com/issues/sg-baked-gi-node-doesnt-have-inputs-on-creation))

- UI Toolkit: Added delay to showing DropwDonwFIeld menu during PointerDownEvent so that additional items can be added.
    ([UUM-72062](https://issuetracker.unity3d.com/issues/dropdownfield-options-added-with-pointerdownevent-are-not-shown-when-clicking-the-dropddownfield-for-the-first-time))

- UI Toolkit: Fixed some error when importing UXML asset when the system locale is in Turkish.
    ([UUM-71670](https://issuetracker.unity3d.com/issues/trying-to-read-value-of-type-dimension-while-reading-a-value-of-type-enum-is-thrown-when-the-system-language-is-set-to-turkish))




#### Package changes in 2022.3.32f1

#### Packages updated

- com.unity.addressables: [1.21.19](https://docs.unity3d.com/Packages/com.unity.addressables@1.21//changelog/CHANGELOG.html) to [1.21.21](https://docs.unity3d.com/Packages/com.unity.addressables@1.21//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.21.21](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.21//changelog/CHANGELOG.html) to [1.21.23](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.21//changelog/CHANGELOG.html)

- com.unity.splines: [2.6.0](https://docs.unity3d.com/Packages/com.unity.splines@2.6//changelog/CHANGELOG.html) to [2.6.1](https://docs.unity3d.com/Packages/com.unity.splines@2.6//changelog/CHANGELOG.html)