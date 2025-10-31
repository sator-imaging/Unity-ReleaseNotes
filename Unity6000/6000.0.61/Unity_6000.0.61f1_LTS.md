# Unity 6000.0.61f1 LTS
Published at Thu, 30 Oct 2025 06:44:03 GMT  
https://unity.com/releases/editor/whats-new/6000.0.61f1

# Known Issues in 6000.0.61f1

- Metal: The Player freezes and Execution of the command buffer was aborted due to an error. Several games started having freezes after the CAMetalDisplayLink was added.
    ([UUM-111494](https://issuetracker.unity3d.com/issues/ios-the-player-freezes-and-execution-of-the-command-buffer-was-aborted-due-to-an-error-during-execution-dot-error-is-continuously-logged))

- 3D Physics: No valid hits are returned when using RaycastCommand
    ([UUM-123124](https://issuetracker.unity3d.com/issues/no-valid-hits-are-returned-when-using-raycastcommand))

- Android: [GameActivity] APK built with Development Build enabled gets flagged as having Malware
    ([UUM-116588](https://issuetracker.unity3d.com/issues/android-gameactivity-apk-built-with-development-build-enabled-gets-flagged-as-having-malware))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DirectX12: [Intel] Crash on BufferD3D12::BeginWrite when opening a newly created URP project with DirectX12 set as the default graphics API
    ([UUM-104889](https://issuetracker.unity3d.com/issues/crash-on-bufferd3d12-beginwrite-when-opening-a-newly-created-urp-project-with-directx12-set-as-the-default-graphics-api))

- Editor Application Shell Integration: [Linux] Crash on ModalProgressBackendLinux::Clear when Domain Reload progress bar appears 
    ([UUM-122055](https://issuetracker.unity3d.com/issues/linux-crash-on-modalprogressbackendlinux-clear-when-domain-reload-progress-bar-appears))

- GPU Resident Drawer: False Warning "BatchRendererGroups currently don't support override shaders" is spammed in Play mode when using H-Trace WSGI with BatchRenderGroups
    ([UUM-122367](https://issuetracker.unity3d.com/issues/warning-batchrenderergroups-currently-dont-support-override-shaders-is-spammed-in-play-mode-when-using-h-trace-wsgi-with-batchrendergroups))

- License: Builds failing with the Error Code 404
    ([UUM-121408](https://issuetracker.unity3d.com/issues/file-watcher-does-not-trigger-after-the-acquirefloatinglease-and-before-the-entitlement-check))

- Metal: Crash on mono_dump_native_crash_info in a project with a Render Pipeline, which uses a 2D renderer when changing the Shader of a material to Standard Unlit 
    ([UUM-121727](https://issuetracker.unity3d.com/issues/crash-on-mono-dump-native-crash-info-when-changing-a-particle-system-renderers-material-shader-to-standard-unlit))

- Serialization: Editor performance degrades when PlayableDirector with multiple bindings remains visible in the Inspector during Play mode
    ([UUM-122354](https://issuetracker.unity3d.com/issues/editor-performance-degrades-when-playabledirector-with-multiple-bindings-remains-visible-in-the-inspector-during-play-mode))

- Shader System: Crash on tlsf_free when selecting a cube in the "Getting Started With Unity" template
    ([UUM-107673](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-adding-a-3d-object-to-a-scene-of-a-new-universal-3d-project))



# 6000.0.61f1 Release Notes

## Features

- Bug Reporter: Use the email address for the Unity ID logged into the Hub in the bug reporter.

- Version Control: Added a new Editor Toolbar Button for Unity Version Control that lets you view project status, track changes, and perform key actions with one click.

- Version Control: Added Unity Version Control actions to the prefab and prefab variant header context menus.

- Version Control: Added Unity Version Control status icons to prefab assets in the hierarchy view in "Edit Mode".



## Improvements

- Bug Reporter: Signed the bug reporter on MacOS.

- Bug Reporter: Signed the bug reporter on Windows.



## Changes

- Bug Reporter: Replaced the Unity Bug Reporter.

- Version Control: Improved overlay icons to align with the Unity Editor design. Added icons for "Controlled" and "Changed" items, removed the icon for "Private" items, and added a "Contains Changes" overlay for directories containing changes.



## Fixes

- 2D: Allow Tile Palette Edit Mode to persist when entering Play mode.
    ([UUM-117622](https://issuetracker.unity3d.com/issues/tile-palette-edit-mode-turns-off-in-play-mode))

- 2D: Fixed Assertion error "\(dx - width &lt; padding\) \|\| \(dy - height &lt; padding\)" when using Pack Preview.
    ([UUM-116057](https://issuetracker.unity3d.com/issues/assertion-error-dx-width-padding-dy-height-padding-when-using-pack-preview))

- 2D: Fixed crash issue with the TilemapRenderer where the TilemapRenderer is destroyed while the graphics renderer is still rendering the TilemapRenderer.
    ([UUM-119285](https://issuetracker.unity3d.com/issues/android-native-crash-on-tilemaprendererjobs))

- 2D: Fixed Create New Tile Palette/Create New Target dropdown menu's vertical alignment when there are no selected options available.
    ([UUM-117545](https://issuetracker.unity3d.com/issues/create-new-tile-palette-dropdown-text-is-not-centered-and-text-is-cut-off))

- 2D: Fixed issue where the "Invalid SortingGroup index set in Renderer" assert is triggered when multiple SortingGroups and SpriteRenderers are disabled and enabled in a single frame without a SortingGroupManager.Update occurring.
    ([UUM-119198](https://issuetracker.unity3d.com/issues/invalid-sortinggroup-index-set-in-renderer-errors-when-making-many-modifications-in-same-frame))

- 2D: Fixed memory regression from Light2D shader.
    (UUM-119296)

- 2D: Fixed Tile Palette Active Target being changed when saving the scene.
    ([UUM-119587](https://issuetracker.unity3d.com/issues/tilemap-selection-resets-to-the-default-when-the-scene-is-saved))

- 2D: Fixed Tile Palette view changing when entering Play mode.
    ([UUM-117623](https://issuetracker.unity3d.com/issues/tile-palette-grid-is-moved-after-entering-play-mode))

- Android: Renamed Android JNI tests that share the same name "TestProcess".

- Android: \[Android\] Upgrade Gradle and Android Gradle Plugin versions to fix development build APKs being incorrectly flagged as malware on Unity 6.0.
    ([UUM-116588](https://issuetracker.unity3d.com/issues/android-gameactivity-apk-built-with-development-build-enabled-gets-flagged-as-having-malware))

- Animation: Fixed corrupted animator window because of dangling animator controller serialized in the layout.
    (UUM-117808)

- Animation: Fixed issues where normalized time would not be incrementing on some animator states, along with excessive errors being logged.
    ([UUM-121440](https://issuetracker.unity3d.com/issues/animator-is-still-spamming-too-much-when-states-stay-active-too-long))

- Animation: Fixed memory leak caused by accumulating event handlers in IMGUI inspectors when changing GameObject selection.
    ([UUM-121239](https://issuetracker.unity3d.com/issues/inspectorelement-and-animationmode-memory-leak-when-selecting-different-gameobjects-in-the-hierarchy-with-the-inspector-tab-open))

- Audio: Fixed a bug that would cause the audio to not resume properly after unpausing a timeline.
    ([UUM-91654](https://issuetracker.unity3d.com/issues/audio-does-not-resume-playing-in-timeline-when-timescale-is-set-to-0-and-back-to-1-after-the-remainder-of-the-audio-has-passed-in-real-time))

- Editor: Allow to use backspace key to delete gradient field keys.
    ([UUM-122403](https://issuetracker.unity3d.com/issues/cant-delete-gradient-keys-with-mac-keyboard-or-context-menu-options))

- Editor: Fixed an Editor crash happening when .shader files contain raygeneration, miss or callable shaders. These shader types are supported in .raytrace files only.
    ([UUM-109230](https://issuetracker.unity3d.com/issues/dx12-crash-on-shaderlab-subprogram-compile-or-freeze-when-compiling-a-specific-ray-tracing-shader))

- Editor: Fixed an issue where popup menus with submenus could be placed incorrectly on macOS when deep submenu items were selected.
    ([UUM-116574](https://issuetracker.unity3d.com/issues/macos-rendering-debugger-volumes-component-dropdown-is-opened-with-a-big-offset-when-component-field-is-set-to-any-sample-scene))

- Editor: Fixed an issue where using the "Select Texture" window would, in certain specific scenarios, spam the console with errors related to an uninitialized variable.
    ([UUM-119204](https://issuetracker.unity3d.com/issues/2d-urp-error-spam-when-textures-in-select-texture-window-dont-have-description))

- Editor: Fixed corrupted kernings.
    ([UUM-121371](https://issuetracker.unity3d.com/issues/font-kerning-breaks-at-runtime-when-multiple-ui-documents-use-different-fonts))

- Editor: Fixed crash in AssetDB worker process.
    ([UUM-112436](https://issuetracker.unity3d.com/issues/crash-on-workerlicense-hasentitlement-when-starting-the-editor))

- Editor: Fixed crash when inputting long text in IMGUI.
    ([UUM-120863](https://issuetracker.unity3d.com/issues/crash-on-material-getshader-when-pasting-an-unusually-large-block-of-text-into-a-gameobjects-name-field))

- Editor: Fixed inability to drag Tabs to a display right of primary in Windows Editor when using different DPI scales.
    ([UUM-116022](https://issuetracker.unity3d.com/issues/window-preview-appears-on-a-different-monitor-when-undocking-and-dragging-a-window-with-a-high-resolution-monitor-set-up-on-the-right-and-a-low-resolution-monitor-on-the-left))

- Editor: Fixed issue with a Build Profile tooltip not showing correct path to Build Profile asset if it was moved.

- Editor: Fixed Manual license activation flow via command-line.
    (UUM-122146)

- Editor: Fixed missing underline in primary font preventing text rendering.
    ([UUM-120878](https://issuetracker.unity3d.com/issues/ui-toolkit-button-text-is-not-rendered-when-the-button-has-fixed-height-with-specific-icon-font))

- Editor: Fixed possible crashes and exceptions when triggering a scene save from script with an unsaved "Untitled" scene.
    ([UUM-121358](https://issuetracker.unity3d.com/issues/urp-crash-on-gameobject-querycomponentbytype-when-accessing-a-component-from-an-unsaved-template-created-scene))

- Editor: Fixed Tesselation plus Quad topology plus SRP Batcher.
    ([UUM-121990](https://issuetracker.unity3d.com/issues/automatic-lod-fails-and-srp-batcher-incompatibility-occurs-when-using-spline-based-quad-topology-meshes))

- Editor: Fixed thread exception when using Fonts instead of FontAssets.
    (UUM-121614)

- Editor: Fixed: https://jira.unity3d.com/browse/UUM-108146<br>
    NullReferenceException thrown when Terrain component is removed and re-added with the existing Terrain data.
    (UUM-108146)

- Editor: Open Popups and Tooltips on the display the mouse is currently on for Windows Editor when monitor look-up fails.
    ([UUM-117239](https://issuetracker.unity3d.com/issues/ui-toolkit-window-popups-are-cropped-when-using-an-uhd-monitor-coupled-with-a-lower-resolution-monitor))

- Editor: Removed missing scripts in SplitScreen and OcclusionEffect scenes from the URP samples.
    ([UUM-71852](https://issuetracker.unity3d.com/issues/urp-package-samples-missing-scripts-in-unity-2022-plus))

- Editor: Replaced the Active Input Handling set to the new Input System instead of the "Both" option.'.
    ([UUM-109503](https://issuetracker.unity3d.com/issues/the-com-dot-unity-dot-template-dot-urp-blank-and-com-dot-unity-dot-template-dot-hdrp-blank-templates-have-active-input-handling-set-to-both))

- Editor: Updated Unity Editor icon on mac for macOS 26 "Liquid Glass" design.
    ([UUM-120993](https://issuetracker.unity3d.com/issues/mac-editor-unity-editor-icon-does-not-follow-macos-tahoe-guidelines))

- GI: Ensured that we don't crash the Editor in a specific edge case, when a reflection probe is added to a scene which has never been saved and the scene is then baked without first explicitly saving the scene.
    ([UUM-120770](https://issuetracker.unity3d.com/issues/urp-crash-on-gameobject-querycomponentbytype-when-baking-a-reflection-probe-in-an-unsaved-slash-untitled-scene))

- Graphics: Color Picker - Swatches - HDR - Was storing the color.gamma instead of the color.
    ([UUM-121056](https://issuetracker.unity3d.com/issues/incorrect-color-values-are-saved-for-swatches-when-using-hdr-color-picker))

- Graphics: Fixed ComputeBuffer.GetData sometimes not waiting for gpu to finish.
    (UUM-122369)

- Graphics: Fixed occasional crash on exit.
    ([UUM-120761](https://issuetracker.unity3d.com/issues/crash-on-playermain-int-char-const-star-star-when-exiting-standalone-player-with-a-particle-system-in-the-scene))

- Graphics: Fixed unreferenced assets not being destroyed when switching scenes or calling Resources.UnloadUnusedAssets when using GPU Resident Drawer.
    ([UUM-120539](https://issuetracker.unity3d.com/issues/memory-usage-rises-when-switching-scenes-with-grd-enabled-and-a-loaded-texture-in-urp))

- Graphics: Removed GC allocations caused by RayTracingAccelerationStructure.AddInstances.
    ([UUM-121305](https://issuetracker.unity3d.com/issues/raytracingaccelerationstructure-dot-addinstances-causes-gc-allocations))

- HDRP: Fixed GC Allocation in Lens Flare Post Processing effect.
    ([UUM-108846](https://issuetracker.unity3d.com/issues/per-frame-gc-allocation-when-using-hdrp-lens-flare-post-process-effect))

- Input System: Fixed mouse warp not working correctly on macOS since it would not update Mouse position state.
    ([UUM-121296](https://issuetracker.unity3d.com/issues/the-mouse-position-is-not-updated-when-the-mouse-dot-warpcursorposition-function-is-executed))

- iOS: Fixed a bug related to changing the default audio output device while recording from the built-in microphone. In that case, sometimes microphone data would stop being captured properly.
    ([UUM-98507](https://issuetracker.unity3d.com/issues/ios-audiosource-errors-slash-warning-logged-and-audiosettings-dot-onaudioconfigurationchanged-event-not-called-when-disconnecting-the-bluetooth-heaphones-from-the-device))

- iOS: Fixed a crash with -nographics launch argument \(Simulator only\).
    (UUM-117757)

- Linux: Fixed Steam Deck D-Pad is either not working or sometimes working when UI-&gt;Navigation is set to "Pass Through" in Input Actions.
    ([UUM-97138](https://issuetracker.unity3d.com/issues/linux-d-pad-is-either-not-working-or-sometimes-working-when-ui-navigation-is-set-to-pass-through-in-input-actions))

- Plugins: AMDUnityPlugin/FSR2: Fixed white flickering around the edges of the image when the camera is rotated.
    ([UUM-110296](https://issuetracker.unity3d.com/issues/white-edges-appear-during-camera-movement-in-runtime-when-using-fsr2-with-motion-vectors-and-exposure-enabled))

- Scene/Game View: Fixed an issue where the editor would throw if layers StateCache json file was empty.
    ([UUM-116877](https://issuetracker.unity3d.com/issues/error-nullreferenceexception-object-reference-not-set-to-an-instance-of-an-object-is-present-when-opening-the-project-or-reloading-the-domain))

- Scene/Game View: Fixed Shortcut Manager's UI elements overlapping when window is resized down to narrow width.
    ([UUM-115947](https://issuetracker.unity3d.com/issues/ui-elements-overlap-in-the-shortcuts-window-when-docked-and-resized-to-a-smaller-window-size))

- Scene/Game View: Fixed the Cameras overlay popup having the wrong height when first person controls are toggled in the overlay.
    ([UUM-110292](https://issuetracker.unity3d.com/issues/cameras-menu-window-size-is-broken-when-control-the-selected-camera-in-first-person-dot-is-selected))

- Services: Fixed exception events not appearing on the Diagnostics dashboard.
    (ULO-7366)

- Shadergraph: Fixed extra scrollbars sometimes appearing in ShaderGraph blackboard when dragging attributes.
    ([UUM-108024](https://issuetracker.unity3d.com/issues/vertical-and-horizontal-scrollbars-appear-and-disappear-when-dragging-an-attribute-to-a-different-position-within-the-shader-graph-hierarchy))

- Shaders: Fixed unnecessary shader warnings and errors being logged when running with -batchmode -nographics.
    ([UUM-114187](https://issuetracker.unity3d.com/issues/unnecessary-warnings-are-logged-when-running-player-with-batchmode-nographics))

- SRP Core: Dispose of compiled graphs on cleanup.
    (UUM-117495)

- Terrain: Added missing selected icons for Terrain properties.
    ([UUM-114855](https://issuetracker.unity3d.com/issues/terrain-property-icons-blends-in-when-selected-in-animation-window-with-the-light-editor-theme-enabled))

- TextMeshPro: Fixed incorrect preferred height calculations when using more than one font per line of text.
    ([UUM-104237](https://issuetracker.unity3d.com/issues/incorrect-preferred-height-calculation-when-a-single-text-line-uses-different-font-assets))

- TextMeshPro: Improved CJK line break handling.
    ([UUM-121295](https://issuetracker.unity3d.com/issues/a-specific-project-freezes-when-content-size-fitters-horizontal-fit-is-set-to-min-size-and-it-contains-double-ellipses-followed-by-a-cjk-character))

- TextMeshPro: Improved line breaking for Chinese and Japanese.
    ([UUM-120042](https://issuetracker.unity3d.com/issues/line-break-position-changes-in-traditional-chinese-when-consecutive-punctuation-is-used))

- UI Toolkit: Added ClearValue API to allow any numeric input field to be cleared.
    ([UUM-122277](https://issuetracker.unity3d.com/issues/uitk-controls-non-text-inputfield-cant-be-reset-by-api))

- UI Toolkit: Fixed gradient fields in UI Builder not using correct timing numbers, causing a green key to appear out of place.
    ([UUM-122159](https://issuetracker.unity3d.com/issues/gradient-editor-window-bottom-right-gradient-marker-color-is-incorrect))

- UI Toolkit: Fixed null exception sometimes thrown when removing focus from element that's no longer in a panel while inside another event callback.
    ([UUM-121130](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-specific-ui-toolkit-focus-changes-are-made))

- UI Toolkit: Fixed the incorrect padding top applied on the collection view's contentContainer when rebuilding a list with a valid offset.
    ([UUM-92179](https://issuetracker.unity3d.com/issues/the-blackboard-scrolls-to-the-top-and-generates-an-artifact-when-duplicating-attributes-when-the-blackboard-has-been-scrolled-down-and-the-custom-attributes-list-is-expanded))

- UI Toolkit: Fixed the item first item of the list view disappearing and the items not showing when spamming the add button.
    (UUM-114653)

- UI Toolkit: Removed unused background repeat fields in canvas settings in UI Builder.
    ([UUM-122232](https://issuetracker.unity3d.com/issues/non-editable-repeat-x-and-repeat-y-settings-appear-when-ui-builder-canvas-background-is-set-to-image))

- UNET: Fixed the UI Builder's selector pill being frozen when dragging and scrolling at the same time.
    ([UUM-93877](https://issuetracker.unity3d.com/issues/selector-gets-stuck-in-ui-if-scroll-is-used-while-dragging))

- Universal RP: Fixed Warning logged when injecting a pass on AfterRenderPostProcessing + X.
    ([UUM-109361](https://issuetracker.unity3d.com/issues/warnings-are-logged-and-rendererfeature-that-requests-an-intermediate-texture-does-not-work-when-adding-an-offset-to-the-renderpassevent))

- Version Control: Fixed applying shelves when some files cannot be checked out due to exclusive checkout lock rules. These files are now applied as local changes instead of failing the whole operation.

- Version Control: Fixed incorrect tab name showing as "Unity.PlasticSCM.Editor.PlasticW" with no icon when upgrading a project to Unity 6.x.

- Version Control: Fixed the missing "Hide" contextual menu on the Unity Version Control button in the Unity 6.3 Toolbar.

- VFX Graph: Fixed "An edge with the same input and output already exists" error popping in the graph.
    ([UUM-120233](https://issuetracker.unity3d.com/issues/an-edge-with-the-same-input-and-output-already-exists-is-thrown-when-operators-are-connected-to-blocks))

- VFX Graph: Properly handle empty enum values in the blackboard and now forbid to remove the last enum value so the list is never empty.
    ([UUM-120288](https://issuetracker.unity3d.com/issues/removing-all-enum-values-from-uint-property-in-vfx-blackboard-causes-argumentoutofrangeexception-error-and-breaks-blackboard))

- WebGL: WebGPU: fix compressed 3d textures if the WebGPU extension is available.
    ([UUM-121604](https://issuetracker.unity3d.com/issues/webgpu-compressed-3d-textures-fail-even-when-extension-is-available))




## Package changes in 6000.0.61f1

## Packages updated

- com.unity.netcode: [1.9.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.9//changelog/CHANGELOG.html) to [1.9.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.9//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.9.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.9//changelog/CHANGELOG.html) to [2.10.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.10//changelog/CHANGELOG.html)

- com.unity.ide.visualstudio: [2.0.23](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html) to [2.0.25](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html)

- com.unity.services.user-reporting: [2.0.11](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) to [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- com.unity.remote-config-runtime: [4.0.2](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@4.0//changelog/CHANGELOG.html) to [4.0.4](https://docs.unity3d.com/Packages/com.unity.remote-config-runtime@4.0//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.5.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.5//changelog/CHANGELOG.html) to [1.7.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- com.unity.xr.management: [4.5.1](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) to [4.5.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html)

- com.unity.xr.meta-openxr: [2.0.1](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.0//changelog/CHANGELOG.html) to [2.0.2](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.0//changelog/CHANGELOG.html)

- com.unity.profiling.systemmetrics.mali: [1.0.3](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)

**Packages deprecated**

- com.unity.muse.common - "This package is no longer supported. Muse is being replaced with Unity AI."

- com.unity.muse.sprite - "This package is no longer supported. Muse is being replaced with Unity AI."

- com.unity.muse.texture - "This package is no longer supported. Muse is being replaced with Unity AI."

- com.unity.muse.chat - "This package is no longer supported. Muse is being replaced with Unity AI."