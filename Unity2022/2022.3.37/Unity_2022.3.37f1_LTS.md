# Unity 2022.3.37f1 LTS
Published at Tue, 09 Jul 2024 12:05:40 GMT  
https://unity.com/releases/editor/whats-new/2022.3.37

# Known Issues in 2022.3.37f1

- Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode
    ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))

- Asset - Database: Crash on "LMDB_Transaction::AbortAndRestart()" when creating 3D Mobile Template Project
    ([UUM-73995](https://issuetracker.unity3d.com/issues/crash-on-lmdb-transaction-abortandrestart-when-creating-3d-mobile-template-project))

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Asset - Database: Crash on SourceAssetDBReadTxn::SourceAssetDBReadTxn when opening a project after deleting an Asset
    ([UUM-75191](https://issuetracker.unity3d.com/issues/crash-on-sourceassetdbreadtxn-sourceassetdbreadtxn-when-opening-a-project-after-deleting-an-asset))

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

- Hybrid Renderer: Crash when loading RenderDoc in a specific Scene
    ([UUM-73405](https://issuetracker.unity3d.com/issues/crash-when-loading-renderdoc-in-a-specific-scene))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Mono: [TypeCache] Crash on RaiseException when opening a specific project
    ([UUM-66498](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-opening-a-specific-project))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Scene Management: Crash on Transform::SetParent when duplicating a Prefab in the Hierarchy
    ([UUM-73287](https://issuetracker.unity3d.com/issues/crash-on-transform-setparent-when-duplicating-a-prefab-in-the-hierarchy))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Vulkan: [Linux][Vulkan] Crash when using Nvidia drivers >545 and graphics API set to Vulkan
    ([UUM-73447](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-when-using-nvidia-drivers-545-and-graphics-api-set-to-vulkan))



# 2022.3.37f1 Release Notes

## Improvements

- Mono: Added Unity Embedding API to load assembly refs with error checking.

- VisionOS: Plugin path "Assets/Plugins/VisionOS/" is now recognized and auto-selects VisionOS as compatible platform.



## Fixes

- Android: Fixed detection of Play Asset Delivery support to avoid problems if there is play.core dependency in the project.
    (UUM-74252)

- Asset Bundles: Only call CollectAllSpriteAtlasesAndPack once when building AssetBundles.
    (UUM-73147)

- Editor: Hide a RenderMode field from Light Component in URP and removed related documentation.
    ([UUM-70283](https://issuetracker.unity3d.com/issues/important-slash-unimportant-setting-on-lights-doesnt-take-effect))

- Editor: Motion Vector pass also filter objects by Opaque Mask.
    ([UUM-72748](https://issuetracker.unity3d.com/issues/motion-vectors-for-an-object-are-included-in-the-urp-motion-vector-pass-when-the-objects-layer-mask-is-filtered-out))

- Graphics: Added validation that SetVertexAttribute\(\) streams doesnt create gaps.
    ([UUM-72229](https://issuetracker.unity3d.com/issues/no-error-is-logged-when-calling-the-setvertexbufferparams-incorrectly))

- Graphics: Fixed broken URL for documentation on Texture2D.
    ([UUM-74607](https://issuetracker.unity3d.com/issues/texture-2d-reference-links-to-missing-documentation))

- GraphView: Some Mac keyboard events not having mousePosition in the editor.
    ([UUM-62291](https://issuetracker.unity3d.com/issues/vfx-node-creation-window-opens-at-the-top-left-corner-of-the-screen-when-using-spacebar))

- IL2CPP: Fixed possible crash in fully shared generic code at calls at the generic code generation limit.
    (UUM-73629)

- iOS: Don't symlink .xcprivacy files when "Symlink Sources" build option is selected.
    (UUM-72375)

- iOS: Fixed touches getting stuck when orientation is forced from code while touching the screen.
    ([UUM-53903](https://issuetracker.unity3d.com/issues/ios-input-system-enhancedtouch-touches-persist-when-released-after-tapping-and-holding-and-then-changing-screen-dot-orientation))

- License: Fixed a bug where normal floating communication regarding feature status would generate too many log messages.

- License: Fixed a bug where web proxy credentials would not be found when added through a dialog triggered by macOS/Safari after web proxy auto-discovery was enabled.

- macOS: Fixed forward and back buttons being recognized as middle button.
    ([UUM-70259](https://issuetracker.unity3d.com/issues/macos-forward-and-backward-mouse-buttons-are-recognized-as-middle-mouse-button))

- Mono: Fixed memory leak when validating a SSL certificate.
    ([UUM-72433](https://issuetracker.unity3d.com/issues/ios-memory-leaks-when-using-the-sslstream-class))

- Physics: Fixed a memory corruption for OverlapXCommand APIs where we would end up writing out of bounds into the results array. Effectively corrupting the adjacent memory block, this would eventually lead to a crash, either immediately or shortly after the operation concluded.
    ([UUM-71476](https://issuetracker.unity3d.com/issues/crash-on-ujob-execute-job-while-using-overlapboxcommand-when-collisions-are-more-than-maxhits))

- Player: Fixed possible crash on shut down when custom player loop is set.
    ([UUM-72551](https://issuetracker.unity3d.com/issues/ios-crash-on-il2cpp-gc-gchandle-free-when-app-returns-to-foreground))

- Prefabs: Ensure Awake is called after SetParent and MergePrefabInstances for all objects on duplicate.
    ([UUM-56488](https://issuetracker.unity3d.com/issues/changes-made-in-awake-function-with-executealways-attribute-are-overwritten-when-duplicating-prefab-with-a-parent))

- UI Toolkit: UI Toolkit foldout interaction enabled on controllers.
    ([UUM-73752](https://issuetracker.unity3d.com/issues/unable-to-select-ui-toolkit-foldout-element-when-using-a-gamepad-controller))

- Universal RP: Fixed an issue with enabling instancing at runtime for a Decal material.
    ([UUM-72363](https://issuetracker.unity3d.com/issues/urp-decal-instanced-rendering-breaks-and-spams-warnings-when-it-is-enabled-at-runtime))

- VFX Graph: Fixed VFX graph renders the wrong mesh when using different exposed meshes with instancing enabled.
    (UUM-59091)

- VFX Graph: Flickering with VFX using instancing and overriding an exposed texture with an empty texture.
    (UUM-74322)

- VFX Graph: Force culling when VFX rendering is disabled.
    (UUM-71482)

- VFX Graph: Improved how the sleep state is updated for particle systems receiving GPU events.
    ([UUM-73758](https://issuetracker.unity3d.com/issues/the-visual-effect-gpu-event-is-forced-into-sleep-until-another-event-is-sent-when-the-visual-effect-consists-of-two-particle-systems-that-communicate-with-trigger-event-set-to-on-die))

- VFX Graph: Wrong mesh rendered with instancing, when using multi mesh output and exposed submesh mask.
    (UUM-74240)

- VisionOS: Consider plugins compatibility even if their .meta files are empty \(default import settings\).
    (UUM-72377)




## Package changes in 2022.3.37f1

## Packages updated

- com.unity.xr.arcore: [5.1.4](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.1//changelog/CHANGELOG.html) to [5.1.5](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.1//changelog/CHANGELOG.html)

- com.unity.xr.arfoundation: [5.1.4](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.1//changelog/CHANGELOG.html) to [5.1.5](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.1//changelog/CHANGELOG.html)

- com.unity.xr.arkit: [5.1.4](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.1//changelog/CHANGELOG.html) to [5.1.5](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.1//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk: [1.0.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.1//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk.tools: [1.0.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.1//changelog/CHANGELOG.html)