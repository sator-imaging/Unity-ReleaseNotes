# Unity 2022.3.61f1 LTS
Published at Thu, 10 Apr 2025 08:38:43 GMT  
https://unity.com/releases/editor/whats-new/2022.3.61

# Known Issues in 2022.3.61f1

- DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when opening a project after changing the Graphics API to DirectX12
    ([UUM-77757](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-opening-a-project-after-changing-the-graphics-api-to-directx12))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DirectX12: The Player hangs when unloading a scene using the UnloadUnusedAssets() method
    ([UUM-79718](https://issuetracker.unity3d.com/issues/the-player-hangs-when-unloading-a-scene-using-the-unloadunusedassets-method))

- Vulkan:  Application crashes with Vulkan when restoring from background on Linux
    ([UUM-90287](https://issuetracker.unity3d.com/issues/vulkan-android-application-crashes-on-android-devices-with-vulkan-when-restoring-from-background))

- WebGL: Scene is not rendered and RenderPass errors in WebGL when MSAA is enabled on URP Asset and the Camera or Overlay Camera Stacking is used
    ([UUM-90459](https://issuetracker.unity3d.com/issues/scene-is-not-rendered-and-renderpass-errors-when-urp-msaa-is-enabled-in-the-webgl-player))



# 2022.3.61f1 Release Notes

## Improvements

- Build System: Improved logging for the "Read the full binlog without getting a BuildFinishedMessage" internal build error, so we can see if the build was cancelled from the editor process.

- Documentation: Added a fixed width to the body of the user manual so that the text doesn't overrun on large screens.

- Shadergraph: Removed duplicate LIGHTMAP_ON and DIRLIGHTMAP_COMBINED variants when generating shaders for builtin-deferred.



## Changes

- Editor: Changed canRunInBackground to false for Windows Gaming Input gamepads since they cannot be used while the application is in background.
    (ISXB-1391)

- Editor: Updated TerrainTools package to version 5.0.6.

- Package: Updated PolySpatial/visionOS packages to version 1.3.12.

- Package: Updated timeline package to 1.7.7 for 2022.3.

- XR: The Oculus XR Plugin package has been updated to 4.5.1.

- XR: Updated com.unity.xr.openxr package version to 1.14.2.



## Fixes

- 2D: Added layer mask in renderer 2d data for filtering options.
    (UUM-95754)

- 2D: Fixed case Sprite Atlas samples show white textures in playmode when using late binding.
    ([UUM-100501](https://issuetracker.unity3d.com/issues/2d-sprite-atlas-samples-show-white-textures-in-playmode-when-using-late-binding))

- 2D: Fixed missing fog parameters in sprite subtargets.
    ([UUM-85456](https://issuetracker.unity3d.com/issues/fog-density-value-is-not-returned-when-using-the-fog-node-in-a-sprite-shader-graph))

- 2D: Fixed normal map preview in Sprite Editor Window's Secondary Texture module.
    ([UUM-99022](https://issuetracker.unity3d.com/issues/normal-maps-are-rendered-differently-in-sprite-editor-when-compared-to-the-inspector-preview))

- 2D: Fixed post processing resolve for Renderer2D.
    ([UUM-99455](https://issuetracker.unity3d.com/issues/not-all-post-processing-overrides-are-visible-when-camera-stack-is-applied))

- 2D: Fixed runtime light2d not created with target sorting layers.
    ([UUM-11350](https://issuetracker.unity3d.com/issues/light2d-is-not-working-in-the-build-when-created-through-script))

- 2D: Fixed warning 'GetControlID at event ValidateCommand returns a controlID different from the one in the Layout event' is logged when undoing the deletion of an Edited Freeform 2D Light.
    ([UUM-90726](https://issuetracker.unity3d.com/issues/warning-getcontrolid-at-event-validatecommand-returns-a-controlid-different-from-the-one-in-the-layout-event-is-logged-when-undoing-the-deletion-of-an-edited-freeform-2d-light))

- Android: Fixed dialog input field not getting dismissed after back gesture.
    (UUM-99637)

- Android: Fixed incorrect BGR color channel swizzle when playing VP8 videos on Android while using Vulkan as Graphics API.
    ([UUM-90144](https://issuetracker.unity3d.com/issues/android-vulkan-the-color-channel-of-videos-changes-from-rgb-to-bgr-when-streaming-in-the-player))

- Android: Fixed Integer input field now allowing negative integers to be entered.
    ([UUM-85618](https://issuetracker.unity3d.com/issues/android-the-symbol-is-not-allowed-to-be-entered-when-entering-a-negative-number-in-an-inputfield-when-the-content-type-is-set-to-integer-number))

- Android: Fixed the problem with additional streaming assets \(added using BuildPlayerContext.AddAdditionalPathToStreamingAssets\) being compressed in APK/AAB.
    (UUM-96090)

- Asset Pipeline: Fixed problem with main thread potentially being blocked, while doing async asset loads.
    ([UUM-95528](https://issuetracker.unity3d.com/issues/loading-animations-are-hitching-or-stopping-when-using-scenemanager-dot-loadsceneasync-to-load-new-scenes))

- Audio: Fixed an issue that would cause audio playables to throw a warning in the console.
    (UUM-96563)

- Build Pipeline: Added a Scriptable Build Pipeline setting that optionally disables logging of asset warnings during build process.
    ([ADDR-3706](https://issuetracker.unity3d.com/issues/warning-logs-about-missing-scripts-are-thrown-when-building-asset-bundles-using-addressables-slash-sbp))

- Editor: Changed made to Static Emissives in Light Explorer do not add to Undo History.
    ([UUM-83357](https://issuetracker.unity3d.com/issues/changes-made-to-static-emissives-in-light-explorer-do-not-add-to-undo-history))

- Editor: Editor no longer crashes when changing template scene to instantiate if user has a preview thumbnail set.
    ([UUM-97241](https://issuetracker.unity3d.com/issues/unity-crashes-during-the-scene-template-selection-in-the-inspector-tab))

- Editor: Fixed a bug where the Occlusion Window active filter would be reset on domain reload.
    ([UUM-99535](https://issuetracker.unity3d.com/issues/scene-filter-buttons-reset-to-all-in-the-occlusion-window-when-entering-play-mode-but-the-scene-filters-themselves-do-not-reset))

- Editor: Fixed a performance issue with user-provided or package-provided gizmo icons. Optimized gizmo icon rendering to significantly improve their performance in large scenes.
    ([UUM-97855](https://issuetracker.unity3d.com/issues/script-icon-gizmos-cause-lag-slash-performance-issues-in-scene-view-even-when-the-scene-camera-is-not-pointed-at-gizmos))

- Editor: Fixed an error message when multiple objects with LODGroup components are selected.
    (UUM-97878)

- Editor: Fixed an issue where having multiple Scene views open would make the Scene views constantly repaint.
    ([UUM-77750](https://issuetracker.unity3d.com/issues/scene-view-always-refreshing-when-multiple-scene-views-are-open))

- Editor: Fixed an issue where the Device Simulator's scale would not persist when maximizing then minimizing another window.
    ([UUM-78562](https://issuetracker.unity3d.com/issues/the-simulator-tab-scale-is-reset-when-using-double-click-to-maximize-and-then-shrink-another-window))

- Editor: Fixed AssetDatabase.GetAssetBundleDependencies returned list doesn't include dependency when it's a Prefab Asset.
    ([UUM-83829](https://issuetracker.unity3d.com/issues/assetdatabase-dot-getassetbundledependencies-returned-list-doesnt-include-dependency-when-its-a-prefab-asset))

- Editor: Fixed freeze within cyclic compositions where internal depth limit was not being observed.
    ([UUM-49767](https://issuetracker.unity3d.com/issues/unity-freezes-when-opening-a-project))

- Editor: Fixed Gradient field picker not updating correctly during Undo/Redo.
    ([UUM-99032](https://issuetracker.unity3d.com/issues/undo-ctrl-plus-z-works-incorrectly-when-editing-markers-on-the-gradient-editor))

- Editor: Fixed GradientPicker removing all swatches when dragging them outside.
    ([UUM-100664](https://issuetracker.unity3d.com/issues/all-newly-created-color-markers-of-gradient-editor-get-removed-at-once-when-trying-to-remove-one-of-them))

- Editor: Fixed offscreen rendering flags to be added only when the "Offscreen Rendering \(Vulkan\)" OpenXR UI setting is present and enabled.
    ([OXRB-358](https://issuetracker.unity3d.com/issues/mobile-the-player-displays-a-black-screen-when-the-openxr-is-used-as-the-plug-in-provider))

- Editor: Fixed opening editor log when -logFile is a relative path.
    ([UUM-96399](https://issuetracker.unity3d.com/issues/clicking-open-editor-log-through-the-console-fails-to-open-redirected-logs-when-relative-log-files-exist-outside-of-the-project-root))

- Editor: Fixed SettingsService.NotifySettingsProviderChanged\(\) not calling OnDeactivate\(\) for existing providers.
    ([UUM-99153](https://issuetracker.unity3d.com/issues/settingsservice-dot-notifysettingsproviderchanged-doesnt-call-ondeactivate-for-existing-settingsproviders-when-new-serviceprovider-is-created))

- Editor: Fixed that a Scene is built with the additive Scene's contents when loading the additive Scene on Awake.
    (UUM-99623)

- Editor: Fixed the indentation of list properties in the inspector.
    ([UUM-99070](https://issuetracker.unity3d.com/issues/foldout-arrow-indent-is-misaligned-in-the-inspector-when-used-for-arrays-or-lists))

- Editor: Fixed the `EditorStyles.whiteBoldLabel` style so the text is white.
    ([UUM-84114](https://issuetracker.unity3d.com/issues/editorguilayout-dot-labelfield-displays-black-text-when-the-editorstyles-dot-whiteboldlabel-parameter-is-passed-in))

- Editor: Graphics: This PR fixes the shadow jittering issue with TAA in deferred pass on URP scenes.
    ([UUM-97957](https://issuetracker.unity3d.com/issues/shadow-is-jittering-when-taa-is-on-lens-shift-is-enabled-and-the-camera-is-at-least-800-units-away-from-the-origin))

- Editor: Improved Add Component window so long item names are truncated with ellipsis.
    ([UUM-91895](https://issuetracker.unity3d.com/issues/extended-component-titles-exceed-the-windows-display-boundaries))

- Editor: Late binding of SpriteAtlas objects now works when loading from content archives.
    ([UUM-101143](https://issuetracker.unity3d.com/issues/entities-android-ui-game-object-missing-sprite-when-using-content-management-and-sprite-atlas))

- Editor: Linux: Fixed crash when an exception is thrown in a docked tab when closing a window.
    (UUM-97461)

- Editor: Modified touch position calculation to match mouse position calculation on Windows \(Input.mousePosition\). This fixes consistency issues between mouse and touch when in certain multi-display and multi-window scenarios.
    ([UUM-99077](https://issuetracker.unity3d.com/issues/touch-input-is-not-registered-correctly-when-using-multiple-displays))

- Editor: Prefab Override comparison window now displays properly with many fields.
    ([UUM-96045](https://issuetracker.unity3d.com/issues/prefab-override-comparison-window-is-squished-and-non-scrollable-when-many-serialized-fields-are-used))

- Editor: Removed the scroller from the prefab override modal when the content does not overflow.
    (UUM-83279)

- Editor: Resolved issue where directories with very large numbers of items and deep directory structures could cause dragging assets into a project to become sluggish and potentially freeze the Editor.
    (UUM-98134)

- Editor: Switch to OnDidApplyAnimationProperties instead of Update for DecalProjectors.
    (UUM-100025)

- Editor: The slider will now accumulate clicks over time when the page size is very small and does not move after a single click.
    ([UUM-86425](https://issuetracker.unity3d.com/issues/moving-the-scrollbar-via-clicking-no-longer-works-after-the-first-click-when-page-size-is-too-small))

- Editor: This PR fixes a bug where position handles still react on hover even when they are not interactive due to being positioned behind an overlay, such as the orientation gizmo.
    ([UUM-97499](https://issuetracker.unity3d.com/issues/sw-unity-6-1-transform-gizmos-cannot-be-interacted-with-when-they-are-overlapping-with-the-orientation-gizmo))

- EmbeddedLinux: Fixed systeminfo::GetExecutableSizeMB reporting wrong values on Embedded and Desktop Linux.
    (UUM-66340)

- Graphics: Compression of NPOT textures with mipmaps is not supported by the GPU. Texture2D.Compress function has been updated to detect that and not compress the texture, issuing an error message, so that it is consistent with the texture import pipeline.
    ([UUM-35314](https://issuetracker.unity3d.com/issues/material-etc2-rgba-block-stride-mipmaps-are-rendered-incorrectly-in-the-preview-window-when-the-android-platform-is-selected-and-using-compressed-npot-texture-mipmaps))

- Graphics: Fixed a crash that can happen when using procedural geometries \(intersection shaders\) in ray tracing effects in the Editor.
    ([UUM-100898](https://issuetracker.unity3d.com/issues/crash-on-stackwalker-getcurrentcallstack-when-opening-a-project))

- Graphics: Fixed LODGroupEditor throwing exceptions when underlying LODGroup is modified through code.
    (UUM-90137)

- Graphics: Fixed separate depth/stencil clears when using Vulkan.
    ([UUM-100002](https://issuetracker.unity3d.com/issues/stencil-buffer-is-incorrectly-cleared-across-vulkan-render-passes-during-depth-only-clear-operations-when-using-commandbuffer-api))

- Graphics: Fixed separate depth/stencil clears when using Vulkan.
    ([UUM-100002](https://issuetracker.unity3d.com/issues/stencil-buffer-is-incorrectly-cleared-across-vulkan-render-passes-during-depth-only-clear-operations-when-using-commandbuffer-api))

- HDRP: Fixed water system memory leak on domain reload.
    ([UUM-91837](https://issuetracker.unity3d.com/issues/memory-leak-when-a-domain-is-reloaded-on-a-scene-that-uses-hdrps-water-simulation-resources))

- HDRP: This PR fixes a shader compilation error of HDRP Lit Shader if UV mapping for Emissive Map is set to "Same as Base".
    ([UUM-100070](https://issuetracker.unity3d.com/issues/hdrp-lit-shader-errors-are-thrown-and-artifacts-are-generated-when-using-emissive-map-and-same-as-base-uv-mapping-setting))

- IL2CPP: Fixed issue where some nested structs configurations could cause long build times.
    ([UUM-98369](https://issuetracker.unity3d.com/issues/long-il2cpp-build-time-when-project-has-a-ufbx-library-wrapper))

- Installer: Fixed installer from always trying to install VC++ 2010 Redistributables.
    (UUM-99960)

- iOS: Fixed soft keyboard Done/Cancel buttons truncating \(to "..."\) in languages like Korean due to decimal font width.
    ([UUM-97527](https://issuetracker.unity3d.com/issues/ios-hwagin-done-and-cwiso-cancel-text-is-displayed-as-dot-dot-dot-in-the-on-screen-keyboard-when-the-system-preferred-language-is-set-to-korean))

- Kernel: Reduced profiler overhead when executing For Each jobs.
    (UUM-92906)

- Mobile: Fixed user certificates included in the app by default.
    ([UUM-97194](https://issuetracker.unity3d.com/issues/android-ios-unitywebrequest-requests-with-unitywebrequest-are-open-for-ssl-proxying))

- Mono: Fixed performance regression where hardware intrinsics were not being applied fully.
    (UUM-85288)

- Package Manager: Fixed the issue when a upm package on Asset Store conflicts with a package on scoped registry, both become unaccessible.
    (UUM-86790)

- Particles: Clarify unexpected behavior on ParticleSystem.Play\(\) API documentation.
    ([UUM-99113](https://issuetracker.unity3d.com/issues/particle-system-doesnt-always-play-when-particlesystem-dot-play-is-called))

- Profiler: Fixed potential Editor crash on invalid_parameter_internal when starting Standalone Profiler.
    ([UUM-98081](https://issuetracker.unity3d.com/issues/crash-on-invalid-parameter-internal-when-starting-standalone-profiler))

- Shadergraph: Fixed an issue where an HDRP fullscreen shader graph imported into a URP project would fail to import under some circumstances.
    ([UUM-55703](https://issuetracker.unity3d.com/issues/fullscreen-shader-graph-assets-are-unusable-when-imported-into-a-urp-project-and-have-both-urp-and-hdrp-as-active-targets-as-well-as-material-set-to-fullscreen))

- Terrain: Fixed the issue in which Terrain splatmaps do not ignore mipmap limit when it should be.
    ([UUM-97145](https://issuetracker.unity3d.com/issues/terrain-masks-do-not-ignore-the-mipmap-limit))

- UI Elements: Corrected the indentation for decorator drawers.
    ([UUM-89976](https://issuetracker.unity3d.com/issues/decoratordrawer-indentation-is-incorrect-when-it-is-called-with-editorgui))

- UI Elements: Fixed the TreeView's item clipping when using the Fixed Height Virtualization together with the Scale with Screen Size.
    ([UUM-84105](https://issuetracker.unity3d.com/issues/the-ui-toolkit-treeview-items-get-clipped-when-resizing-the-game-view-window-when-scale-with-screen-size-is-set-as-the-scale-mode-in-the-panel-settings))

- UI Elements: Prevent rename and create template option in the context menu when multiple elements are selected within UIBuilder hierarchy.
    ([UUM-76831](https://issuetracker.unity3d.com/issues/the-option-to-rename-or-create-template-is-exposed-to-users-when-multiple-elements-are-selected-in-the-hierarchy))

- UI Elements: Updated the pointer counter logic for collection views.
    ([UUM-82931](https://issuetracker.unity3d.com/issues/android-itemschosen-event-is-not-triggered-when-double-clicking-an-item-in-treeview-on-specific-devices))

- UI Toolkit: Fixed an issue where non-default dimension units were omitted in the USS output by the UI Builder when the value was 0.
    ([UUM-99023](https://issuetracker.unity3d.com/issues/uss-units-are-not-serialized-when-values-are-edited-manually-in-the-file))

- UI Toolkit: Fixed an issue with the final item of a ListView hiding at high display scales when another item was moved.
    ([UUM-81516](https://issuetracker.unity3d.com/issues/element-disappears-from-a-list-after-its-reordered-when-a-high-display-resolution-and-a-250-percent-display-scale-is-used))

- UI Toolkit: Fixed dropdown menu positions appearing in the wrong place.
    ([UUM-74016](https://issuetracker.unity3d.com/issues/the-visual-effects-graphs-dropdown-menus-open-outside-the-window-when-another-window-is-selected-first))

- UI Toolkit: Fixed expressions for serialized properties in numeric fields.
    ([UUM-82983](https://issuetracker.unity3d.com/issues/numeric-field-expressions-do-not-provide-correct-results-when-used-in-a-public-float-field-in-the-inspector))

- UI Toolkit: Fixed NullReferenceException.
    (UUM-100051)

- UI Toolkit: Fixed UI Builders incorrectly informs about a circular dependency when the reference document is removed.
    ([UUM-85011](https://issuetracker.unity3d.com/issues/ui-builders-incorrectly-informs-about-a-circular-dependency-when-the-reference-in-the-second-ui-document-is-removed))

- UI Toolkit: Fixed UI Debugger picking for editor panel.
    ([UUM-95486](https://issuetracker.unity3d.com/issues/sw-unity-6-1-ui-toolkit-debuggers-pick-element-functionality-does-not-work-when-hovering-on-any-editor-panel-except-the-game-view))

- UI Toolkit: TwoPaneSplitView can now collapse its child immediately after initialization.
    ([UUM-66400](https://issuetracker.unity3d.com/issues/twopanesplitview-collapsechild-doesnt-work-when-the-pane-is-first-drawn))

- UI Toolkit: UI Builder: the last Canvas Theme applied to a UXML Document by the user is now remembered.
    (UUM-17567)

- URP: Fixed DecalProjector's animation-clip support.
    ([UUM-96218](https://issuetracker.unity3d.com/issues/urp-decal-projector-fade-factor-doesnt-get-updated-when-changing-it-through-animation))

- Version Control: When modifying the mergespecfile.tx to use Beyond Compare, it continues to fall back to FileMerge.
    ([UUM-91595](https://issuetracker.unity3d.com/issues/unityyamlmerge-does-not-open-fallback-merge-tool-when-encountering-merge-conflicts))

- VFX Graph: Fixed BakedGI node showing black in VFX graph outputs using Shader Graph.
    ([UUM-99499](https://issuetracker.unity3d.com/issues/vfx-graph-particles-render-black-when-using-baked-gi-in-urp-unlit-shader-graph))

- VFX Graph: Fixed crash on mobile player builds when loading a Scene referencing a VisualEffect component but not a VfxRenderer component with the "Strip Engine Code" feature enabled. The VfxRenderer component engine code is no longer incorrectly stripped.
    ([UUM-99927](https://issuetracker.unity3d.com/issues/android-ios-il2cpp-the-application-crashes-when-loading-a-subscene-with-a-baker-that-adds-a-prefab-using-a-visualeffect-component))

- VFX Graph: Fixed crash when reimporting textures used by a VFX that is active and culled.
    ([UUM-97920](https://issuetracker.unity3d.com/issues/crash-on-vfxvaluewrapper-gettexture-when-reimporting-texture-in-use-by-out-of-bounds-vfx))

- VFX Graph: Unexpected visible particle if set alive is force to true in SG Opaque Output.
    (UUM-96266)

- Video: Fixed an edge case in error handling when attempting to open a video file on Android.
    ([UUM-88992](https://issuetracker.unity3d.com/issues/android-neither-of-the-callbacks-are-called-when-several-videos-with-videoplayer-are-spawned-on-the-target-on-the-google-pixel-devices))

- Video: \[Windows\] Allow an arbitrary amount of webcam \(virtual and/or physical\) devices to be used.
    ([UUM-96061](https://issuetracker.unity3d.com/issues/crash-on-monostringnewutf16-when-calling-webcamtexture-dot-devices-with-more-than-20-active-webcams))

- Web: Fixed bug where calling RequestUserAuthorization\(UserAuthorization.Microphone\) in the Web player would prompt the user for webcam permissions instead of microphone permissions. The microphone API is not yet supported in Web, so a warning message has been added to inform developers of this limitation.
    ([UUM-75678](https://issuetracker.unity3d.com/issues/webcam-permissions-are-asked-instead-of-microphone-permissions-when-using-requestuserauthorization-userauthorization-dot-microphone-in-the-webgl-player))

- Web: Fixed bug where RangeError: Array buffer allocation failed was thrown when running URP sample on Chrome with compression.
    ([UUM-98061](https://issuetracker.unity3d.com/issues/universal-3d-sample-template-build-throws-rangeerror-array-buffer-allocation-failed-when-launched-on-chrome))

- Web: Fixed issue preventing AudioClip from playing in Timeline in WebGL builds.
    ([UUM-77185](https://issuetracker.unity3d.com/issues/only-the-first-audio-clip-gets-played-in-webgl-when-more-than-one-track-is-in-the-timeline))

- Windows: Fixed for Video Player when reading video files with long path prefix.
    (UUM-78606)

- Windows: Fixed monitor handle association with the display details, for all resolutions.
    ([UUM-78860](https://issuetracker.unity3d.com/issues/screen-api-breaks-when-setting-resolution-below-1280x720-in-an-exclusive-fullscreen-player-on-a-specific-monitor))




## Package changes in 2022.3.61f1

## Packages updated

- com.unity.2d.animation: [9.1.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@9.1//changelog/CHANGELOG.html) to [9.2.0](https://docs.unity3d.com/Packages/com.unity.2d.animation@9.2//changelog/CHANGELOG.html)

- com.unity.2d.common: [8.0.4](https://docs.unity3d.com/Packages/com.unity.2d.common@8.0//changelog/CHANGELOG.html) to [8.1.0](https://docs.unity3d.com/Packages/com.unity.2d.common@8.1//changelog/CHANGELOG.html)

- com.unity.2d.pixel-perfect: [5.0.3](https://docs.unity3d.com/Packages/com.unity.2d.pixel-perfect@5.0//changelog/CHANGELOG.html) to [5.1.0](https://docs.unity3d.com/Packages/com.unity.2d.pixel-perfect@5.1//changelog/CHANGELOG.html)

- com.unity.2d.psdimporter: [8.0.5](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.0//changelog/CHANGELOG.html) to [8.1.0](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@8.1//changelog/CHANGELOG.html)

- com.unity.2d.spriteshape: [9.0.5](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@9.0//changelog/CHANGELOG.html) to [9.1.0](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@9.1//changelog/CHANGELOG.html)

- com.unity.ide.rider: [3.0.34](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.35](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.inputsystem: [1.11.2](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.11//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.14//changelog/CHANGELOG.html)

- com.unity.probuilder: [5.2.3](https://docs.unity3d.com/Packages/com.unity.probuilder@5.2//changelog/CHANGELOG.html) to [5.2.4](https://docs.unity3d.com/Packages/com.unity.probuilder@5.2//changelog/CHANGELOG.html)

- com.unity.services.analytics: [6.0.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html) to [6.0.3](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.0//changelog/CHANGELOG.html)

- com.unity.splines: [2.7.2](https://docs.unity3d.com/Packages/com.unity.splines@2.7//changelog/CHANGELOG.html) to [2.8.0](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)

- com.unity.timeline: [1.7.6](https://docs.unity3d.com/Packages/com.unity.timeline@1.7//changelog/CHANGELOG.html) to [1.7.7](https://docs.unity3d.com/Packages/com.unity.timeline@1.7//changelog/CHANGELOG.html)

- com.unity.xr.arcore: [5.1.6](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.1//changelog/CHANGELOG.html) to [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.2//changelog/CHANGELOG.html)

- com.unity.xr.arfoundation: [5.1.6](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.1//changelog/CHANGELOG.html) to [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.2//changelog/CHANGELOG.html)

- com.unity.xr.arkit: [5.1.6](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.1//changelog/CHANGELOG.html) to [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.2//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.5.1](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) to [2.5.2](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.xr.meta-openxr: [1.0.1](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@1.0//changelog/CHANGELOG.html) to [1.0.3](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@1.0//changelog/CHANGELOG.html)

- com.unity.xr.oculus: [4.5.0](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) to [4.5.1](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.14.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html) to [1.14.2](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html)

- com.unity.terrain-tools: [5.0.5](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.0//changelog/CHANGELOG.html) to [5.0.6](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.0//changelog/CHANGELOG.html)

- com.unity.memoryprofiler: [1.1.5](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.6](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- com.unity.polyspatial: [1.3.11](https://docs.unity3d.com/Packages/com.unity.polyspatial@1.3//changelog/CHANGELOG.html) to [1.3.12](https://docs.unity3d.com/Packages/com.unity.polyspatial@1.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.visionos: [1.3.11](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@1.3//changelog/CHANGELOG.html) to [1.3.12](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@1.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.xr: [1.3.11](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@1.3//changelog/CHANGELOG.html) to [1.3.12](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@1.3//changelog/CHANGELOG.html)

- com.unity.xr.visionos: [1.3.11](https://docs.unity3d.com/Packages/com.unity.xr.visionos@1.3//changelog/CHANGELOG.html) to [1.3.12](https://docs.unity3d.com/Packages/com.unity.xr.visionos@1.3//changelog/CHANGELOG.html)