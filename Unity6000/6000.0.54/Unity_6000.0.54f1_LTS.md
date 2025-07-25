# Unity 6000.0.54f1 LTS
Published at Wed, 23 Jul 2025 11:28:35 GMT  
https://unity.com/releases/editor/whats-new/6000.0.54

# Known Issues in 6000.0.54f1

- 2D: UI is not rendering and an error is thrown when FXAA is enabled and cameras are stacked in a 2D URP project
    ([UUM-110338](https://issuetracker.unity3d.com/issues/ui-is-not-rendering-and-an-error-is-thrown-when-fxaa-is-enabled-and-cameras-are-stacked-in-a-2d-urp-project))

- Asset - Database: Warnings appear in the Console window when opening a new project
    ([UUM-109594](https://issuetracker.unity3d.com/issues/warnings-appear-in-the-console-window-when-opening-a-new-project))

- Asset Store / Publisher portal: Fix for 6000.0.X: Accepting Asset Store EULA endless loop in Package Manager window
    (UUM-83711)

- Cloud Diagnostics: [Android]Crash on lib/arm64/libil2cpp.so when Unity Analytics and Engine Code stripping are enabled
    ([UUM-95408](https://issuetracker.unity3d.com/issues/android-crash-on-lib-slash-arm64-slash-libil2cpp-dot-so-when-unity-analytics-and-engine-code-stripping-are-enabled))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Environment Effects: [HDRP] Water displacement fades when camera move far in worldspace. 
    ([UUM-111903](https://issuetracker.unity3d.com/issues/hdrp-water-displacement-fades-when-camera-move-far-in-worldspace))

- Hub: Licensing Client fails to launch when opening Unity Hub
    ([UUM-103995](https://issuetracker.unity3d.com/issues/licensing-client-fails-to-launch-when-opening-unity-hub-1))

- Hub: Licensing Client fails to launch when opening Unity Hub (licensing client path is not found)
    ([UUM-103996](https://issuetracker.unity3d.com/issues/licensing-client-fails-to-launch-when-opening-unity-hub-licensing-client-path-is-not-found))

- Lighting: All baked data for all scenes using APV is always loaded in Editor
    ([UUM-104833](https://issuetracker.unity3d.com/issues/all-baked-data-for-all-scenes-using-apv-is-always-loaded-in-editor))

- Mono: Crash on mono_domain_jit_foreach when performing various Unity operations
    ([UUM-112001](https://issuetracker.unity3d.com/issues/crash-on-mono-domain-jit-foreach-when-performing-various-unity-operations))

- SRP XR: GameObjects are transparent when a custom fog renderer feature is enabled
    ([UUM-104832](https://issuetracker.unity3d.com/issues/gameobjects-are-transparent-when-a-custom-fog-renderer-feature-is-enabled))

- SRP XR: The Player renders black on a Quest headset when MSAA, Post Processing, and Spacewarm depth submission are enabled
    ([UUM-84612](https://issuetracker.unity3d.com/issues/the-player-renders-black-on-a-quest-headset-when-msaa-post-processing-and-spacewarm-depth-submission-are-enabled))

- UI Toolkit Controls: Persisted event listeners are reset when collapsing and expanding a component in the Inspector
    ([UUM-111210](https://issuetracker.unity3d.com/issues/persisted-event-listeners-are-reset-when-collapsing-and-expanding-a-component-in-the-inspector))

- Video: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    ([UUM-111599](https://issuetracker.unity3d.com/issues/videoplayer-freezes-or-stops-on-certain-android-devices-when-enabling-and-disabling-the-video-multiple-times))

- Vulkan: [Android] Runtime performance deteriorates on certain Android devices when Graphics API is set to Vulkan on an upgraded project
    ([UUM-107530](https://issuetracker.unity3d.com/issues/build-performance-deteriorates-on-certain-android-devices-when-graphics-api-is-set-to-vulkan-on-an-upgraded-project))



# 6000.0.54f1 Release Notes

## Improvements

- QNX: Enabled shader caching.



## API Changes

- Asset Pipeline: Added: Added FindAssetGUIDs methods that return an array of GUIDs instead of strings.

- Asset Pipeline: Added: Added LoadAssetByGUID method that accepts a GUID as an input argument.



## Changes

- Documentation: Added link to relevant area of Discussions on the multiplayer landing page.

- Editor: The game view rendering statistics window now displays a warning of incorrect triangle and vertex count when indirect draw calls are issued, such as is the case with GPU Occlusion Culling.
    ([UUM-102572](https://issuetracker.unity3d.com/issues/statistics-window-shows-incorrect-information-when-gpu-resident-drawer-and-gpu-occlusion-culling-are-enabled))

- XR: Updated com.unity.xr.openxr package version to 1.15.0.



## Fixes

- 2D: Fixed artifacts occurring on Metal when using Rendergraph pipeline.
    (UUM-109986)

- 2D: Fixed UI rendering when FXAA is enabled with camera stack.
    ([UUM-110338](https://issuetracker.unity3d.com/issues/ui-is-not-rendering-and-an-error-is-thrown-when-fxaa-is-enabled-and-cameras-are-stacked-in-a-2d-urp-project))

- 2D: Fixed URP 2D lighting with meshes in Rendergraph.
    (UUM-109312)

- 2D: Improved validation of RefreshTile Tilemap argument signature in Editor.
    ([UUM-109125](https://issuetracker.unity3d.com/issues/crash-on-tilemap-gettileasset-when-calling-tilemap-dot-gettile-in-new-refreshtile-method-for-tilebase-class))

- Accessibility: Set a minimum width on HierarchyViewer panes to fix resizing issues.
    ([UUM-109362](https://issuetracker.unity3d.com/issues/accessibility-hierarchy-viewer-sections-can-be-resized-to-zero-width))

- AI: Agent was not progressing past a corner between polygons of different area types.
    ([UUM-72975](https://issuetracker.unity3d.com/issues/navmeshagent-gets-stuck-when-going-over-a-vertex-of-a-higher-cost-area))

- AI: Agent was some times getting stuck in its movement along axis-aligned NavMesh edges.
    ([UUM-18593](https://issuetracker.unity3d.com/issues/game-objects-get-stuck-in-an-infinite-loop-when-passing-navmesh-surface-nodes))

- AI: Agent was taking steps back while trying to correct the path it had computed through the NavMesh.
    ([UUM-79120](https://issuetracker.unity3d.com/issues/nav-mesh-agent-gets-stuck-and-oscillate-when-traveling-along-edges-and-corners-of-nav-mesh-areas-with-different-costs))

- Android: Fixed a bug where calls lead to a state where starting new audio streams caused a main thread stall.
    ([UUM-103525](https://issuetracker.unity3d.com/issues/android-player-freezes-when-an-audio-source-is-playing-and-an-incoming-call-is-picked-up-and-then-hung-up-and-the-audio-source-is-started-again))

- Android: Fixed crash on GameActivity, when touching screen with 9 fingers or more. GameActivity only supports up to 8 fingers touching screen at the same time.
    ([UUM-108743](https://issuetracker.unity3d.com/issues/android-crash-on-unitymotioneventcallbacks-getpointeridimpl-when-giving-8-simultaneous-touch-inputs))

- Android: Fixed the problem with installing AAB to some Samsung devices which have Secure Folder.
    ([UUM-110694](https://issuetracker.unity3d.com/issues/android-exception-shell-does-not-have-permission-to-access-user-150-and-app-does-not-get-deployed-on-a-samsung-device-with-secure-folder-when-building-an-app-bundle-google-play))

- Android: Fixed warning showing libraries as not 16 KB page aligned when they have been updated externally.
    ([UUM-111393](https://issuetracker.unity3d.com/issues/android-native-libraries-dot-so-are-not-checked-for-16kb-alignment-when-modified-externally))

- Animation: Fixed an issue where a state machine state's name would be extending beyond the bounds of the node if the name was too long.
    ([UUM-107423](https://issuetracker.unity3d.com/issues/animator-state-name-overflows-outside-the-visual-box-when-the-state-has-a-long-name))

- Asset Import: Detect a corrupt library when loading a project in the Unity Editor, and present an error message with instructions on how to delete the corrupt library, with documentation URL.
    ([UUM-109873](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-opening-a-specific-project-1))

- Asset Import: Fixed indeterminism of artifact ids which could occur when importers set dependencies to other assets.
    (UUM-107448)

- Asset Pipeline: Asset Import workers could get out of sync with their main editor process, rendering them unable to load assets.
    (UUM-100493)

- DX12: Fixed for crash when running with Native Jobs.
    (UUM-110198)

- Editor: "Asset Labels" section should not appear when a non-asset is being selected.
    ([UUM-110356](https://issuetracker.unity3d.com/issues/asset-labels-section-appears-in-inspector-when-selecting-a-scene-gameobject))

- Editor: Avoid rare crash while sending Analytics during Licensing operations.
    (UUM-111546)

- Editor: Changed the TextInputBaseField Blur behaviour so that it now resets and scrolls the text back to the start when focus is lost.
    (UUM-73005)

- Editor: Exception thrown when renaming component with symbols in UIBuilder.
    ([UUM-107901](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-errors-are-thrown-everytime-a-keyboard-key-is-pressed-when-renaming-a-component-in-ui-builder-with-a-symbol-and-changing-the-name-after-label-attribute-warning))

- Editor: Fixed a bug where ctrl + left click would not open the contextual menu for the Orientation Gizmo and added support for Mac's two-finger click.
    (UUM-102749)

- Editor: Fixed an exception when accessing the toolbar of the animator window with a deleted animator.
    ([UUM-107430](https://issuetracker.unity3d.com/issues/animator-window-has-a-dropdown-button-that-throws-missingreferenceexception-error-on-a-new-project-when-the-previous-project-had-a-gameobject-with-an-animation))

- Editor: Fixed Cursor.visible ignoring CursorLockMode.Locked.
    ([UUM-85853](https://issuetracker.unity3d.com/issues/mouse-pointer-remains-visible-on-screen-when-cursor-dot-lockstate-is-set-to-cursorlockmode-dot-locked-and-cursor-dot-visible-gets-set-to-true-in-update))

- Editor: Fixed distorted TagManagerInspector pop up window if tag confirmed using Enter.
    ([UUM-110586](https://issuetracker.unity3d.com/issues/the-tag-popup-window-is-deformed-and-stretched-out-when-creating-a-tag-with-the-same-name-as-an-already-existing-tag))

- Editor: Fixed IMGUI EditorGUIUtility.labelWidth value being changed by the Scene View UI. This could impact other windows drawn afterwards.
    ([UUM-110450](https://issuetracker.unity3d.com/issues/editorguilayout-dot-toggle-clickable-area-is-shifted-when-using-built-in-render-pipeline))

- Editor: Fixed prefab stage applying changes too early.
    ([UUM-107890](https://issuetracker.unity3d.com/issues/values-in-rect-transform-component-are-only-partially-updated-when-changing-values-in-prefab-mode))

- Editor: Fixed renaming profiles adding a suffix '1' with capitalization only edits.
    (UUM-104025)

- Editor: Fixed SerializedProperty errors that could occur when editing and canceling the edit for an int2 followed by float2.
    ([UUM-110524](https://issuetracker.unity3d.com/issues/serializedproperty-errors-are-thrown-when-pressing-the-esc-key-to-cancel-the-modification-of-int-or-float-values))

- Editor: Fixed the method to get object picker control ID while avoiding creating a new instance.
    ([UUM-110121](https://issuetracker.unity3d.com/issues/invalid-editor-window-of-type-unityeditor-dot-objectselector-error-message-is-thrown-when-maximizing-any-editor-window))

- Editor: Fixed Underline with font fallback chain.
    ([UUM-110065](https://issuetracker.unity3d.com/issues/the-text-underline-partially-disappears-when-the-bold-effect-is-applied-with-certain-fonts-in-the-ui-builder))

- Editor: LaunchScreen for Windows Editor only closed with Esc key and not also Enter.
    ([UUM-111095](https://issuetracker.unity3d.com/issues/editor-launch-screen-will-close-when-enter-is-pressed-on-it))

- Editor: Random crash in BatchRendererGroup rendering fixed.
    (UUM-105252)

- Editor: Removed redundant NUnit include from SRP Core code.
    (UUM-110025)

- Editor: Updated 7-Zip to 25.00.

- GI: Fixed case where custom properties on a Renderer are not taken into account, leading to incorrectly baked lightmaps.
    ([UUM-108565](https://issuetracker.unity3d.com/issues/material-property-block-emits-and-reflects-incorrect-color-when-baked-indirect-light-is-used))

- Graphics: Fixed additional separator in menu when the VolumeComponent is in the default VolumeProfile.
    ([UUM-108517](https://issuetracker.unity3d.com/issues/double-separation-lines-are-present-in-override-controls-in-a-defaultvolumeprofile-asset))

- Graphics: Fixed additional separator in menu when there is no advanced properties in the VolumeComponent.
    ([UUM-108543](https://issuetracker.unity3d.com/issues/double-separation-lines-are-present-in-override-controls-in-a-new-volume-profile-asset))

- HDRP: Fixed material debug view when path tracing is enabled.
    ([UUM-103401](https://issuetracker.unity3d.com/issues/rendering-debugger-throws-a-warning-and-renders-the-scene-view-in-solid-black-when-material-debug-tools-and-path-tracing-are-used))

- HDRP: Fixed the position node in ShaderGraph with the fog volume material type not working as intended.
    ([UUM-83347](https://issuetracker.unity3d.com/issues/local-volumetric-fog-gameobject-ignores-position-node-settings-when-applying-a-custom-fog-volume-shadergraph))

- IL2CPP: Ensure macOS `.dSYM` debug symbol bundles are reliably copied to the build output on clean builds when detailed stacktraces are enabled.
    ([UUM-108362](https://issuetracker.unity3d.com/issues/dsym-file-is-not-created-during-macos-standalone-build))

- IL2CPP: Fixed issue where Linux was running out of memory pages due to them not being returned.
    (UUM-110285)

- IL2CPP: Prevent possible shutdown deadlock when using waits with zero time out.
    ([UUM-104910](https://issuetracker.unity3d.com/issues/player-with-il2cpp-scripting-backend-crashes-when-calling-application-dot-quit-while-a-thread-is-running))

- IMGUI: Fixed fallback font weight for Roboto-Mono in IMGUI.
    ([UUM-110337](https://issuetracker.unity3d.com/issues/monospaced-fonts-do-not-maintain-a-fixed-width-when-using-the-bold-variants))

- Kernel: Fixed rare deadlock on Windows in `Resources.UnloadUnusedAssets`.
    (UUM-100691)

- Mono: Fixed crash on incorrectly optimized calls to EqualityComparer&lt;T&gt;.Default in Generic Record Type Equals implementations.
    ([UUM-99151](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-checking-for-null-equality-in-a-specific-variable))

- Mono: Fixed crash on some default interface method calls.
    ([UUM-99049](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-using-default-interface-methods))

- Mono: Fixed crash that would occur due to symbol collision between builtin Brotli compression and system installed versions.
    ([UUM-108000](https://issuetracker.unity3d.com/issues/silicon-freeze-slash-crash-on-brotlidecoderdecompressstream-when-using-system-dot-io-dot-compression-dot-brotlidecoder-dot-trydecompress))

- Mono: Fixed issue where mono's debugger agent thread would not restart when a connection issue was encountered.
    (UUM-107431)

- Player: The DeveloperConsole now correctly opens after being re-enabled, fixing an issue where it would remain stuck in a closed state.
    ([UUM-109718](https://issuetracker.unity3d.com/issues/debug-console-does-not-reappear-when-disabling-and-re-enabling-debug-dot-developerconsoleenabled))

- Profiler: Align profiler frame duration of Edit mode profiling with Play mode when playing.
    ([UUM-74665](https://issuetracker.unity3d.com/issues/the-profiler-ignores-a-modified-targetframerate-when-profiling-edit-mode))

- Scene/Game View: Fixed an issue where Focus Pan command would often set an impractical zoom pivot if Canvas object was picked.
    ([UUM-108790](https://issuetracker.unity3d.com/issues/scene-view-doesnt-select-the-canvas-when-its-clicked-with-the-view-tool))

- Scripting: Optimized the Main Thread times of InstantiateAsync and added a new OriginalImmutable flag to reduce the times even more.
    ([UUM-102307](https://issuetracker.unity3d.com/issues/long-scheduler-times-on-main-thread-when-using-instantiateasync-with-a-singular-massive-prefab))

- TextCore: Make sure disabled TextField do not collapse.
    ([UUM-103184](https://issuetracker.unity3d.com/issues/text-field-becomes-narrow-when-selecting-children-of-toggle-element-in-ui-builder))

- uGUI: Updated Image raycast behavior to ensure consistent handling of screenPoints outside bounds, preventing parent Images from blocking child Images.
    ([UUM-110769](https://issuetracker.unity3d.com/issues/child-image-does-not-trigger-an-event-when-the-parent-image-is-using-alphahittestminimumthreshold-0))

- UI Toolkit: Clicking on Spacing/Border Widget values in the UI Builder now selects these values.
    ([UUM-105818](https://issuetracker.unity3d.com/issues/ui-builder-value-is-not-selected-when-left-clicking-on-spacing-slash-border-widget-values))

- UI Toolkit: Clicks in dead zones of the canvas selection header won't select the element underneath in UI Builder.
    ([UUM-107380](https://issuetracker.unity3d.com/issues/ui-builder-viewports-tool-gizmo-has-deadzones))

- UI Toolkit: Ensure margin gizmo stays visible while dragging.
    ([UUM-105900](https://issuetracker.unity3d.com/issues/ui-builder-viewports-gizmos-for-margin-and-padding-disappear-when-dragging-to-modify-the-value-and-the-cursor-leaves-the-spacing-section))

- UI Toolkit: Fixed an exception thrown by the runtime dropdown field when choices list is empty.
    ([UUM-105552](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-an-empty-dropdownfield-is-clicked-at-runtime))

- UI Toolkit: Fixed an exceptions when displaying PropertyFields bound to an array named "Array" in the inspector.
    ([UUM-110573](https://issuetracker.unity3d.com/issues/binding-listview-failed-warning-is-thrown-when-a-gameobject-with-an-attached-script-containing-an-array-or-list-named-array-is-selected))

- UI Toolkit: Fixed an issue in UI Builder where clicking the scrollbar buttons in the code preview would focus and select the content.
    ([UUM-105775](https://issuetracker.unity3d.com/issues/ui-builder-scroll-button-for-code-preview-section-automatically-selects-all-of-the-code))

- UI Toolkit: Fixed an issue where the IMGUI TreeView's context menu option to rename wouldn't work when the containing view was not focused.
    ([UUM-110067](https://issuetracker.unity3d.com/issues/gameobject-cannot-be-renamed-when-right-clicked-and-a-different-window-is-in-focus))

- UI Toolkit: Fixed an issue with PropertyFields bound to an array named "Array" throwing an exception when the add button was clicked.
    ([UUM-110572](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-attempting-to-add-an-element-to-an-array-or-list-named-array-in-the-inspector))

- UI Toolkit: Fixed bound fields not showing an indication if they were animated or driven.
    (UUM-105089)

- UI Toolkit: Fixed change events being sent when the text had not changed, but the precision of the text value did not exactly match the float value.
    ([UUM-100527](https://issuetracker.unity3d.com/issues/the-inspector-rounds-up-float-values-up-to-a-maximum-of-7-digits-and-overwrites-the-actual-values-in-the-file-when-saving-the-asset))

- UI Toolkit: Fixed crash when stroking rounded joins with Painter2D.
    ([UUM-110455](https://issuetracker.unity3d.com/issues/crash-on-uitoolkit-uipainter2d-strokeroundedcap-when-drawing-an-arc-with-painter2d-on-specific-progress-value-using-linecap-dot-round))

- UI Toolkit: Fixed elements sometimes still referenced in memory after being removed from their panel.
    ([UUM-109369](https://issuetracker.unity3d.com/issues/memory-address-leaks-when-using-visual-elements-in-a-specific-project))

- UI Toolkit: Fixed focus in UI Builder code preview when clicking on ScrollView controls.
    ([UUM-105775](https://issuetracker.unity3d.com/issues/ui-builder-scroll-button-for-code-preview-section-automatically-selects-all-of-the-code))

- UI Toolkit: Fixed ListView bug where a drag operation would select the item even with SelectionType.None.
    (UUM-107346)

- UI Toolkit: Fixed property field indentation.
    ([UUM-108741](https://issuetracker.unity3d.com/issues/header-attribute-is-misaligned-when-placed-before-an-inputactionproperty-field))

- UI Toolkit: Fixed QuickSearch warning from removing an element during its AttachToPanel event.
    ([UUM-107328](https://issuetracker.unity3d.com/issues/modifying-the-parent-of-a-visualelement-while-its-already-being-modified-is-not-allowed-error-is-thrown-when-entering-text-and-pressing-tab-in-the-search-window))

- UI Toolkit: Fixed runtime dropdown checkmark styling.
    ([UUM-109393](https://issuetracker.unity3d.com/issues/check-mark-in-enum-element-is-misaligned-when-hovered-on-in-play-mode))

- UI Toolkit: Fixed the argument exception when docking a window that contains a RadioButtonGroup control.
    ([UUM-105010](https://issuetracker.unity3d.com/issues/argumentexception-cannot-unschedule-unknown-scheduled-function-error-thrown-when-filling-out-multiplayer-center-recommendation-tab))

- UI Toolkit: Text in the new selector field in UI Builder is no longer covered by the pseudo states button.
    ([UUM-109121](https://issuetracker.unity3d.com/issues/add-new-selector-input-text-is-partially-covered-by-the-add-pseudo-class-button))

- URP: Avoid persistent memory allocation \(_CameraTargetAttachmentX and _CameraUpscaledTargetAttachmentX\) in RenderGraph when possible \(single camera\), and use a RenderGraph texture instead.
    ([UUM-99384](https://issuetracker.unity3d.com/issues/cameratargetattachmentb-unnecessarily-allocates-memory-even-when-post-processing-is-disabled-and-camera-stacking-is-not-used))

- URP: RP converter was not displaying the results of the converters execution in the console.
    ([UUM-97117](https://issuetracker.unity3d.com/issues/urprenderpipelineconverter-no-message-in-the-console-after-the-successful-slash-failed-conversion))

- Video: Fixed an issue where the VideoPlayer component failed to play MP4 files from StreamingAssets on some Android devices using Vulkan. The required NV12 decode shaders are now correctly included, restoring video playback on affected hardware.
    ([UUM-105019](https://issuetracker.unity3d.com/issues/vulkan-on-certain-android-devices-unitys-videoplayer-component-fails-to-play-mp4-files-located-under-the-streamingassets-folder))

- Video: \[Android\] VideoPlayer leaks memory when repeating Play and Stop on a Video.
    ([UUM-77668](https://issuetracker.unity3d.com/issues/android-videoplayer-leaks-memory-when-repeating-play-and-stop-on-a-video))

- Windows: Fixed SystemInfo.deviceType to correctly return the type of device the Windows Standalone player is running on.
    (UUM-110392)

- XR: Fixed for the background motion vectors being generated incorrectly for spacewarp.




## Package changes in 6000.0.54f1