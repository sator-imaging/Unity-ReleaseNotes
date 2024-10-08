# Unity 2022.3.38f1 LTS
Published at Tue, 16 Jul 2024 13:52:35 GMT  
https://unity.com/releases/editor/whats-new/2022.3.38

# Known Issues in 2022.3.38f1

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

- Asset Importers: Unity crashes on strtol_l when importing a specific .obj file
    ([UUM-42697](https://issuetracker.unity3d.com/issues/unity-crashes-on-strtol-l-when-importing-a-specific-obj-file))

- DirectX12: Editor crashes when starting a new game session using Direct3D12 Graphics API
    ([UUM-74726](https://issuetracker.unity3d.com/issues/editor-crashes-when-starting-a-new-game-session-using-direct3d12-graphics-api))

- DirectX12: [DX12] Player crash on UnityMain when building HDRP Sample on Windows
    ([UUM-75100](https://issuetracker.unity3d.com/issues/dx12-player-crash-on-unitymain-when-building-hdrp-sample-on-windows))

- DOTS: Job allocator contention causes slow job execution
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- DOTS: [Android] [Entities] Build fails with the error “Asset has disappeared while building player to 'globalgamemanagers.assets' - path '', instancedID '-xxxxxx'“ when building
    ([UUM-41830](https://issuetracker.unity3d.com/issues/android-entities-build-fails-with-the-error-asset-has-disappeared-while-building-player-to-globalgamemanagers-dot-assets-path-instancedid-xxxxxx-when-building))

- Editor Platform: The "Hold On" dialog box persists when entering the Play Mode
    ([UUM-74916](https://issuetracker.unity3d.com/issues/the-hold-on-dialog-box-persists-when-entering-the-play-mode))

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



# 2022.3.38f1 Release Notes

## Improvements

- Animation: Improved Animation Mode performance when using custom properties.
    ([UUM-73525](https://issuetracker.unity3d.com/issues/the-editor-freezes-when-changes-are-made-in-the-timeline-window-and-a-large-number-of-animation-curve-bindings-and-gameobjects-are-loaded))

- Documentation: Added notes about player build cache to PostProcessScene docs.
    ([UUM-69256](https://issuetracker.unity3d.com/issues/the-postprocesssceneattribute-is-not-called-when-the-project-is-built-more-than-once))



## Fixes

- Android: AndroidX use is always true. Fixed problem with Gradle AAB build fail when Split App Binary is on, but there are no asset packs in the generated Gradle project.
    (UUM-73808)

- Android: Fixed crash when an AndroidJavaProxy method throws an exception and is called from multiple threads.
    ([UUM-60297](https://issuetracker.unity3d.com/issues/android-player-crashes-when-androidjavaproxy-which-throws-an-exception-is-called-from-multiple-threads))

- Android: Fixed player crash when changing cursor multiple times.
    ([UUM-74941](https://issuetracker.unity3d.com/issues/android-the-player-crashes-when-changing-cursor-multiple-times-on-android))

- Android: To add activity null handling in isInMultiWindowMode API.
    ([UUM-71574](https://issuetracker.unity3d.com/issues/android-the-player-crashes-at-isinmultiwindowmode-when-using-lifecycle-methods))

- Apple TV: Fixed tvOS simulator input crash.
    ([UUM-70232](https://issuetracker.unity3d.com/issues/tvos-project-crashes-on-startup-on-apple-tv-simulator-both-x86-64-and-arm64-architectures))

- Audio: Fixed an issue that would cause the pan control on audio sources to not work properly in some cases.
    ([UUM-65071](https://issuetracker.unity3d.com/issues/audiosource-stereo-pan-property-doesnt-fully-mute-the-right-or-left-channel-when-using-a-videoplayer-attached-to-an-audiosource-and-setting-the-option-to-1-or-1))

- Documentation: Fixed a typo in the Create your own overlay page of the documentation.

- Editor: Ensure we do not execute empty menu item from within the AddComponent window.
    ([UUM-64144](https://issuetracker.unity3d.com/issues/executemenuitem-failed-because-there-is-no-menu-named-error-is-thrown-when-clicking-just-below-create-and-add-in-the-add-component-window))

- Editor: Fixed a bug where UI Canvas using Screen Space render mode would use an incorrect game view size and behave erratically.
    ([UUM-73707](https://issuetracker.unity3d.com/issues/erratic-behavior-while-editing-ui-in-prefab-when-canvas-render-mode-is-set-to-screen-space-camera-option))

- Editor: Fixed an error when destroying a camera with a texture assigned to the TargetTexture property.
    ([UUM-2869](https://issuetracker.unity3d.com/issues/android-releasing-render-texture-that-is-set-as-camera-dot-targettexture-error-when-calling-resources-dot-unloadunusedassets))

- Editor: Fixed an issue with ordering of processing newly created ScriptableObjects. Awake\(\) is now the last step as expected and is no longer called twice.
    ([UUM-54568](https://issuetracker.unity3d.com/issues/assetpostprocessor-dot-onpostprocessallassets-is-called-twice-when-creating-an-asset-and-any-changes-to-serialized-fields-performed-in-the-first-call-are-not-saved))

- Editor: Fixed an issue with point cache and vector field that could cause unexpected import when referenced from VFX.
    (UUM-73877)

- Editor: Fixed crash when hot-loading renderdoc in editor and GPU Resident Drawer running.
    ([UUM-73405](https://issuetracker.unity3d.com/issues/crash-when-loading-renderdoc-in-a-specific-scene))

- Editor: Fixed failing importing of multi image EXR files with alternative channel names.
    ([UUM-62509](https://issuetracker.unity3d.com/issues/exr-import-fails-when-using-valid-exr-textures-from-alab-dataset))

- Editor: Fixed issues with menu item Id values going out of sync on windows.
    ([UUM-73047](https://issuetracker.unity3d.com/issues/custom-and-built-in-menu-items-stop-working-when-a-project-has-lots-of-menu-items))

- Editor: Fixed neutral Tonemapping artifacts when using 64-bit textures.
    ([UUM-55852](https://issuetracker.unity3d.com/issues/unlit-shader-graph-displays-incorrect-data-when-in-the-scene-view))

- Editor: Make Search Window available providers more consistant across the editor.
    ([UUM-72552](https://issuetracker.unity3d.com/issues/search-windows-opened-from-the-project-browser-and-windows-menu-act-differently))

- Graphics: Fixed blending artifacts on some old Adreno GPUs.
    ([UUM-72350](https://issuetracker.unity3d.com/issues/vulkan-android-visual-corruption-is-visible-on-some-android-devices-in-the-player-when-depth-of-field-is-enabled-in-global-volume-and-the-vulkan-graphics-api-is-selected))

- Graphics: Fixed Linear01DepthFromNear shader utility function on APIs with reversed Z buffer.
    ([UUM-19101](https://issuetracker.unity3d.com/issues/linear01depth-doesnt-return-different-values-depending-on-unity-reversed-z-when-graphics-api-is-not-openglcore))

- HDRP: Changed ProbeSettings.cubeResolution field from internal to public.
    ([UUM-74949](https://issuetracker.unity3d.com/issues/hdrp-probessettings-dot-cuberesolution-is-internal-and-can-not-be-changed-easilly))

- Input: Improved the performance of the Gamepad.SetMotorSpeeds\(\) script API.
    ([UUM-72692](https://issuetracker.unity3d.com/issues/gamepad-dot-setmotorspeeds-cpu-usage-is-3-times-higher-when-the-controller-is-connected-via-bluetooth))

- Package: Updated Cinemachine 2.10.1.

- Particles: Convert Particles trail vertex color to linear space when needed.
    ([UUM-71125](https://issuetracker.unity3d.com/issues/the-particle-system-trail-module-creates-trails-with-a-lighter-coloring-than-the-particles-when-the-color-space-is-set-to-linear))

- Particles: Fixed a freeze that occurs if user particle system jobs are completed immediately after schedule.
    ([UUM-74409](https://issuetracker.unity3d.com/issues/editor-freezes-when-opening-a-scene-containing-a-timeline))

- Particles: Updated ParticleSystem.Start\(\) documentation to reflect correct behavior.
    ([UUM-72281](https://issuetracker.unity3d.com/issues/the-particle-system-prewarm-flag-is-ignored-when-calling-the-start-function-after-the-stop-function))

- UI Toolkit: Fixed an issue where the source generator of the the Unity.Properties module was targeting net6 instead of netstandard2.0, causing issues in VisualStudio.
    (UUM-74852)

- UI Toolkit: Fixed element name being deleted when pressing the "ESC" key to cancel the renaming of an element in UI Builder.
    ([UUM-71820](https://issuetracker.unity3d.com/issues/element-name-is-deleted-when-pressing-the-esc-key-to-cancel-the-renaming-of-an-element-in-ui-builder))

- Undo System: Improved performance when recording property modifications for large object groups.
    ([UUM-53686](https://issuetracker.unity3d.com/issues/editor-hangs-for-several-seconds-when-changing-static-flags))

- VFX Graph: Blackboard could be out of the screen when the VFX Graph window was too small.
    ([UUM-65513](https://issuetracker.unity3d.com/issues/layout-elements-are-missing-when-the-vfx-graph-window-is-docked-horizontally))

- VFX Graph: Fixed SpawnIndex attribute when using instancing.
    ([UUM-74856](https://issuetracker.unity3d.com/issues/vfx-graph-spawnindex-values-are-wrong-with-instancing-on-and-several-vfx-instances))

- VFX Graph: Indeterministic skin mesh sampling when previous and current were fetch within the same VFX.
    (UUM-45920)

- VFX Graph: Use unknown particle count when count readback has never been received.
    ([UUM-71300](https://issuetracker.unity3d.com/issues/vfx-graph-effect-instance-stops-rendering-when-a-second-instance-of-the-same-effect-starts-2-frames-later))

- Video: \[Android\] Player with the specific Video clip crashes on "/apex/com.android.runtime/lib/bionic/libc.so \(__memcpy_a53+96\)" when the video is bundled with other video clips and Codec is set to VP8. The first few seconds of the video audio is distorted on the Android Player.
    ([UUM-73032](https://issuetracker.unity3d.com/issues/android-player-with-the-specific-video-clip-crashes-on-slash-apex-slash-com-dot-android-dot-runtime-slash-lib-slash-bionic-slash-libc-dot-so-memcpy-a53-plus-96-when-the-video-is-bundled-with-other-video-clips-and-codec-is-set-to-vp8))




## Package changes in 2022.3.38f1

## Packages updated

- com.unity.cinemachine: [2.10.0](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) to [2.10.1](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.28](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.31](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)