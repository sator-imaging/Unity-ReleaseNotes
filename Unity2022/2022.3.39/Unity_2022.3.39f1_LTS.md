# Unity 2022.3.39f1 LTS
Published at Tue, 23 Jul 2024 16:04:16 GMT  
https://unity.com/releases/editor/whats-new/2022.3.39

# Known Issues in 2022.3.39f1

- Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode
    ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Asset - Database: OnAfterDeserialize is not called when Prefabs are instantiated using InstantiateAsync
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- Asset Bundles: The resource is not properly referenced when there is a dependency on another asset bundle
    ([UUM-74871](https://issuetracker.unity3d.com/issues/the-resource-is-not-properly-referenced-when-there-is-a-dependency-on-another-asset-bundle))

- Asset Importers: Crash on StackAllocator<0>::GetOverheadSize when importing the “POLYGON City - Low Poly 3D Art by Synty“ asset pack
    ([UUM-55981](https://issuetracker.unity3d.com/issues/crash-on-stackallocator-getoverheadsize-when-importing-the-polygon-city-low-poly-3d-art-by-synty-asset-pack))

- DirectX12: Editor crashes when starting a new game session using Direct3D12 Graphics API
    ([UUM-74726](https://issuetracker.unity3d.com/issues/editor-crashes-when-starting-a-new-game-session-using-direct3d12-graphics-api))

- DOTS: [Android] [Entities] Build fails with the error “Asset has disappeared while building player to 'globalgamemanagers.assets' - path '', instancedID '-xxxxxx'“ when building
    ([UUM-41830](https://issuetracker.unity3d.com/issues/android-entities-build-fails-with-the-error-asset-has-disappeared-while-building-player-to-globalgamemanagers-dot-assets-path-instancedid-xxxxxx-when-building))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Material: Crash on SourceAssetDBReadTxn::SourceAssetDBReadTxn when opening a project after deleting an Asset
    ([UUM-75191](https://issuetracker.unity3d.com/issues/crash-on-sourceassetdbreadtxn-sourceassetdbreadtxn-when-opening-a-project-after-deleting-an-asset))

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

- UI Toolkit Controls: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- UI Toolkit Framework: "TextureImporterInspector.OnInspectorGUI must call ApplyRevertGUI to avoid unexpected behaviour." thrown when selecting Asset then selecting and deselecting Texture 2D
    ([UUM-35998](https://issuetracker.unity3d.com/issues/textureimporterinspector-dot-oninspectorgui-must-call-applyrevertgui-to-avoid-unexpected-behaviour-dot-thrown-when-selecting-asset-then-selecting-and-deselecting-texture-2d))

- Vulkan: [Linux][Vulkan] Crash when using Nvidia drivers >545 and graphics API set to Vulkan
    ([UUM-73447](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-when-using-nvidia-drivers-545-and-graphics-api-set-to-vulkan))



# 2022.3.39f1 Release Notes

## Improvements

- Editor: Added details to the "incompatible keyword space" error message which is occasionally generated by shaders.
    ([UUM-58563](https://issuetracker.unity3d.com/issues/state-comes-from-incompatible-keyword-space-error-not-very-informative))



## Fixes

- AI: Fixed an issue where NavMeshData belonging to a scene would remain loaded after the scene had been offloaded. This issue only occurred when the "Do not reload scene"-option has been checked in the editor settings.
    ([UUM-29346](https://issuetracker.unity3d.com/issues/navmesh-from-previous-scene-is-visible-after-going-into-play-mode-when-reload-scene-is-toggled-off))

- Animation: Fixed additive animations ever increasing non animated values.
    ([UUM-68376](https://issuetracker.unity3d.com/issues/gameobject-continues-to-increase-in-scale-when-the-animation-layers-blending-is-set-to-additive))

- DX12: Corrected unbind counter resources to prevent GPU crash.
    ([UUM-75100](https://issuetracker.unity3d.com/issues/dx12-player-crash-on-unitymain-when-building-hdrp-sample-on-windows))

- DX12: Fixed incorrect values for GetNextFrameFenceValue\(\) in render plugins.
    (UUM-72389)

- Editor: Fixed wrong unity version in gradle overview documentation.
    (UUM-75674)

- Graphics: Fixed crash when using SRP, Handle.DrawOutline\(\) and filtering the hierarchy.
    ([UUM-67677](https://issuetracker.unity3d.com/issues/crash-on-camera-releasecamerastackrenderingstate-when-searching-in-hierarchy))

- Graphics: The condition for the "Graphics.CopyTexture with a region will not copy readable texture data for compressed formats" warnings has been fixed to match the documentation so that when a CPU copy would not normally be attempted \(ie., at least one texture is not readable\), the warnings will not appear.
    ([UUM-73721](https://issuetracker.unity3d.com/issues/graphics-dot-copytexture-with-a-region-will-not-copy-readable-texture-data-for-compressed-formats-warnings-are-thrown-when-copying-compressed-texture-regions))

- Package Manager: Fixed Exception Thrown When Minor Unity Version is Zero.
    ([UUM-73851](https://issuetracker.unity3d.com/issues/invalid-unity-version-6000-dot-0-is-thrown-when-the-major-version-is-set-to-6000-and-minor-to-0))

- Particles: Fixed crash when calling Camera.Render during OnApplicationQuit.
    ([UUM-55832](https://issuetracker.unity3d.com/issues/crash-when-calling-camera-dot-render-during-onapplicationquit-while-cast-shadows-is-checked-in-the-particle-system-component))

- Shadergraph: Fixed issues with the Feature Examples sample and Production Ready Shaders sample.
    (UUM-75425)

- UI Toolkit: Fixed a stack overflow and provided users with proper logs explaining the situation when it occurs.
    ([UUM-69438](https://issuetracker.unity3d.com/issues/editor-crashes-freezes-or-throws-a-stackoverflowexception-error-when-selecting-an-element-within-the-graphwindow))

- VFX Graph: Fixed Screen Space Size block in Shader Graph outputs.
    (UUM-64713)

- Video: Memory increases gradually when UWP webcam is opened/closed.
    ([UUM-62347](https://issuetracker.unity3d.com/issues/memory-increases-gradually-when-the-camera-is-opened-and-closed))

- Windows: Fixed issue with non-native Refreshrate not being restored in Exclusive Fullscreen mode upon restart.
    ([UUM-62542](https://issuetracker.unity3d.com/issues/player-refresh-rate-is-not-restored-after-restarting-when-setting-the-refresh-rate-to-a-non-native-one-in-exclusivefullscreen-mode))




## Package changes in 2022.3.39f1

## Packages updated

- com.unity.services.friends: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html)

- com.unity.services.lobby: [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.1//changelog/CHANGELOG.html) to [1.2.2](https://docs.unity3d.com/Packages/com.unity.services.lobby@1.2//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.2.3](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html) to [1.2.6](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html)