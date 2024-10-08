# Unity 6000.0.13f1
Published at Wed, 31 Jul 2024 18:30:12 GMT  
https://unity.com/releases/editor/whats-new/6000.0.13

# Known Issues in 6000.0.13f1

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- Kernel: Crash on TypeTreeQueries::IsStreamedBinaryCompatible when waiting for Unity’s code in UnityEditor.CoreModule.dll to finish executing
    ([UUM-77033](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-isstreamedbinarycompatible-when-waiting-for-unitys-code-in-unityeditor-dot-coremodule-dot-dll-to-finish-executing))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Lighting: Block compression leads to lightbaking artifacts in HDRP
    ([UUM-74735](https://issuetracker.unity3d.com/issues/lightmap-has-artifacts-when-generating-lighting))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- SRP Architecture & API: URP internal shader errors when the iOS is selected as a Build Target on the Windows Editor
    ([UUM-75654](https://issuetracker.unity3d.com/issues/urp-internal-shader-errors-when-the-ios-is-selected-as-a-build-target-on-the-windows-editor))

- SRP Templates: A bunch of Shader Warnings are thrown after switching platform to Linux/Linux Server when using Universal 3D Template
    ([UUM-76186](https://issuetracker.unity3d.com/issues/a-bunch-of-shader-warnings-are-thrown-after-switching-platform-to-linux-when-using-universal-3d-template))

- SRP XR: Error is thrown when Shader Graph Material is changed to "Decal"
    ([UUM-76172](https://issuetracker.unity3d.com/issues/error-is-thrown-when-shader-graph-material-is-changed-to-decal))

- UI Toolkit Controls: MultiColumnListView causes a memory leak when repeatedly shown and hidden
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- Vulkan:  Editor crash when changing Vulkan Number of Swapchain Buffers
    ([UUM-60016](https://issuetracker.unity3d.com/issues/vulkan-editor-crash-when-changing-vulkan-number-of-swapchain-buffers))



# 6000.0.13f1 Release Notes

## Improvements

- HDRP: Improved the batching of the Lit shaders in HDRP.
    (UUM-70368)

- Package Manager: Improved code coverage for BasePage, SimplePage and MyAssetpage classes.



## API Changes

- Editor: Added: Added ShaderUtil.CreateRayTracingShaderAsset\(\) to the Editor API



## Changes

- Android: Updated default androidMaxAspectRatio from 2.1 to 2.4.

- Burst: Improved error message for pointer-like types in non-`readonly` `static` fields.

- Burst: Improved performance of Burst-compiled code in the Windows x64 Editor by only emitting context-saving code when the code being compiled contains a `throw`.

- URP: Sprite Default Material - Moved to Graphics Settings, Sprite Settings from Renderer2DData.
    ([UUM-74931](https://issuetracker.unity3d.com/issues/nullreferenceexception-when-changing-the-default-material-type-to-custom))



## Fixes

- 2D: Fixed a crash that would occur when a user does an infinite recursion loop using a Tile's StartUp call by limiting the recursion.
    ([UUM-74939](https://issuetracker.unity3d.com/issues/crash-on-unsafeutility-custom-memset-when-simulating-a-random-tick-event-for-a-tile-at-a-specified-position))

- 2D: Fixed a null exception that would occur when a user tries to copy and paste a Sprite Outline to all Sprites when no SpriteRect in the Sprite Editor is selected.
    ([UUM-75806](https://issuetracker.unity3d.com/issues/nullreferenceexception-object-reference-not-set-to-an-instance-of-an-object-is-thrown-when-clicking-on-the-past-all-button-after-copying-in-the-custom-physics-shape-and-custom-outline-modules))

- 2D: Fixed an issue where generate outline turned sprites a solid black.
    ([UUM-75316](https://issuetracker.unity3d.com/issues/2d-generate-outline-will-turn-sprites-a-solid-black))

- 2D: Fixed an issue where SpriteRenderer sprite visual would appear unchanged when the sprite changed.
    ([UUM-73222](https://issuetracker.unity3d.com/issues/spriterenderer-sprite-visual-appears-unchanged-when-changing-it-during-the-runtime-in-2d-urp-projects))

- 2D: Fixed crash associated with VertexUtility::CopyChannel.
    ([UUM-72866](https://issuetracker.unity3d.com/issues/crash-on-vertexutility-copychannel-when-selecting-or-using-a-specific-sprite))

- 2D: Fixed errors that were thrown when errors are thrown when packing the Sprite Atlas due to TilingNotScheduled.
    ([UUM-75224](https://issuetracker.unity3d.com/issues/errors-are-thrown-when-packing-the-sprite-atlas-when-packables-contain-a-single-folder))

- 2D: Fixed Sprite Mask not correctly masking out normals pass.

- 2D: Set a minimum width for the Tile Palette window based on the size of the toolbar for Tile Palette Tools when undocked.
    ([UUM-75187](https://issuetracker.unity3d.com/issues/tile-palette-toolbar-controls-are-inaccessible-when-minimizing-the-window-to-its-minimum-width))

- 2D: Update Tile Palette Clipboard immediately when user activates a toggle on the Tile Palette Clipboard
    ([UUM-75498](https://issuetracker.unity3d.com/issues/tile-palettes-option-toggle-buttons-do-not-redraw-the-tile-palette))

- Android: Fixed an issue that prevented Gradle from buildingon API Level Targets bellow 30.
    (UUM-71048)

- Android: Fixed AndroidConfiguration so `keyboard/keyboardHidden` is properly set for GameActivity.
    (UUM-72217)

- Android: Re-set the minimum width for Android symbol format dropdowns to ensure it fits to width correctly.
    ([UUM-60933](https://issuetracker.unity3d.com/issues/longer-build-profile-window-fields-are-not-compatible-with-the-resized-window))

- Android: Removed a crash workaround on UnityPlayerGameActivity.java applyInsetListener, where we need to handle null instance for instance. GameActivity 3.0.4 now correctly handles this situation.

- Asset Pipeline: Fixed invalid iterator in AcceleratorClient.
    (UUM-69264)

- Audio: Added better error handling in AudioClipPlayable in the case of FMOD errors.
    ([UUM-65779](https://issuetracker.unity3d.com/issues/crash-on-audioclipplayable-handleplayevent-when-loading-and-instantiating-addressables-in-play-mode))

- Build System: Removed forked 7za binaries and Workspace.SevenZipPath.
    (UUM-37529)

- Burst: BurstAotSettings files are no longer written to disk unless default settings are changed.

- Burst: Fixed a compiler crash caused by faulty alias analysis.

- Burst: Fixed an issue that would cause `Mathf.Approximately` to return the wrong result.

- Burst: Fixed an issue where creating a project with a space in the path would cause burst to fail on Windows arm64.

- Burst: Fixed an issue where direct negation of enums was not correctly promoting the underlying type, causing wrong results.

- Burst: Fixed an issue with default interface methods which would result in compiler errors due to IL corruption.

- Editor: Fixed a bug where the Console log would only ping objects the first time they were clicked on.
    (UUM-76179)

- Editor: Fixed a crash that would occur on FlareManager::DeleteFrame when exiting Play mode.
    ([UUM-64098](https://issuetracker.unity3d.com/issues/crash-on-flaremanager-deleteflare-when-exiting-play-mode-after-selecting-the-scene-view))

- Editor: Fixed a potential crash or freeze that occured in the Editor with DX12.
    (UUM-74842)

- Editor: Fixed a shader compile error in the Production Ready Shaders sample in Shader Graph.
    (UUM-75983)

- Editor: Fixed an issue where properties for prefabs in Preview mode were treated as though they were being animated when they were not.
    ([UUM-61742](https://issuetracker.unity3d.com/issues/values-of-duplicated-prefab-instance-in-the-hierarchy-resets-to-the-original-prefab-when-preview-mode-is-enabled-in-animation-view))

- Editor: Fixed an issue where repaint injection on Linux was not allowed.
    ([UUM-70769](https://issuetracker.unity3d.com/issues/hdrp-samples-showcase-settings-not-found-in-window-project-settings))

- Editor: Fixed an issue where Texture2D could not have changes applied if the Inspector was in Debug mode.
    (UUM-51993)

- Editor: Fixed an issue where the scroll bar would not appear when a Volume Component was added.
    ([UUM-74506](https://issuetracker.unity3d.com/issues/horizontal-scrollbar-appears-in-the-inspector-window-when-the-volume-component-is-added))

- Editor: Fixed an issue with the computation of the width of tabs when an icon is above 16px.
    ([UUM-74176](https://issuetracker.unity3d.com/issues/tabs-open-with-elongated-width-for-its-label-section-when-opening-properties-for-an-asset-or-component))

- Editor: Fixed an open button from the Adaptive Probe Volume component.
    ([UUM-71680](https://issuetracker.unity3d.com/issues/warning-item-m-lightprobesystem-not-found-in-window-pc-rpasset-logged-when-navigating-to-rp-asset-from-probe-volume-component))

- Editor: Fixed build failure when setting custom iPhone splash screen storyboard.
    ([UUM-75293](https://issuetracker.unity3d.com/issues/ios-building-a-project-for-ios-with-launch-screen-set-to-custom-storyboard-fails-if-only-iphone-storyboard-was-setup))

- Editor: Fixed jam parameters for building player library from the Editor.
    (UUM-73389)

- Editor: Fixed multiple warnings from the same RP.
    ([UUM-74947](https://issuetracker.unity3d.com/issues/hdrp-multiple-warnings-for-the-supported-rendering-layers-in-the-rendering-layers-section))

- Editor: Fixed overlay popups so they display correctly under their collapsed overlay.
    (UUM-71222)

- Editor: Improved the caching performance of the Uxml Serialization store during domain reloads.
    (UUM-75268)

- Editor: Reduced the overhead of the macOS Editor task progress bar. This improves performance when many tasks are running in succession that require their own progress bar.
    ([UUM-52922](https://issuetracker.unity3d.com/issues/editor-hangs-and-throws-the-processes-pop-up-when-compiling-many-shaders-simultaneously))

- Editor: Removed alpha channel on gtk windows to prevent gnome from blending the window with other window's when our windows alpha is set to 0.
    ([UUM-67512](https://issuetracker.unity3d.com/issues/linux-scene-view-skybox-shows-artifacts-and-windows-behind-the-editor-when-a-material-with-transparency-is-used))

- Graphics: Fixed a crash that would occur when calling the C\# function `MaterialPropertyBlock.CopySHCoefficientArraysFrom` on a non-empty property block.
    ([UUM-74614](https://issuetracker.unity3d.com/issues/property-offset-falls-outside-of-range-for-type-in-getpropertydata-errors-are-thrown-when-using-materialpropertyblock-dot-copyshcoefficientarraysfrom))

- Graphics: Fixed an issue where Editor crashes on GfxDeviceVK::UpdateComputeResources when using compute shader with Vulkan Graphics API.
    ([UUM-74110](https://issuetracker.unity3d.com/issues/editor-crashes-on-gfxdevicevk-updatecomputeresources-when-using-compute-shader-with-vulkan-graphics-api))

- HDRP: Fixed broken link in fullscreen samples.
    ([UUM-71042](https://issuetracker.unity3d.com/issues/hdrp-fullscreen-samples-showcase-link-to-doc-is-broken))

- Kernel: Fixed an issue with connection to Profiler when using Autoconnect Profiler build option.
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- N/A \(internal\): Fixed instability in TexturePatched_MaterialsUpdateReferences.
    (UUM-73853)

- Package Manager: Fixed an error caused by deleting the Unity App Data folder by regenerating that folder when neccessary.
    ([UUM-72430](https://issuetracker.unity3d.com/issues/package-manager-does-not-create-a-default-cache-directory-for-asset-downloads))

- Particles: Fixed an issue where Particle System's "Texture Sheet Animation" module failed to load Sprite Atlas texture after exiting the Play mode.
    ([UUM-69612](https://issuetracker.unity3d.com/issues/particle-systems-texture-sheet-animation-module-fails-to-load-sprite-atlas-texture-after-exiting-the-play-mode))

- Particles: Limited the tile count in the Texture Sheet Animation module to 511 to avoid a potential crash scenario.
    ([UUM-75642](https://issuetracker.unity3d.com/issues/crash-on-transformparticlemesh-11-11-when-texture-sheet-animation-tiles-x-is-set-to-2-n-n-equals-9))

- Physics: Fixed an issue where negative scale would incorrectly affect the joint axis computation. Resulting in explosive behavior for the first few frames.
    ([UUM-75908](https://issuetracker.unity3d.com/issues/joint-connections-cause-rigidbodies-to-move-unpredictably-when-the-connected-rigidbodies-scales-are-of-opposite-sign))

- Search: Fixed error "AssetDatabase.SaveAssets are restricted during asset importing" when assigning Icons to a Saved Search if the project contained Scene Templates.
    ([UUM-72672](https://issuetracker.unity3d.com/issues/error-assetdatabase-dot-saveassets-are-restricted-during-asset-importing-when-assigning-icons-to-a-saved-search))

- Search: Fixed navigating between Saved Searches resulting in broken search results.
    ([UUM-75505](https://issuetracker.unity3d.com/issues/search-navigating-between-saved-searches-carries-over-all-results-and-can-result-in-a-nullreferenceexception))

- Search: Fixed NullReference exception when opening scenes with Window &gt; Search &gt; Scenes.
    ([UUM-73863](https://issuetracker.unity3d.com/issues/search-nullreferenceexception-on-selecting-search-scene-scenes))

- Search: Fixed QueryBuilder vectors showing uneditable values.
    ([UUM-74901](https://issuetracker.unity3d.com/issues/search-query-builder-uneditable-nan-in-transform-vectors))

- Search: Fixed Search's autocomplete window not closing when the text field loses focus.
    ([UUM-75254](https://issuetracker.unity3d.com/issues/recent-search-window-cant-be-closed))

- Search: Fixed shortcuts in the Search window not working depending on the focus area.
    ([UUM-75244](https://issuetracker.unity3d.com/issues/search-window-shortcuts-are-not-functioning-when-certain-areas-of-the-window-are-focused))

- SRP Core: \[GLES3\] Fixed an issue where Blitter.GetBlitMaterial\(TextureDimension.Tex2DArray\) returns null.
    (UUM-75623)

- uGUI: Fixed an issue where Anchor foldout in RectTransform doesn't get keyboard focus.
    ([UUM-71130](https://issuetracker.unity3d.com/issues/field-names-under-anchors-in-the-recttransform-component-dont-get-focused-when-tabbing-through-the-fields))

- UI Toolkit: Fixed an issue in the UI Builder where the parts of a selector were displayed without a space between them.
    (UUM-72728)

- UI Toolkit: Fixed an issue that would cause a null reference exception when adding an element to an array.
    ([UUM-54028](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-adding-an-element-to-an-array))

- UI Toolkit: Fixed an issue that would cause a null reference exception when using custom type property drawer on an array or list.
    ([UUM-74491](https://issuetracker.unity3d.com/issues/system-dot-nullreferenceexception-is-thrown-when-selecting-a-gameobject-with-custom-inspector))

- UI Toolkit: Fixed an issue where ListView's allowAdd and allowRemove properties would call an unnecessary rebuild.
    ([UUM-72630](https://issuetracker.unity3d.com/issues/the-font-and-border-color-indicating-the-selected-rendering-layer-is-displayed-incorrectly-when-more-than-two-new-layers-are-added))

- UI Toolkit: Fixed an issue where reorderable ListView handles with custom display style being overridden by inline styles.
    ([UUM-66690](https://issuetracker.unity3d.com/issues/reorderable-listview-items-handles-with-a-display-none-class-become-visible-when-reordering-the-list-and-adding-a-new-item))

- UI Toolkit: Fixed an issue with ToggleButtonGroup so it has more padding around buttons.
    (UUM-73306)

- UI Toolkit: Fixed InspectorElement so it supports editing multiple objects.
    ([UUM-74891](https://issuetracker.unity3d.com/issues/transform-dot-rotation-property-is-as-a-vector4-quaternion-instead-of-a-vector3-field-when-using-inspectorelement-dot-filldefaultinspector))

- UI Toolkit: Fixed ListView focus order so it follows: Foldout &gt; Size Field &gt; Contents &gt; Add Button &gt; Remove Button.
    (UUM-32041)

- UI Toolkit: Fixed performance issues related to saving a document in the builder.
    (UUM-75704)

- UI Toolkit: Fixed separators so they are not allowed to be the first item in a submenu in the dropdown menu.
    ([UUM-75495](https://issuetracker.unity3d.com/issues/unused-separation-line-is-present-in-scene-view-options-prefab-dropdown-menu))

- UI Toolkit: Fixed StackOverflowException in ListView when scrolling to an item.
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- UI Toolkit: Foldout can now be bound to a simple boolean.
    ([UUM-72868](https://issuetracker.unity3d.com/issues/ui-toolkit-foldout-cannot-be-bound-when-serializable-property-is-used))

- UI Toolkit: Made significant improvements to selection performance when dealing with a large number of indices in BaseVerticalCollectionView. This should be noticeable in the ListView, TreeView, MultiColumnTreeVIew and MultiColumnListView.
    ([UUM-74996](https://issuetracker.unity3d.com/issues/setselectionbyidwithoutnotify-and-setselectionwithoutnotify-takes-more-than-20-seconds-when-uielements-dot-treeview-contains-100000-items))

- UI Toolkit: Reduced mesh allocation when using background repeat.
    (UUM-73770)

- URP: Fixed an issue with the Inspector of Render2DData when selecting custom default material.
    ([UUM-74931](https://issuetracker.unity3d.com/issues/nullreferenceexception-when-changing-the-default-material-type-to-custom))

- Version Control: Fixed an issue where the Unity Editor would get stuck on *Creating workspace* when *Use Unity Version Control* was selected from the Hub.

- VFX Graph: Fixed a potential division by zero in RayBoxIntersection code.
    (UUM-73448)

- VFX Graph: Fixed an issue where copying or pasting in a different asset in a context with a block that used a custom attribute would lose the custom attribute type and fallback to float.
    ([UUM-75894](https://issuetracker.unity3d.com/issues/vfx-graph-copy-slash-paste-custom-attributes-between-graph-fall-back-to-float-type))

- VFX Graph: Fixed missing drag area to change a value for inline float, uint and int operators.
    ([UUM-75981](https://issuetracker.unity3d.com/issues/vfx-cannot-drag-value-with-inline-float-operator-and-a-few-others))

- VisionOS: Added support for using WebCamTexture to obtain the Persona feed on visionOS.

- Web: Fixed an issue where the key state of the 'v' key could sometimes remain active even after released when pasting from the clipboard.
    ([UUM-71733](https://issuetracker.unity3d.com/issues/ctrl-plus-c-and-ctrl-plus-v-keyboard-inputs-are-not-registered-in-player-when-the-build-platform-is-webgl))

- WebGL: \[WebGPU\] Fixed an issue that caused Unity WebGPU builds to fail on Chrome Canary.

- WebGL: \[WebGPU\] Fixed an issue with Graphics.CopyTexture.




## Package changes in 6000.0.13f1

## Packages updated

- com.unity.burst: [1.8.16](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.17](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.4.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.4//changelog/CHANGELOG.html) to [2.4.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.4//changelog/CHANGELOG.html)

- com.unity.polybrush: [1.1.6](https://docs.unity3d.com/Packages/com.unity.polybrush@1.1//changelog/CHANGELOG.html) to [1.1.8](https://docs.unity3d.com/Packages/com.unity.polybrush@1.1//changelog/CHANGELOG.html)

- com.unity.purchasing: [4.12.1](https://docs.unity3d.com/Packages/com.unity.purchasing@4.12//changelog/CHANGELOG.html) to [4.12.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.12//changelog/CHANGELOG.html)

- com.unity.sequences: [2.1.1](https://docs.unity3d.com/Packages/com.unity.sequences@2.1//changelog/CHANGELOG.html) to [2.1.2](https://docs.unity3d.com/Packages/com.unity.sequences@2.1//changelog/CHANGELOG.html)