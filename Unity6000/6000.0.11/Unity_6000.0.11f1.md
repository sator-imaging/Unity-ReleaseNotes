# Unity 6000.0.11f1
Published at Wed, 17 Jul 2024 10:16:09 GMT  
https://unity.com/releases/editor/whats-new/6000.0.11

# Known Issues in 6000.0.11f1

- Asset - Database: OnAfterDeserialize is not called when Prefabs are instantiated using InstantiateAsync
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- Asset Bundles: The resource is not properly referenced when there is a dependency on another asset bundle
    ([UUM-74871](https://issuetracker.unity3d.com/issues/the-resource-is-not-properly-referenced-when-there-is-a-dependency-on-another-asset-bundle))

- DirectX12: Crash on D3D12 when entering Play Mode in High Definition 3D Core project's Environment scene
    ([UUM-74769](https://issuetracker.unity3d.com/issues/crash-on-d3d12-when-entering-play-mode-in-high-definition-3d-core-projects-environment-scene))

- DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when selecting the “Cloud Layer“ option in Visual Environment component
    ([UUM-75220](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-selecting-the-cloud-layer-option-in-visual-environment-component))

- DirectX12: [DX12] Player crash on UnityMain when building HDRP Sample on Windows
    ([UUM-75100](https://issuetracker.unity3d.com/issues/dx12-player-crash-on-unitymain-when-building-hdrp-sample-on-windows))

- DOTS: Job allocator contention causes slow job execution
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- Editor Platform: The "Hold On" dialog box persists when entering the Play Mode
    ([UUM-74916](https://issuetracker.unity3d.com/issues/the-hold-on-dialog-box-persists-when-entering-the-play-mode))

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

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- Vulkan:  Editor crash when changing Vulkan Number of Swapchain Buffers
    ([UUM-60016](https://issuetracker.unity3d.com/issues/vulkan-editor-crash-when-changing-vulkan-number-of-swapchain-buffers))



# 6000.0.11f1 Release Notes

## Improvements

- Animation: Improved Animation Mode performance when using custom properties.
    ([UUM-73525](https://issuetracker.unity3d.com/issues/the-editor-freezes-when-changes-are-made-in-the-timeline-window-and-a-large-number-of-animation-curve-bindings-and-gameobjects-are-loaded))

- Documentation: Added information about Player Build cache to PostProcessScene documentation.
    ([UUM-69256](https://issuetracker.unity3d.com/issues/the-postprocesssceneattribute-is-not-called-when-the-project-is-built-more-than-once))

- QNX: Video playback enabled



## API Changes

- Editor: Added: Adds RequestAsyncReadbackIntoNativeArray API to the Unsafe Pass.
    (UUM-73907)

- Physics 2D: Changed: Rigidbody2D.angularDrag is now Rigidbody2D.angularDamping.

- Physics 2D: Changed: Rigidbody2D.drag is now Rigidbody2D.linearDamping.

- Physics 2D: Changed: Rigidbody2D.velocity is now Rigidbody2D.linearVelocity.

- Physics 2D: Changed: Rigidbody2D.velocityX is now Rigidbody2D.linearVelocityX.

- Physics 2D: Changed: Rigidbody2D.velocityY is now Rigidbody2D.linearVelocityY.

- Physics 2D: Deprecated: Rigidbody2D.isKinematic is deprecated.  Use Rigidbody2D.bodyType instead.



## Changes

- SRP Core: Adding What's New in Unity 6 to SRP Core Package



## Fixes

- 2D: Fix issue where R 16 bit textures have banding effect when packed into a Sprite Atlas
    ([UUM-73396](https://issuetracker.unity3d.com/issues/r-16-bit-textures-have-banding-effect-when-packed-into-a-sprite-atlas))

- AI: Fixed an issue where NavMeshData belonging to a scene would remain loaded after the scene had been offloaded. This issue only occurred when the "Do not reload scene"-option has been checked in the editor settings.
    ([UUM-29346](https://issuetracker.unity3d.com/issues/navmesh-from-previous-scene-is-visible-after-going-into-play-mode-when-reload-scene-is-toggled-off))

- Android: AndroidX use is always true. Fixed problem with Gradle AAB build fail when Split App Binary is on, but there are no asset packs in the generated Gradle project.
    (UUM-73808)

- Android: Fixed player crash when changing cursor multiple times.
    ([UUM-74941](https://issuetracker.unity3d.com/issues/android-the-player-crashes-when-changing-cursor-multiple-times-on-android))

- Android: Resolved an issue where the OK button was absent in the Mobile Input Field of the soft keyboard.
    ([UUM-74675](https://issuetracker.unity3d.com/issues/android-soft-keyboard-is-missing-the-ok-button-on-android))

- Asset Bundles: Improved performance of AssetBundle.UnloadAsync. In certain large bundles with many scenes, the async unloading could take an excessively long time.

- Audio: Fixed an issue that would cause the pan control on audio sources to not work properly in some cases.
    ([UUM-65071](https://issuetracker.unity3d.com/issues/audiosource-stereo-pan-property-doesnt-fully-mute-the-right-or-left-channel-when-using-a-videoplayer-attached-to-an-audiosource-and-setting-the-option-to-1-or-1))

- Audio: Fixed empty playback when instantiating an AudioSource game object set to play on awake with AudioRandomContainer resource.
    ([UUM-74723](https://issuetracker.unity3d.com/issues/play-on-awake-does-not-work-with-an-audio-random-container-when-instantiating-a-game-object))

- Audio: Make fmodprofiling command line argument a diagnostic switch and update docs to show how to profile audio mixer effects
    ([UUM-41887](https://issuetracker.unity3d.com/issues/cpu-usage-display-is-not-toggled-when-toggling-it-in-audiomixergroupcontroller))

- Core: Fixed errors when duplicating scene.
    (UUM-74732)

- Documentation: Fixed a typo in the Create your own overlay page of the documentation.

- DX12: Fixed incorrect values for GetNextFrameFenceValue\(\) in render plugins
    (UUM-72389)

- Editor: Enabled hiding layers above current RP limit except when they are selected.
    (UUM-69315)

- Editor: Enabled Search Window available providers to display consistently across the Editor.
    ([UUM-72552](https://issuetracker.unity3d.com/issues/search-windows-opened-from-the-project-browser-and-windows-menu-act-differently))

- Editor: Filter out dynamic branch keywords when computing shader variants.
    ([UUM-48599](https://issuetracker.unity3d.com/issues/dynamic-branching-generates-shader-variants-when-building-the-project))

- Editor: Fix Exception Thrown When Minor Unity Version is Zero
    ([UUM-73851](https://issuetracker.unity3d.com/issues/invalid-unity-version-6000-dot-0-is-thrown-when-the-major-version-is-set-to-6000-and-minor-to-0))

- Editor: Fixed 100% editor freeze that occurs when clearing tracked shader variants.
    (UUM-74754)

- Editor: Fixed a bug where UI Canvas using Screen Space render mode would use an incorrect game view size and behave erratically.
    ([UUM-73707](https://issuetracker.unity3d.com/issues/erratic-behavior-while-editing-ui-in-prefab-when-canvas-render-mode-is-set-to-screen-space-camera-option))

- Editor: Fixed an error regarding invalid serialized properties when removing and adding multiple items to a UnityEvent.
    ([UUM-72670](https://issuetracker.unity3d.com/issues/adding-and-removing-items-from-serializefield-unityevent-throws-a-bunch-of-errors))

- Editor: Fixed an issue where an empty menu item was executed from within the AddComponent window.
    ([UUM-64144](https://issuetracker.unity3d.com/issues/executemenuitem-failed-because-there-is-no-menu-named-error-is-thrown-when-clicking-just-below-create-and-add-in-the-add-component-window))

- Editor: Fixed crash when hot-loading renderdoc in editor and GPU Resident Drawer running.
    ([UUM-73405](https://issuetracker.unity3d.com/issues/crash-when-loading-renderdoc-in-a-specific-scene))

- Editor: Fixed incorrect safeArea reported values and an error at the bottom of the screen for iOS versions 15 and below.
    ([UUM-51667](https://issuetracker.unity3d.com/issues/ios-the-safe-area-value-changes-when-reopening-the-app-in-landscape-orientation))

- Editor: Fixed issues with menu item Id values going out of sync on windows.
    ([UUM-73047](https://issuetracker.unity3d.com/issues/custom-and-built-in-menu-items-stop-working-when-a-project-has-lots-of-menu-items))

- Editor: Fixed log spamming and small chance of freezing due to missing sleep implemenation.
    (UUM-72409)

- Editor: Fixed low resolution artefacts when atmospheric scattering is on.
    (UUM-75115)

- Editor: Fixed saving a new scene with cloned dependencies to no longer overwrite the existing folder.
    ([UUM-66799](https://issuetracker.unity3d.com/issues/existing-folder-contents-are-overwritten-with-the-globalvolumeprofile-asset-when-saving-a-new-standard-urp-scene-in-unity))

- Editor: Fixed wrong exception messages in RenderGraph files.
    (UUM-74144)

- Editor: GameObjects can be selected in the Scene View when GPU Resident Drawer is enabled.
    (UUM-73317)

- Editor: Moved Realtime CPU Usage property above VSync Count.
    (UUM-73719)

- Editor: Reduced severity of AutoLocale validation message on Linux.
    ([UUM-74127](https://issuetracker.unity3d.com/issues/linux-autolocale-current-locale-expects-c-but-got-error-is-thrown-when-starting-a-project))

- Editor: When closing a modal dialog, the previous window's tabs are now properly restored.
    (UUM-74407)

- GI: Apply matching presets in Preset Manager when generating lightmaps and reflection probes.
    (UUM-70818)

- GI: Fixed noise when using Sky Occlusion with APV.
    ([UUM-71590](https://issuetracker.unity3d.com/issues/uneven-lighting-is-seen-on-the-gameobjects-when-sky-occlusion-is-enabled))

- Graphics: Different reflections on GameObject in Player compared to the Game View when DisplayP3 Color Gamut For Mac is selected on Silicon macOS
    ([UUM-46003](https://issuetracker.unity3d.com/issues/different-reflections-on-gameobject-in-player-compared-to-the-game-view-when-displayp3-color-gamut-for-mac-is-selected-on-silicon-macos))

- Graphics: Fixed culling split exclusion mask not working for Unity terrain.
    (UUM-74139)

- Graphics: Fixed Linear01DepthFromNear shader utility function on APIs with reversed Z buffer.
    ([UUM-19101](https://issuetracker.unity3d.com/issues/linear01depth-doesnt-return-different-values-depending-on-unity-reversed-z-when-graphics-api-is-not-openglcore))

- HDRP: Fix clouds interaction with thin geometry
    ([UUM-74923](https://issuetracker.unity3d.com/issues/visible-light-glares-appear-on-gameobjects-when-a-volumetric-clouds-effect-is-added-to-the-sky-and-fog-volume))

- HDRP: Fix clouds rendering on top of geometry
    (UUM-74934)

- HDRP: Fixed a disc area light calculation used for light unit conversion, which was previously incorrect by a factor of Pi.
    (UUM-74727)

- HDRP: Fixed light culling for raytracing.
    ([UUM-70779](https://issuetracker.unity3d.com/issues/errors-no-more-space-in-reflection-probe-atlas-logged-when-enabling-realtime-raytracing-in-the-hdrp-sample-template))

- HDRP: Fixed time of day script in environement sample.

- iOS: Added missing header files for plugins to Xcode project.
    (UUM-74318)

- iOS: Updated capability list
    (UUM-65394)

- License: Https://github.cds.internal.unity3d.com/unity/licensing.entitlement/releases/tag/v1.16.0-alpha.1.

- Package: Fixed Cinemachine bugs.

- Package Manager: Fixed the issue where My Assets page search result does not match that from the Asset Store website.
    (UUM-74477)

- Package Manager: Fixed the issues where Null Exception will be thrown sometimes in My Assets page.
    (UUM-72068)

- Particles: Fix potential unbounded memory and excessive work when using Ring Buffer mode
    ([UUM-72277](https://issuetracker.unity3d.com/issues/particle-system-allocates-large-amounts-of-memory-when-it-is-very-far-away-from-the-origin-of-the-scene))

- Particles: Updated ParticleSystem.Start\(\) documentation to reflect correct behavior.
    ([UUM-72281](https://issuetracker.unity3d.com/issues/the-particle-system-prewarm-flag-is-ignored-when-calling-the-start-function-after-the-stop-function))

- Scripting: Fixed an exception when calling destroy cancellation token after destroying the game object
    ([UUM-71988](https://issuetracker.unity3d.com/issues/requested-destroycancellationtoken-reports-as-not-requested-when-not-called-before-destroyed))

- Search: Enabled SearchContext attribute to work with arrays and lists.
    ([UUM-65462](https://issuetracker.unity3d.com/issues/searchcontext-attribute-does-not-work-when-used-with-arrays))

- Search: Ensured rebinding properties when docking or undocking the SearchWindow if the Detail view is open.
    (UUM-73162)

- Search: Fixed Search behaviour so that executing a temp query \(e.g. narrow area query\) doesn't set it as the activeQuery.
    ([UUM-72858](https://issuetracker.unity3d.com/issues/user-is-able-to-save-a-search-without-a-previous-search-selected-when-in-search-pills-are-introduced))

- Shaders: Fixed "\#pragma argument" being ignored in certain cases.
    (UUM-74358)

- uGUI: UGUI elements can be correctly selected in Scene view.
    ([UUM-74758](https://issuetracker.unity3d.com/issues/incorrect-element-gets-selected-when-trying-to-select-ugui-elements-in-the-scene-view))

- UI Toolkit: Fixed a stack overflow and provided users with proper logs explaining the situation when it occurs.
    ([UUM-69438](https://issuetracker.unity3d.com/issues/editor-crashes-freezes-or-throws-a-stackoverflowexception-error-when-selecting-an-element-within-the-graphwindow))

- UI Toolkit: Fixed an issue where a binding that is triggered in WhenSourceChanged mode would be continuously updated when the resolved data source is null.
    (UUM-74720)

- UI Toolkit: Fixed an issue where a data source was being unregistered twice when set on a children during an AttachToPanelEvent callback.
    ([UUM-75077](https://issuetracker.unity3d.com/issues/window-with-a-multi-column-list-view-crashes-after-it-is-moved-when-its-binding-source-selection-mode-is-set-to-auto-assign))

- UI Toolkit: Fixed an issue where the source generator of the the Unity.Properties module was targeting net6 instead of netstandard2.0, causing issues in VisualStudio.
    (UUM-74852)

- UI Toolkit: Fixed artifacts when rendering world-space UI Toolkit with WebGL.
    ([UUM-73117](https://issuetracker.unity3d.com/issues/world-space-ui-renders-with-artifacts-on-webgl))

- UI Toolkit: The TwoPaneSplitView's CollapseChild method can now be called during initialization.
    ([UUM-66400](https://issuetracker.unity3d.com/issues/twopanesplitview-collapsechild-doesnt-work-when-the-pane-is-first-drawn))

- UI Toolkit: The TwoPaneSplitView's drag line no longer hides its panes.
    ([UUM-53998](https://issuetracker.unity3d.com/issues/element-is-covered-by-the-dragline-when-using-twopanesplitview-and-adding-a-dragline-in-the-ui-toolkit))

- UI Toolkit: The TwoPaneSplitView's drag line no longer jumps when constrained by the minimum sizes of the panes.
    ([UUM-53665](https://issuetracker.unity3d.com/issues/uitoolkit-twopanesplitview-splitter-jumps-position-when-it-should-not-be-allowed-to-move))

- Universal RP: Fixed BlitAndSwapColorPass sample.
    ([UUM-74427](https://issuetracker.unity3d.com/issues/urp-shaderdata-namespace-error-is-thrown-when-building-a-project-with-urp-rendergraph-samples))

- Universal RP: Update template \(Create &gt; Rendering &gt; URP Post-Processing Effect \(Renderer Feature with Volume\)
    (UUM-72249)

- URP: Fixed an issue where reflection probes would render incorrectly on some platforms.
    (UUM-54060)

- VFX Graph: Fixed a crash that occurred when visualizing a VFX preview with raytracing enabled.
    (UUM-75069)

- VFX Graph: Fixed random texture rendered with instancing when using exposed texture set to None.
    ([UUM-74364](https://issuetracker.unity3d.com/issues/vfxg-setting-an-exposed-texture-to-none-assigns-a-random-texture))

- Web: Fixed an issue that Application.persistentDataPath would not automatically persist, by adding a new JS config option "autoSyncPersistentDataPath: true" to enable automatic synchronization of Application.persistentDataPath over to IndexedDB.
    ([UUM-60385](https://issuetracker.unity3d.com/issues/webgl-streamwriter-not-triggering-syncfs-when-writing-a-file-to-slash-idbfs))

- Web: Fixed compiler error when emscripten option "-sERROR_ON_UNDEFINED_SYMBOLS=0" is used.
    ([UUM-74261](https://issuetracker.unity3d.com/issues/webgl-build-is-missing-malloc-and-free-functions-when-passing-serror-on-undefined-symbols-equals-0-to-emscriptenargs))




## Package changes in 6000.0.11f1

## Packages updated

- com.unity.addressables: [2.1.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.1//changelog/CHANGELOG.html) to [2.2.2](https://docs.unity3d.com/Packages/com.unity.addressables@2.2//changelog/CHANGELOG.html)

- com.unity.cinemachine: [2.10.0](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) to [2.10.1](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [2.1.3](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.1//changelog/CHANGELOG.html) to [2.1.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.1//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.2.3](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html) to [1.2.6](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html)

- com.unity.addressables.android: [1.0.2](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html) to [1.0.3](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)