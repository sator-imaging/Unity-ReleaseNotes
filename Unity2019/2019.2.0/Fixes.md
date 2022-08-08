# Unity 2019.2.0

https://unity3d.com/unity/whats-new/2019.2.0

## Fixes



*   2D: Changed position of Tile Instantiated GameObject to align with the Tile Anchor position of the Tilemap.
    
*   2D: Cleaned up and updated the Sorting Group status of Renderers whose GameObjects were activated and then deactivated. ([1141682](https://issuetracker.unity3d.com/issues/invalid-sortinggroup-index-set-in-renderer-error-when-managing-sortinggroups-children-objects), 1151999)
    
*   2D: Edge Sprite Material changed when using a fill texture that is already an edge sprite on spriteshape. ([1157201](https://issuetracker.unity3d.com/issues/2d-spriteshape-edge-sprite-material-changed-when-using-a-fill-texture-that-is-already-an-edge-sprite-on-spriteshape), 1163660)
    
*   2D: Fixed an issue where a Particle System's Sorting Fudge value while it is in a Sorting Group caused it to sort correctly. Similar Renderers are now sorted according to their Sorting Group order.
    
*   2D: Fixed an issue where a Sprite Atlas did not change when its associated "Object for Packing" Texture was modified by a custom AssetPostprocessor script. ([1135638](https://issuetracker.unity3d.com/issues/spiteatlas-does-not-change-when-its-associated-object-for-packing-texture-is-modified-by-a-custom-assetpostprocessor-script))
    
*   2D: Fixed clipping of Tilemap selection option for Tilemap Focus Dropdown ([1158947](https://issuetracker.unity3d.com/issues/tilemap-focus-on-dropdown-text-gets-clipped-when-tilemap-option-is-selected), 1163376)
    
*   2D: Fixed crash when rendering a Hexagonal Tilemap with Top Left/Right Sort Order in Individual mode ([1142429](https://issuetracker.unity3d.com/issues/rendernodequeue-reset-crash-when-editing-hexagonal-tilemaps-with-top-left-slash-right-sort-order-and-individual-mode), 1155196)
    
*   2D: Fixed crash when setting SpriteRenderer to tiling draw mode when textureless Sprite is assigned ([1156756](https://issuetracker.unity3d.com/issues/unity-crash-when-svg-image-draw-mode-is-set-to-sliced-or-tiled), 1161725)
    
*   2D: Fixed links to documentation for Tilemap components. ([972901](https://issuetracker.unity3d.com/issues/tilemap-components-are-missing-links-to-docs))
    
*   2D: Fixed recomposite Collider2Ds with CompositeCollider2D when offset and vertex distance changes while in outline generation mode.
    
*   2D: Open ended Spriteshape renders the fill texture instead of the range sprite ([1162134](https://issuetracker.unity3d.com/issues/2d-spriteshape-open-ended-spriteshape-renders-the-fill-texture-instead-of-the-range-sprite), 1163663)
    
*   2D: Updated SortingLayerField and SpriteRendererEditor to correctly handle PrefabOverrides. ([1109376](https://issuetracker.unity3d.com/issues/material-and-sorting-layer-fields-of-sprite-renderer-component-do-not-show-prefab-overrides-in-inspector), 1151997)
    
*   Analytics: Fixed an issue where passing Unity objects to `AnalyticsEvent` caused allocation leak warnings. (1086690)
    
*   Android: Android now handles an Application.targetFrameRate value of -1 as 30 fps again.
    
*   Android: Fix performance penalty when using Vulkan on Android Q preview 5 (1169046, 1169302)
    
*   Android: Fixed a crash when using Android JNI methods from custom thread. ([545977](https://issuetracker.unity3d.com/issues/androidjava-star-is-crashing-when-used-from-custom-threads))
    
*   Android: Fixed a crash when using Optimized Frame Pacing with Vulkan. (1164435)
    
*   Android: Fixed an issue that caused APK builds to fail because Unity failed to retrieve the version code from the APK. ([1133867](https://issuetracker.unity3d.com/issues/android-build-and-run-doesnt-deploy-apk-on-device-when-split-apks-by-target-architecture-is-enabled))
    
*   Android: Fixed an issue that caused the build to fail when setting a keystore name from script. ([1158036](https://issuetracker.unity3d.com/issues/android-build-fails-when-setting-keystore-path-via-script-as-a-string-with-relative-path-value), 1162258)
    
*   Android: Fixed an issue that caused the Editor to crash when opening Player Settings withough having Android SDK set up. ([1143624](https://issuetracker.unity3d.com/issues/crash-macos-editor-crash-when-android-platform-is-selected-no-sdk-installed-and-player-settings-button-was-pressed), 1144223)
    
*   Android: Fixed an issue where custom Android libraries would not be initialized after launching an app after previously exiting the app via Application.Quit. ([1116123](https://issuetracker.unity3d.com/issues/vr-android-application-dot-quit-no-longer-causes-apps-to-fully-terminate-the-process-on-oculus-go))
    
*   Android: Fixed an issue where only part of a static splash image was visible on load when using a transparent splash image. ([1136826](https://issuetracker.unity3d.com/issues/android-only-part-of-static-splash-image-is-visible-on-load-when-splash-image-is-transparent))
    
*   Android: Fixed error "gradleOut-debug-unsigned.apk does not exist" that would occur while trying to build a signed development build. ([1137971](https://issuetracker.unity3d.com/issues/android-development-build-with-signed-keystore-fails-building-because-gradleout-debug-unsigned-dot-apk-does-not-exist))
    
*   Android: Fixed incomplete reading of large texture files. (1111919)
    
*   Android: Fixed large Unicode character marshaling between C# and Java on Android 4 and 5. ([1123693](https://issuetracker.unity3d.com/issues/android-strings-consisted-of-astral-characters-are-corrupted-on-5-or-lower-android-devices))
    
*   Android: Restored our previous method of managing Android signing keys and keystores. ([1144308](https://issuetracker.unity3d.com/issues/android-unable-to-load-or-use-keystore-with-password-due-to-incorrect-storepass-parameter-quoting), 1153333)
    
*   Android: The Y position for the touch and mouse are now inverted in the native backend instead of managed code using the new input system.
    
*   Animation: Allow deleting curve keys whilst dragging, without throwing errors. ([1129837](https://issuetracker.unity3d.com/issues/console-throws-indexoutofrangeexception-when-editing-curves-after-deleting-a-key-and-moving-a-mouse))
    
*   Animation: Fix live link not showing the right edge (1032879)
    
*   Animation: Fixed a crash when unloading animations that are part of an AnimatorController. (1122054)
    
*   Animation: Fixed an issue where RectTransform properties would show missing curves that were not actually missing ([1115014](https://issuetracker.unity3d.com/issues/animation-anchored-position-z-reads-as-missing-in-the-animation-window))
    
*   Animation: Fixed an issue where the Animation Component would stay ActiveAndEnabled when the GameObject was disabled. ([1094567](https://issuetracker.unity3d.com/issues/behaviour-dot-isactiveandenabled-returns-true-when-used-on-a-script-disabled-object-with-an-animation-component))
    
*   Animation: Fixed an issue where the AnimationEvent "Function" field would accept spaces. ([1111933](https://issuetracker.unity3d.com/issues/error-about-animation-event-not-having-a-receiver-when-the-events-function-field-is-ended-with-a-space))
    
*   Animation: Fixed an issue where the Animator would keep references to temporary strings when using ADBv2. (1137999, 1154360)
    
*   Animation: Fixed an issue where the Avatar preview would not react to ObjectSelector changes. ([1113154](https://issuetracker.unity3d.com/issues/animation-preview-model-does-not-appear-in-preview-tab-when-being-selected-through-avatar-tab))
    
*   Animation: Fixed an issue where the preview of transitions with exitTime == 0 would generate some NaN errors ([1092857](https://issuetracker.unity3d.com/issues/preview-window-of-a-transition-shows-nan-when-changing-transition-duration-after-selecting-a-state-in-the-animator-window))
    
*   Animation: Fixed AnimationUtility.SetAnimationClipSettings not regenerating runtime data. ([1091972](https://issuetracker.unity3d.com/issues/root-values-played-by-the-timeline-that-has-a-recorded-track-are-incorrect-when-using-setanimationclipsettings))
    
*   Animation: Fixed crash when changing controller in Animator Override Controller used in a Playable Graph. (1104518)
    
*   Animation: Fixed FileNotFoundException when double-clicking to open an Animator Controller asset. ([1127826](https://issuetracker.unity3d.com/issues/macos-filenotfound-exception-when-trying-to-open-an-animator-controller))
    
*   Animation: Fixed issue with .NET 4.0 causing issues with System.Single conversion (1057751)
    
*   Animation: Fixed memory leak in AnimationWindow when inspecting animation with large number of keyframes ([1092423](https://issuetracker.unity3d.com/issues/animation-window-is-leaking-memory-when-inspecting-animation-with-more-keyframes))
    
*   Animation: Fixed TransformStreamHandle.GetPosition not returning global position when applyRootMotion is off and user is controlling the root transform. ([1115701](https://issuetracker.unity3d.com/issues/transformstreamhandle-dot-getposition-doesnt-get-the-correct-world-space-position-when-the-apply-root-motion-is-disabled))
    
*   Animation: Properly stop graph when switching to manual update mode ([1084441](https://issuetracker.unity3d.com/issues/the-manual-mode-is-stuck-when-changing-directorupdatemode-to-manual-in-play-mode-via-script))
    
*   Animation: Right clicking on an item in a ReoderableList will select it, but will not trigger dragging logic ([907650](https://issuetracker.unity3d.com/issues/animation-parameter-is-not-selected-properly-when-deleting-it-by-using-lmb))
    
*   Asset Import: An error message now appears in the Texture Import Settings window when assigning an invalid texture format for a given platform and texture type. ([1115190](https://issuetracker.unity3d.com/issues/error-when-changing-format-to-bc5-with-textureimporter-and-a-pop-up-for-unapplied-import-settings-when-deselecting-texture))
    
*   Asset Import: Fixed a crash in the FBX Importer when calculating tangents on a blendshape that has infinite values in vertex positions. ([1152354](https://issuetracker.unity3d.com/issues/generatesharedverticesindexlist-crashes-when-importing-a-fbx-file), 1161614)
    
*   Asset Import: Fixed a problem with the Audio Importer which failed to save changes to platform specific settings when performing a Reset or applying an Audio Preset. ([1150491](https://issuetracker.unity3d.com/issues/presets-platform-settings-are-not-saved-for-audio-importer-preset), 1156484)
    
*   Asset Import: Fixed a regression where the contextual menu items for adding and deleting events were not working on the Animation tab of the Import Settings window. ([1136900](https://issuetracker.unity3d.com/issues/fbx-importer-contextual-menu-for-events-not-working-anymore), 1144451)
    
*   Asset Import: Fixed an issue where imported Assets were reverting to their names at the time of export, if they didn't match the name associated with the GUID. ([1130301](https://issuetracker.unity3d.com/issues/importing-unity-package-does-not-keep-track-of-renames))
    
*   Asset Import: Fixed an issue where re-importing a Shader caused a property size to keep growing even when the Shader failed to compile. ([1127367](https://issuetracker.unity3d.com/issues/surface-shader-inspector-ui-keeps-adding-albedo-texture-parameters-when-a-multidimensional-array-is-added-to-the-shader))
    
*   Asset Import: Fixed an issue with the model importer inspector material remapping section where the remapped materials are not properly updated after an item was added. ([1115556](https://issuetracker.unity3d.com/issues/remapped-materials-material-selector-only-works-once), 1160131)
    
*   Asset Import: Fixed cases where Sketchup files, originating from Sketchup 2019, failed to import successfully.
    
*   Asset Import: Fixed issue where clicking Cancel on the Import Package dialog failed to invoke the importPackageCancelled callback. ([1037916](https://issuetracker.unity3d.com/issues/assetdatabase-dot-importpackagecancelled-callback-is-not-called-at-all))
    
*   Asset Import: Fixed issue where Unity returned an error instead of creating an empty package if no Assets can be exported. ([1105480](https://issuetracker.unity3d.com/issues/exporting-package-without-exportpackageoptions-dot-recurse-exports-an-empty-package))
    
*   Asset Import: The Import Settings window now shows a specific error when the Editor is not a valid MonoScript type. (1127110)
    
*   Asset Management: Fixed issue where fbx files are not re-imported when a AssetPostprocessor implementing OnPostprocessAnimation has its version updated. ([1153110](https://issuetracker.unity3d.com/issues/asset-postprocessor-doesnt-reimport-fbx-file-with-animations-on-version-change-if-only-onpostprocessanimation-is-used), 1161616)
    
*   Asset Pipeline: Fix race condition crash when loading asset bundles from managed streams. ([1135251](https://issuetracker.unity3d.com/issues/crash-on-assetbundleloadfromasyncoperation-getassetbundleblocking-when-loading-assetbundles-via-loadfromstreamasync), 1157657)
    
*   Asset Pipeline: Fixed an issue where mutually recursive assets could cause a crash.
    
*   Asset Pipeline: Fixed an issue with Unity crashing when a Material that is highlighted in the Project window is overwritten from a script. ([1119351](https://issuetracker.unity3d.com/issues/unity-crashes-when-a-material-that-is-highlighted-in-the-project-window-is-overwritten-from-a-script))
    
*   Audio: Fixed an issue with AudioClip Get/SetData when the provided offset/length requires wrapping around the end of the clip. ([844064](https://issuetracker.unity3d.com/issues/audioclip-dot-getdata-returns-samples-that-are-missing-parts-of-the-original-clip-when-wrap-around-is-needed), 1162046)
    
*   Audio: Removed "raw speaker mode" option from Project Settings for audio, as it was never usable and made the matching enum value obsolete. ([1062387](https://issuetracker.unity3d.com/issues/unified-player-settings-on-changing-the-audio-default-speaker-mode-to-raw-it-sets-as-mono))
    
*   Build Pipeline: Fix Unity allows to build project via script with not compatible color space and graphics API. ([1076664](https://issuetracker.unity3d.com/issues/unity-allows-to-build-project-via-script-with-not-compatible-color-space-and-graphics-api))
    
*   Build Pipeline: Fixed an issue where BuildPipeline.BuildAssetBundles was not releasing memory frequently enough leading to a out of memory crash
    
*   Build Pipeline: Fixed an issue where sprite atlas Sprites were included in the bundle multiple times. ([1121868](https://issuetracker.unity3d.com/issues/android-same-atlas-assets-are-being-included-in-asset-bundle-multiple-times-when-bundle-is-built))
    
*   Build Pipeline: Fixed SBP out of memory crash. ([1158643](https://issuetracker.unity3d.com/issues/building-asset-bundles-with-sbp-may-get-oom-crash), 1160712)
    
*   Build Pipeline: Fixed sprite sheets in asset bundles built by scriptable build pipeline crash on access. ([1146568](https://issuetracker.unity3d.com/issues/sprite-sheets-in-asset-bundles-built-by-scriptable-build-pipeline-crash-on-access), 1167257)
    
*   Build Pipeline: Made Unity include the splash screen background textures even when the splash screen is disabled, so that the scripting API can draw the splash screen. ([1114547](https://issuetracker.unity3d.com/issues/splash-screen-background-is-not-included-when-drawing-with-scripting-api-and-splashscreen-is-disabled-in-player-settings))
    
*   Deployment Management: Fixed an issue with throwing BuildFailedException from a build callback not failing the build. ([1097286](https://issuetracker.unity3d.com/issues/build-does-not-fail-when-using-buildfailedexception), 1159243)
    
*   DX12: Fix for DX12 heap alignment (1160388, 1162983)
    
*   DX12: Fixed exclusive fullscreen always reverting to windowed fullscreen.
    
*   DX12: Make sure we draw the light probe visualization only if we are inside a frame. ([1158553](https://issuetracker.unity3d.com/issues/dx12-selecting-a-light-probe-group-game-object-in-directx12-mode-crashes-the-editor-at-d3d12scratchbuffer-d3d12scratchbuffer), 1166716)
    
*   Editor: Added an error message to `EditorGUI.EndChangeCheck` when the stack is empty.
    
*   Editor: Added Material checkout support in the Game Object Inspector. (962080)
    
*   Editor: Added support for a new toolbox format for Rider.
    
*   Editor: Added support for menu trees in EditorTool context menu.
    
*   Editor: Assume calls in UnityTest are now treated as an inconclusive result. (1075663)
    
*   Editor: Checkbox buttons now toggle correctly when users press the **Space** shortcut key. ([1136216](https://issuetracker.unity3d.com/issues/imgui-checkboxes-dont-toggle-when-keyboard-shortcut-space-is-pressed))
    
*   Editor: Creating a material while multiple inspector windows are open no longer triggers `IndexOutOfRange` errors. ([1122847](https://issuetracker.unity3d.com/issues/clicking-on-audio-listener-component-in-inspector-toggles-some-empty-space))
    
*   Editor: Deleting a Preset Asset in ADB2 no longer causes an error. ([1157112](https://issuetracker.unity3d.com/issues/presets-deleting-a-single-preset-from-the-project-generates-an-error-in-the-console), 1159888)
    
*   Editor: Fix an issue where Panels displayed in the Scene view blocked user input across the width of the viewport. ([1147144](https://issuetracker.unity3d.com/issues/panels-displayed-in-scene-view-block-user-input-across-the-width-of-the-viewport), 1161722)
    
*   Editor: Fix Batchmode build hanging in PackageManager::RunRequestSynchronously. ([1137073](https://issuetracker.unity3d.com/issues/osx-batchmode-build-hangs-at-refresh-detecting-if-any-assets-need-to-be-imported-or-removed), 1154317)
    
*   Editor: Fix the issue with NullReferenceException when previewing assets on Unity Package import ([1148966](https://issuetracker.unity3d.com/issues/custom-package-preview-window-goes-gray-when-clicking-on-image-files), 1159897)
    
*   Editor: Fixed an issue where gamepad input was not detected when 3 Xbox controllers were connected. ([1127453](https://issuetracker.unity3d.com/issues/input-xbox-controller-input-not-detected))
    
*   Editor: Fixed a crash that occurred when entering or exiting Play mode with certain AssetImporters displayed in the Inspector. (1141570, 1144208)
    
*   Editor: Fixed a crash that sometimes occurred if a sprite that was being drawn was deleted or modified while the splash screen was playing. The splash screen is now cancelled when an asset is modified or deleted. ([857060](https://issuetracker.unity3d.com/issues/splash-image-changing-logo-shown-while-splash-screen-is-on-preview-crashes-the-editor))
    
*   Editor: Fixed a delay when dragging the end cap of an edge in GraphView.
    
*   Editor: Fixed a holdover of the alt modifier in the Editor when gaining focus for Linux editor from alt+tab (1104979)
    
*   Editor: Fixed a NullReferenceException that occurred when changing the order of a reorderable list.
    
*   Editor: Fixed an Editor crash that occurred when switching to DirectX 12. ([1127388](https://issuetracker.unity3d.com/issues/directx-12-editor-crashes-on-switching-windows-graphics-apis-to-direct3d12))
    
*   Editor: Fixed an error that occurred when closing a detached Material preview window belonging to a "second" instance of an Inspector window. (1119612)
    
*   Editor: Fixed an exception that occurred when expanding the Mesh Renderer's Shader section in the Tree Inspector. ([1145010](https://issuetracker.unity3d.com/issues/inspector-exception-when-expanding-the-mesh-renderers-shader-section-in-the-tree-inspector), 1145056)
    
*   Editor: Fixed an issue in Unity Test Runner where tests timed out early when using large Timescale values. ([1098090](https://issuetracker.unity3d.com/issues/playmode-tests-timeout-when-time-dot-timescale-is-large))
    
*   Editor: Fixed an issue where **PropertyAttribute** was not applied on arrays. ([1140241](https://issuetracker.unity3d.com/issues/propertyattribute-has-no-effect-on-items-in-an-array))
    
*   Editor: Fixed an issue where **Shift + Del** did not remove empty elements from arrays in the Inspector window. ([1105084](https://issuetracker.unity3d.com/issues/shift-plus-delete-does-not-remove-an-empty-element-from-the-array-in-the-inspector-window))
    
*   Editor: Fixed an issue where clicking an AudioListener Component in the Inspector window caused empty space to appear. ([1122847](https://issuetracker.unity3d.com/issues/clicking-on-audio-listener-component-in-inspector-toggles-some-empty-space))
    
*   Editor: Fixed an issue where compliation failures caused Play mode tint to affect parts of the Editor after exiting Play mode. ([1130997](https://issuetracker.unity3d.com/issues/color-of-the-editor-changes-as-if-it-was-play-mode-when-trying-to-enter-play-mode-before-scripts-are-compiled))
    
*   Editor: Fixed an issue where Console windows disappear when the Unity Editor does not have focus. ([1109182](https://issuetracker.unity3d.com/issues/console-windows-disappear-when-unity-editor-is-not-in-focus))
    
*   Editor: Fixed an issue where Editor layouts with undocked windows were saved/loaded incorrectly. ([1122565](https://issuetracker.unity3d.com/issues/editor-windows-layout-is-being-saved-slash-loaded-incorrectly-when-saving-undocked-or-maximized-tabs))
    
*   Editor: Fixed an issue where Editor windows responded to mouse events outside their window areas. ([1143721](https://issuetracker.unity3d.com/issues/editor-windows-respond-to-mouse-events-outside-the-window), 1144224)
    
*   Editor: Fixed an issue where invoking `ShowObjectPicker` right after closing another ObjectPicker freezes the Editor. ([1113046](https://issuetracker.unity3d.com/issues/showobjectpicker-freezes-editor-when-its-invoked-right-after-another-objectpicker-is-closed))
    
*   Editor: Fixed an issue where relaunching the Editor after changing graphics settings returned the user to the Hub rather than the Editor. ([1134314](https://issuetracker.unity3d.com/issues/hub-editor-doesnt-restart-instead-hub-opens-up-on-selecting-restart-editor-from-popup-when-changing-graphics-apis), 1161970)
    
*   Editor: Fixed an issue where the **Reset** option in the Inspector context menu cleared the **Name** property for MonoBehaviour assets. ([1092051](https://issuetracker.unity3d.com/issues/using-the-reset-context-menu-option-on-a-scriptable-object-clears-its-name-property-in-the-inspector-window))
    
*   Editor: Fixed an issue where the **Transform** fields in the AvatarMask Inspector don't show all of a skeleton's transforms. ([1123656](https://issuetracker.unity3d.com/issues/avatarmask-inspector-transforms-field-doesnt-show-all-transforms-from-the-skeleton), 1152129)
    
*   Editor: Fixed an issue where the Camera preview had a fixed size when the Scene view tools panel was displayed. ([1125006](https://issuetracker.unity3d.com/issues/camera-preview-has-minimum-width-and-does-not-shrink-when-tools-popup-in-scene-view-is-present))
    
*   Editor: Fixed an issue where the Edit button became stuck in its enabled state. ([1120360](https://issuetracker.unity3d.com/issues/imgui-edit-button-in-components-stays-activated-even-on-disabling-it))
    
*   Editor: Fixed an issue where the Editor window "cropped" render textures. ([1127773](https://issuetracker.unity3d.com/issues/postprocessing-depth-of-field-is-not-applied-to-the-whole-screen-when-resolution-is-fixed-and-is-resized))
    
*   Editor: Fixed an issue where the Splash Screen Unity logo did not fit inside the **Logos** list in the Player section of the Project Settings window. ([976154](https://issuetracker.unity3d.com/issues/editor-splashscreen-logo-is-too-big-in-playersettings-editor))
    
*   Editor: Fixed an issue where the `FilePathAttribute` constructor threw an exception if called from a `MonoBehaviour` constructor or another thread. ([1077857](https://issuetracker.unity3d.com/issues/filepathattribute-class-calls-an-api-method-get-unitypreferencesfolder-from-its-constructor-resulting-in-an-exception-error))
    
*   Editor: Fixed an issue where unassigning a shortcut in the Shortcuts Manager did not update the command entry in the main menu. ([1109108](https://issuetracker.unity3d.com/issues/shortcut-label-is-still-being-displayed-when-adding-and-removing-a-shortcut-for-the-command))
    
*   Editor: Fixed an issue where uniformly scaling a zero-sized PrimitiveBoundsHandle using the **Shift** modifier caused the center point to drift. Uniform scaling now applies to all axes if the bounding volume had zero size at the time the control handle was clicked. ([1021975](https://issuetracker.unity3d.com/issues/physics-capsule-collider-center-drifts-away-while-dragging-by-holding-shift-key), 1152362)
    
*   Editor: Fixed an issue with "Assembly has duplicate references" errors not listing the duplicate references correctly. (1132593, 1148355)
    
*   Editor: Fixed an issue with "Multiple precompiled assemblies with the same name" errors not listing the paths of the precompiled assemblies. ([1138754](https://issuetracker.unity3d.com/issues/precompiledassemblyexception-does-not-show-file-paths-in-its-message-when-there-are-few-assemblies-with-the-same-name), 1148356)
    
*   Editor: Fixed an issue with **Use GUIDs** being enabled in the Assembly Definition File inspector when GUID references are not used. ([1140806](https://issuetracker.unity3d.com/issues/assembly-definition-useguids-property-gets-enabled-when-changes-are-applied), 1148354)
    
*   Editor: Fixed an issue with C# solutions not getting regenerated when changing the **Allow 'unsafe' code** Project setting. ([1105512](https://issuetracker.unity3d.com/issues/visual-studio-continues-to-warn-about-unsafe-code-when-unsafe-code-is-enabled-in-project-settings), 1148358)
    
*   Editor: Fixed an issue with jittery scrolling through large serialized lists in the Inspector. ([1131250](https://issuetracker.unity3d.com/issues/inspector-is-stuttering-when-scrolling-through-the-large-serializable-list-on-the-scriptable-object-in-the-inspector))
    
*   Editor: Fixed an issue with orphan host views that occurred while loading an Editor window layout. ([1079742](https://issuetracker.unity3d.com/issues/console-throws-failed-to-destroy-views-number-1-hostview-error-when-changing-layout))
    
*   Editor: Fixed an issue with `CompilationPipeline.GetAssemblies(AssemblyType.Player)` not returning test assemblies. (1137205, 1148357)
    
*   Editor: Fixed assertion message 's2 != NULL' in log files.
    
*   Editor: Fixed display of blendshapes count when count is 1 in model preview. ([1162436](https://issuetracker.unity3d.com/issues/a-model-with-1-blendshape-does-not-show-blendshapes-count-info-in-previewgui), 1166909)
    
*   Editor: Fixed incorrect asset icon being shown for assemblies.
    
*   Editor: Fixed resize borders on floating windows to better expose window controls. This also fixes an issue where dragging from other parts of the window triggered resizing. (1116567)
    
*   Editor: Fixed security vulnerability UNITY-SEC-2144.
    
*   Editor: Fixed splitter view layout and resizing rounding issues. ([1099360](https://issuetracker.unity3d.com/issues/editor-windows-layout-is-being-saved-slash-loaded-incorrectly-when-saving-undocked-tabs))
    
*   Editor: Fixed the misalignment by reverting the fadegroup functionality. ([1111065](https://issuetracker.unity3d.com/issues/video-aspect-ratio-drop-down-appears-misaligned-on-changing-the-original-dimensions-of-the-video), 1158313)
    
*   Editor: Fixed the position of the drag area of the preview resizer depending on whether the target preview is in an img container. ([1154694](https://issuetracker.unity3d.com/issues/resizing-the-preview-in-the-asset-explorer-window-causes-the-wrong-mouse-icon-to-be-used), 1160640)
    
*   Editor: Fixed the Preview pane in the Object Selector.
    
*   Editor: Fixed VU meter display on custom audio filter behaviours with custom Editors. ([1117744](https://issuetracker.unity3d.com/issues/onaudiofilterread-meter-disappears-when-using-a-custom-editor), 1162045)
    
*   Editor: Made the "Add Component" popup window receive focus in Linux editor. (1098140)
    
*   Editor: Maximizing an Editor window after resizing it by dragging from the top bar now works correctly. ([1126516](https://issuetracker.unity3d.com/issues/editor-windows-dont-change-the-restoredown-to-maximize-when-pulled-from-the-top-bar))
    
*   Editor: One column layout drop fix ([1150509](https://issuetracker.unity3d.com/issues/editor-files-are-not-being-added-to-assets-folder-if-dragged-and-dropped-in-empty-space-below-the-package-manager-folder), 1158294)
    
*   Editor: Renamed MeshRenderer Priority in the Editor to match the documentation.
    
*   Editor: Renamed the "Logging" preference in "Stack Trace" to avoid confusion. ([1118914](https://issuetracker.unity3d.com/issues/turning-off-logging-still-shows-log-messages-and-disables-double-clicking-them))
    
*   Editor: Renamed the UI Transparency Priority to Renderer Priority in MeshRenderer component.
    
*   Editor: Unity native DefaultImporter is now excluded from Presets. ([1129083](https://issuetracker.unity3d.com/issues/presets-defaultinpector-type-needs-to-be-blacklisted))
    
*   Editor: Updated the Windows splash screen.
    
*   Editor: `CustomPropertyDrawer`s of array elements inside another array now now work correctly on each element. ([1156837](https://issuetracker.unity3d.com/issues/custompropertydrawers-have-different-behavior-now-in-2019-dot-2), 1158011)
    
*   GI: Fixed a crash that occured when you recompiled Shaders, both manually or when you switched render pipelines.
    
*   GI: Fixed a crash with baking global illumination when HideFlags was configured on objects. (1129038)
    
*   GI: Fixed an intermediate lookup issue in Enlighten when using SSDs with Realtime GI and Baked GI enabled ([1128583](https://issuetracker.unity3d.com/issues/realtime-gi-editor-throws-failed-opening-gi-file-errors-when-switching-ambient-modes), [1134676](https://issuetracker.unity3d.com/issues/realtime-gi-editor-throws-failed-opening-gi-file-at-relative-path-errors-when-switching-lighting-backends), [1134702](https://issuetracker.unity3d.com/issues/ui-ssds-do-not-contribute-to-realtime-lightmaps-even-when-contribute-gi-flag-is-enabled), 1143679, 1143686, 1143687)
    
*   GI: Fixed an issue where Light Probes had corrupted gizmos when there was 1 static object in the Scene. ([1123892](https://issuetracker.unity3d.com/issues/light-probe-gizmos-are-corrupted-after-upgrading-the-project))
    
*   GI: Fixed an issue where push off parameter in Lightmap Parameters asset was ignored when baking lightmaps. ([1117680](https://issuetracker.unity3d.com/issues/pushoff-slider-in-lightmap-parameters-asset-has-no-effect))
    
*   GI: Fixed an issue where selecting Probe groups would make the Editor crash on Metal (macOS). ([1123971](https://issuetracker.unity3d.com/issues/osx-editor-crashes-after-selecting-light-probe-group-gameobject-in-the-hierarchy))
    
*   GI: Fixed broken bake in Editor with additive loaded scenes. ([1138556](https://issuetracker.unity3d.com/issues/editor-freezes-in-an-infinite-loop-with-integrate-failed-on-write-lighting-job-error-when-baking-gi), 1167604)
    
*   GI: Fixed case of missing lighting when baking with GPU lightmapper. ([1121705](https://issuetracker.unity3d.com/issues/gpu-plm-scene-is-black-after-baking-lighting-with-the-gpu-lightmapper))
    
*   GI: Fixed error related to cached G buffer data "Failed reading from a9/a9af123a12f31.ghd" when using the progressive lightmapper while having data from older versions in the GI cache.
    
*   GI: Fixed hashing issue when writing out AO textures for PLM.
    
*   GI: Fixed the GPU Lightmapper so it gives stable results when changing compositing parameters, sample counts, or the number of bounces. (1111135)
    
*   GI: Fixed the Lighting Explorer so that it saves the column settings when you restart the Editor. ([1131422](https://issuetracker.unity3d.com/issues/light-explorer-does-not-remember-column-states-between-sessions))
    
*   GI: GI - Fix player crashes on Application.Quit() in Debug builds when using real-time GI (1158498) (1158498, 1160124)
    
*   GI: GPU lightmapper: Ensure OpenCL kernel are recompiled on Nvidia even when only the include files changes.
    
*   GI: GPU lightmapper: Fix crash on application exit when GPU lightmapper openCL context is lost.
    
*   GI: GPU lightmapper: Fixed a crash caused by running out of GPU memory when allocating the BVH (acceleration structure for ray tracing). This could happen when baking a terrain with a high heightmap resolution.
    
*   GI: GPU lightmapper: Make render jobs resilient to not yet prepared materials. This fix a crash when GPU lightmapper fallback to CPU. ([1133816](https://issuetracker.unity3d.com/issues/gpu-plm-editor-crashes-in-radeonraysmeshmanager-storeperinstancematerialandtransmissiondata-when-baking-the-archviz-project), 1149276)
    
*   GI: Renamed "Auto Bake On/Off" to "Auto Generate Lighting On/Off" in the app bar.
    
*   GI: Use AI denoising for shadow mask and direct environment samples when baking with the GPU lightmapper. ([1138839](https://issuetracker.unity3d.com/issues/gpu-plm-ai-denoisers-do-not-denoise-shadowmask), 1144432)
    
*   Graphics: Delay in bursts no longer works. ([1154292](https://issuetracker.unity3d.com/issues/spawner-delay-in-bursts-no-longer-works), 1156374)
    
*   Graphics: Enabled GPU skinning for BlendShapes on Metal.
    
*   Graphics: Fix CommandBuffer.SetShadowSamplingMode code typo. (1143760, 1158287)
    
*   Graphics: Fix Reflection Probes baking when R11G11B10 HDR mode is used in Graphics Settings. ([1115040](https://issuetracker.unity3d.com/issues/reflection-probe-gozmos-are-distorted-when-selected-in-the-scene-and-android-platform-is-selected), 1169640)
    
*   Graphics: Fixed a crash caused by Unknown LightMode in a ShaderLab Shader. ([1132088](https://issuetracker.unity3d.com/issues/shaderlab-shader-is-causing-unity-to-crash-when-closing-the-editor-or-upgrading-the-project-to-newer-version))
    
*   Graphics: Fixed a crash on GPU skinning when blend shapes had zero vertices. ([1121794](https://issuetracker.unity3d.com/issues/crash-slash-freeze-on-skinnedmeshrender-when-gpu-skinning-is-enabled))
    
*   Graphics: Fixed a crash that happened when updating mesh data from script when using Vulkan and graphics jobs. (1090932)
    
*   Graphics: Fixed an infinite console error loop when the user tried to assign a 2D texture in the Cubemap field of a Custom Reflection Probe. ([1156727](https://issuetracker.unity3d.com/issues/lighting-assigning-2d-texture-to-cubemap-property-of-reflection-probe-throws-error), 1156969)
    
*   Graphics: Fixed an issue where shadow quality settings were hidden when using an SRP, which meant that culling sometimes didn't include shadow casters.
    
*   Graphics: Fixed an issue where the Game view did not fully update streaming mips while in Edit mode. ([1141222](https://issuetracker.unity3d.com/issues/game-view-texture-mip-levels-are-loaded-based-on-the-scene-view-camera-when-the-showtexturestreamingsummary-script-has-been-run), 1145166)
    
*   Graphics: Fixed an issue where visual flickering happened when Mesh data was edited from a script while graphics jobs were in use in Vulkan. ([1075277](https://issuetracker.unity3d.com/issues/dx12-dynamic-mesh-corruption-with-native-graphics-jobs-flickering-and-disapearing-meshes))
    
*   Graphics: Fixed an issue with non-readable mesh where indices were kept in memory when loading from built data ([1126675](https://issuetracker.unity3d.com/issues/mesh-memory-usage-increase-from-2018-dot-2-to-2018-dot-3-and-forward))
    
*   Graphics: Fixed an issue with skinned mesh where vertex compression was disabled for all components. ([1118278](https://issuetracker.unity3d.com/issues/vertex-compression-is-completely-disabled-on-platforms-with-compressedgpuskinningdisabled))
    
*   Graphics: Fixed bad alignment of render surface resource heaps ([1155163](https://issuetracker.unity3d.com/issues/d3d12immediatecontext-bindtexture-crash-when-opening-a-scene-with-directx3d12), 1156592)
    
*   Graphics: Fixed cases where overlapping cross-fade objects sometimes appeared as opaque. ([916831](https://issuetracker.unity3d.com/issues/lod-blinking-artifact-at-speedtree-cross-fade-animation-when-several-tree-billboards-overlap))
    
*   Graphics: Fixed dynamic resolution when using Vulkan. ([1148341](https://issuetracker.unity3d.com/issues/android-player-crashes-on-changing-resolution-dynamically), 1148390)
    
*   Graphics: Fixed issue where Vulkan implementation of Texture2D.SetPixels may pipeline stall. ([1141239](https://issuetracker.unity3d.com/issues/vulkan-inefficient-memory-barriers-vkcmdcopybuffertoimage), 1145494)
    
*   Graphics: Fixed missing caps in the Pixels32 APIs. (1129776)
    
*   Graphics: Fixed missing IsEACFormat and IsXRFormat APIs. (1129777)
    
*   Graphics: Fixed RenderTextureFormat BGRA support. (1141798, 1144325)
    
*   Graphics: Fixed the app bar so it shows "Compiling shader 'x'" instead of just the Shader name.
    
*   Graphics: Fixed: Instancing batcher would crash hard on Vulkan if attempting to draw without an active GPU program.
    
*   Graphics: Made changes to correctly display a preview image of the Billboard Renderer in the Project Window and LODGroup preview panel. ([769753](https://issuetracker.unity3d.com/issues/speedtree-lod-inspector-lod-renderer-preview-is-not-displayed-for-spm-model))
    
*   Graphics: Made create texture occur on a thread in cases where async loads to update an existing texture.
    
*   Graphics: Made normal maps acknowledge the \[Normal\] attribute in shader when Unity checks that they have "Normal Map" texture usage. (1132148)
    
*   Graphics: Made Textures unsupported by mip map streaming such as reflection probes and decals now load highest mip. ([1115306](https://issuetracker.unity3d.com/issues/reflection-probes-have-low-resolution-textures-when-building-with-texture-streaming-enabled-and-and-default-compression-mode), 1145164)
    
*   Graphics: Metal: Artifacts appear when using Dynamic Resolution with MSAA ([1111105](https://issuetracker.unity3d.com/issues/os-x-artifacts-appear-when-using-dynamic-resolution-with-msaa))
    
*   Graphics: Removed 4G limit on texture mip streaming budget. ([1147394](https://issuetracker.unity3d.com/issues/qualitysettings-dot-streamingmipmapsmemorybudget-is-always-clamped-down-to-4096-mb-even-on-64-bit-systems), 1150741)
    
*   Graphics: Terrain alphamaps now ignore QualitySettings master texture limit ([1148582](https://issuetracker.unity3d.com/issues/painting-texture-on-the-terrain-does-not-work-slash-crash-the-editor-when-projects-texture-quality-setting-is-not-set-to-full-res), 1154326)
    
*   Graphics: Unity crashes when a VFX is playing and the VFX project settings are reset. ([1154099](https://issuetracker.unity3d.com/issues/project-settings-unity-crashes-when-a-vfx-is-playing-and-the-vfx-project-settings-are-reset), 1154781)
    
*   Graphics: unity\_LightIndices\[1\] are identical to every object and are set per frame ([1155879](https://issuetracker.unity3d.com/issues/srp-unity-lightindices-1-are-identical-to-every-object-and-are-set-per-frame), 1166706)
    
*   Graphics: VFX : Enable/Disable doesn't restart effect. (1133474, 1152230)
    
*   Graphics: Vulkan: Fixed a crash that occcured when setting rendertexture sampler properties before creating the actual texture. (1115165)
    
*   Graphics: Vulkan: Fixed an issue that caused an error message to repeatedly occur when attempting to draw with missing bindings.
    
*   Graphics: Vulkan: Fixed crash when rendering reflection probes on Android. (1108968)
    
*   Graphics: Vulkan: Fixed crash when using MSAA.
    
*   IL2CPP: Fixed a crash on background threads when a managed exception occured while the process was shutting down.
    
*   IL2CPP: Fixed a crash when many threadpool threads or sockets were in use. (1129409, 1168721)
    
*   IL2CPP: Fixed a performance issue with lumped builds.
    
*   IL2CPP: Made generated code marshal an array of primitive types as `SAFEARRAY` by default if it's used as a field. ([1131557](https://issuetracker.unity3d.com/issues/the-generated-il2cpp-code-no-longer-marshals-a-struct-to-its-native-representation-before-passing-it-to-a-native-function), 1146301)
    
*   IL2CPP: Throw a managed exception at runtime when a generic type is marshaled as a delegate parameter. (1122074)
    
*   Input: Fixed a crash that happened with non-ASCII key mapping when trying to map a key which does not produce characters for single key presses (e.g. Japanese).
    
*   Input: Made scrolling delta on Mac work with older mice
    
*   Internal: Fixed `BatchRendererGroup` group removal.
    
*   iOS: 'UIApplicationExitsOnSuspend' will no longer be included in the Xcode project's info.plist file because it was made obsolete by Apple. ([1160614](https://issuetracker.unity3d.com/issues/ios-apps-with-uiapplicationexitsonsuspend-in-info-dot-plist-failing-to-pass-apple-store-validation), 1165520)
    
*   iOS: Added missing iOS devices to the device list used by the editor for profiler, Unity Remote, etc. ([1111598](https://issuetracker.unity3d.com/issues/ios-unity-remote-doesnt-work-with-new-ios-devices-shows-unknown-dot-in-the-project-settings-device-name-dropdown-menu))
    
*   iOS: Added missing RG16 texture format for Metal.
    
*   iOS: Fixed an issue that caused keyboard type to sometimes not change when switching controls. ([1154527](https://issuetracker.unity3d.com/issues/ios-when-int-input-fields-keyboard-is-opened-focusing-other-input-fields-doesnt-open-corresponding-keyboards), 1165455)
    
*   iOS: Fixed an issue where the Xcode framework search paths setting was overridden when appending an Xcode project. ([703217](https://issuetracker.unity3d.com/issues/ios-framework-search-paths-are-overriden-using-append))
    
*   iOS: Fixed build failure when Xcode `DerivedData` path was set relative to the project. (1117371)
    
*   iOS: Fixed identification of iPad 6th (it used to be identified as iPadPro10Inch2Genor or iPadUnknown with iOS.Device.generation) ([1065983](https://issuetracker.unity3d.com/issues/ios-ipad-6th-generation-is-identified-as-ipadpro10inch2genor-or-ipadunknown-with-ios-dot-device-dot-generation))
    
*   iOS: Fixed problem where Audio was "jumpy" on some iOS devices, skipping a few frames every few seconds ([1124966](https://issuetracker.unity3d.com/issues/ios-audio-is-jumpy-on-some-ios-devices-skipping-a-few-frames-every-few-seconds))
    
*   iOS: Fixed Screen.autorotateTo causing missing call to UnityOrientationRequestWasCommitted, effectively resulting in running some code every frame from now on erroneously. ([1122902](https://issuetracker.unity3d.com/issues/ios-setting-screen-dot-autorotatetolandscapex-causes-the-next-attempt-to-open-safari-to-immediately-return-to-unity-silently))
    
*   iOS: Fixed UIApplicationExitsOnSuspend is deprecated in iOS 13 ([1160614](https://issuetracker.unity3d.com/issues/ios-apps-with-uiapplicationexitsonsuspend-in-info-dot-plist-failing-to-pass-apple-store-validation), 1165520)
    
*   iOS: `Screen.currentResolution.refreshRate` now correctly returns the actual refresh rate instead of returning 30 in all situations. (1117877)
    
*   Kernel: Fixed a crash when resizing an array through `SerialziedProperty`. ([1123752](https://issuetracker.unity3d.com/issues/editor-crashes-on-selecting-a-texture-preset-with-different-settings))
    
*   Linux: Fixed an issue that caused submenus to lose focus and close prematurely. ([1142911](https://issuetracker.unity3d.com/issues/linux-sprite-editor-slice-window-disappears-when-trying-to-change-slicing-type), 1144233)
    
*   Linux: Fixed an issue that caused the Editor to overwrite the PlayerPrefs file at launch. ([1072116](https://issuetracker.unity3d.com/issues/linux-editor-overwrites-playerprefs-file-when-launched))
    
*   Linux: Fixed an issue where the Editor crashed when started from the Hub ([1140369](https://issuetracker.unity3d.com/issues/linux-editor-hangs-on-launch-when-running-through-unity-hub), 1154319)
    
*   Linux: Fixed non-printable characters being allowed in GUI text objects in the Linux Editor. ([1126208](https://issuetracker.unity3d.com/issues/linux-empty-characters-are-created-in-text-fields-when-using-ctrl-shortcuts))
    
*   Linux: Linux Editor no longer fails to delete assets on partitions or network drives that do not contain trash directories. ([1062162](https://issuetracker.unity3d.com/issues/you-cannot-delete-assets-on-a-network-drive-in-linux))
    
*   Linux: Nvidia drivers are now forced to turn off vsync on Linux. (1109048, 1146524)
    
*   Linux: Pausing the Linux editor while playing with cursor lock mode set to locked or confined will now free the cursor. (1132336)
    
*   Linux: Vuforia link is now hidden in the Linux Editor for Linux. ([1144110](https://issuetracker.unity3d.com/issues/linux-player-settings-link-to-download-vufora-sdk-fails-due-to-permission-rights), 1157123)
    
*   Lumin: Fixed error preventing running playmode tests on a Lumin device.
    
*   Lumin: Re-added package signing support for MagicLeap packages.
    
*   macOS: Fixed an issue that caused the built game icon to appear distorted. ([1152484](https://issuetracker.unity3d.com/issues/osx-default-icon-for-mac-standalone-is-distorted), 1158746)
    
*   macOS: Fixed excessive fencing causing all GPU workload to be serialized.
    
*   macOS: Fixed incorrect Input.keyCode value when keyboard layout changes on macOS.
    
*   macOS: Fixed queued key events getting incorrect modifiers flags causing the wrong shortcut to be executed.
    
*   Multiplayer: Fixed an error with the NetworkManagerHUD when clicking Lan Client on WebGL build ([860733](https://issuetracker.unity3d.com/issues/networkmanagerhud-uncaught-typeerror-cannot-read-property-id-of-null-thrown-when-clicking-lan-client-on-webgl-build))
    
*   Package Manager: A local package (using the `file:/` protocol) is no longer allowed to reference a sub folder inside "Assets", "Library" or "ProjectSettings".
    
*   Package Manager: Added error handling for when a user has an empty `package.json` file in their Project. ([1157243](https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-packages-package-dot-json-contains-incorrect-data-and-package-manager-window-is-open), 1163613)
    
*   Package Manager: Fix the issue where the up/down arrows cycle through the full list of packages during search ([1144663](https://issuetracker.unity3d.com/issues/package-manager-after-a-search-the-up-slash-down-arrows-cycle-through-the-full-list-of-packages), 1154427)
    
*   Package Manager: Fixed an error in the Package Manager UI when the OS uses a language other than English.
    
*   Package Manager: Fixed an issue where a Git dependency resolved to the locked hash even after removing the commitish part of a Git URL.
    
*   Package Manager: Fixed an issue where cloning a Git repository could wait indefinitely for user input if credentials for that repository were not configured.
    
*   Package Manager: Fixed an issue where the cancel icon (x) on the Search box in the Package Manager UI disappears when installing or removing a package. ([1152444](https://issuetracker.unity3d.com/issues/package-manager-search-cross-icon-disappears-on-installing-or-removing-a-package), 1156832)
    
*   Package Manager: Fixed an issue where the status icons got corrupted whenever a user exits search mode. (1142542, 1144549)
    
*   Package Manager: Fixed an issue with hidden elements erroneously appearing in the UI. ([1139170](https://issuetracker.unity3d.com/issues/unnecessary-ui-icons-are-drawn-at-the-top-left-of-the-package-manager-window-when-certain-package-search-strings-are-entered))
    
*   Package Manager: Fixed incorrect error messages in the Package Manager UI while disabling the Built-in package. ([1131602](https://issuetracker.unity3d.com/issues/packman-ui-disabling-modules-error-message-is-inaccurate), 1145317)
    
*   Particles: Added fade and soft particle properties to the Emissive color of the Standard Particle Shaders.
    
*   Particles: Fixed ETC transparency on particles (1144935, 1150180)
    
*   Particles: Fixed ParticleSystem prewarm not locating WindZones, ForceFields and Colliders during Awake. ([1122824](https://issuetracker.unity3d.com/issues/wind-zone-effect-is-not-prewarped-on-a-particle-system-after-reopening-the-project), 1164545)
    
*   Particles: Fixed stuttering when using scripted simulation to request long simulation times. ([753940](https://issuetracker.unity3d.com/issues/particle-system-simulate-issues), 1144335)
    
*   Particles: Opening a legacy Prefab with a ParticleSystem in Prefab Mode: ParticleSystemRenderer component is now correctly hidden in the Inspector.
    
*   Phyics2D: The implicitly created static ground-body is now not shown in the static body count in the profiler 2D physics area. ([1143465](https://issuetracker.unity3d.com/issues/profiler-shows-1-static-body-under-physics-2d-when-profiling-an-empty-scene), 1148737)
    
*   Physics: Fix issue with bounds in SkinnedMeshRenderer. ([879696](https://issuetracker.unity3d.com/issues/adding-cloth-component-to-skinnedmeshrenderer-changes-bounds), 1153181)
    
*   Player: Fixed the order of event timestamps on windows. (1132707)
    
*   Player: Fixes CoreStats to only send Ads id if Ads service is enabled. (1120830, 1154339)
    
*   Player: New Input System: Fix potential deadlock when adding new devices.
    
*   Player: New Input System: Make Input Debugger work in edit mode.
    
*   Player: PlayerConnection API now works correctly when reconnecting after disconnecting.
    
*   Prefabs: Fix loosing selection of Prefab root in Prefab Mode after draggging script to Inspector.
    
*   Prefabs: Made imports batch when multi-selecting Prefab instances and clicking Apply All.
    
*   Prefabs: PrefabMode: For broken prefabs use the root that the PrefabImporter has chosen when opening the prefab file in Prefab Mode, other dangling roots are deleted.
    
*   Prefabs: Reflection CubeMap for default reflection in Prefab Mode has been replaced with a lower resolution and without a sun (which caused multiple highlights)
    
*   Profiler: Fix \[Profiler\] "Requested frame does not exists" exception thrown on clearing data while looking at UI Module ([1160622](https://issuetracker.unity3d.com/issues/profiler-requested-frame-does-not-exists-exception-thrown-on-clearing-data), 1164595)
    
*   Scene Management: Fix reverting object override not working on Prefab instance inside Prefab Asset and throwing errors. ([1146441](https://issuetracker.unity3d.com/issues/cannot-revert-changes-to-prefab-variants-when-the-prefab-variant-is-edited-via-project-view), 1153391)
    
*   Scene Management: Prevent removing or altering components on immutable Prefab Assets via component context menu. (1129842, 1153396)
    
*   SceneManager: MergeTwoScenes test has occasional instability (1150769, 1160351)
    
*   Scripting: Fixed a crash when large array initializer is used. ([1148592](https://issuetracker.unity3d.com/issues/windows-editor-crashes-with-a-stackoverflowexception-if-a-script-references-a-large-array), 1160548)
    
*   Scripting: Fixed an error where assertion failed on expression: '!m\_CoroutineEnumeratorGCHandle.HasTarget()' is thrown when GC is collected ([1094391](https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-m-coroutineenumeratorgchandle-dot-hastarget-is-thrown-when-running-tests-in-test-runner))
    
*   Scripting: Fixed an issue when running the Editor with old scripting runtime if incremental GC is enabled in Project Settings. ([1119216](https://issuetracker.unity3d.com/issues/incremental-gc-projects-fails-to-open-if-switching-from-net-4-dot-x-to-net-3-dot-5-with-incremental-gc-enabled))
    
*   Scripting: Fixed an issue where constructors were called twice on ScriptableObjects with custom attributes when referencing the ScriptableObject instance. ([1113071](https://issuetracker.unity3d.com/issues/constructors-called-multiple-times-on-scriptableobjects-with-custom-attributes))
    
*   Scripting: Fixed an issue where user scripts could unload global game managers ([1114406](https://issuetracker.unity3d.com/issues/when-loading-up-the-project-fatal-error-unityeditor-dot-assetdatabase-loadassetatpath-is-being-thrown-out-and-unity-hangs))
    
*   Scripting: Fixed TargetInvocationException when using ML.NET. ([1109657](https://issuetracker.unity3d.com/issues/system-dot-reflection-dot-targetinvocationexception-is-thrown-when-using-net-machine-learning))
    
*   Scripting: Made useGUID enabled by default when the reference field is empty in the Assembly Definition Reference editor
    
*   Shaders: Fixed non-deterministic Shader binaries in Asset bundles. ([749340](https://issuetracker.unity3d.com/issues/static-batching-makes-the-assetbundles-built-with-the-same-scene-different-from-each-other))
    
*   Shaders: Fixed shader upgrader to not add exclude\_renderers due to const array usage. (1053734, 1143646)
    
*   Shaders: Minor HLSLcc fixes. (1105361, [1142484](https://issuetracker.unity3d.com/issues/two-shadercompilertests-hitting-asserts-on-reflection-callbacks), 1143647, 1143648)
    
*   Shadows/Light: Fix shadows culling when camera and frustum are almost perpendicular ([1150849](https://issuetracker.unity3d.com/issues/shadows-shadows-flicker-when-camera-is-moving), 1163791)
    
*   SpeedTree: Fixed the import of collision objects from SpeedTree v8 Assets.
    
*   Terrain: Fix TerrainLayer selection in Paint Texture Tool when the terrain layer assets are deleted. ([1113312](https://issuetracker.unity3d.com/issues/unable-to-remove-deleted-terrain-layers), 1164861)
    
*   Terrain: Fix the case that alpha map textures were lost during saving of newly created TerrainData. (1158454, 1164113)
    
*   Terrain: Made Terrain Tree brush paint across Terrain tiles ([1126622](https://issuetracker.unity3d.com/issues/terrain-trees-are-not-painted-on-neighbouring-terrain-when-painting-on-the-edge-of-terrain))
    
*   Terrain: Support for passing down per-layer attributes regarding mask maps and alpha channels ([1110520](https://issuetracker.unity3d.com/issues/terrain-lwrp-lod-popping-of-terrain-quad-nodes-with-instancing-enabled), 1159521)
    
*   Timeline: Clips will no longer randomly disappear when showing or hiding inline curves. (1141661, 1150620)
    
*   Timeline: Fixed an issue where dragging and dropping objects between tracks did not insert a new track correctly. ([1011381](https://issuetracker.unity3d.com/issues/timeline-misleading-track-insertion-when-dragging-objects-between-tracks-inside-a-track-group))
    
*   Timeline: Fixed an issue where the Track group background would disappear while scrolling. (876340)
    
*   Timeline: Fixed an issue with dragging and dropping objects on a Track group. (1014774)
    
*   Timeline: Fixed Disable the possibility to add Markers to tracks of a Timeline that is ReadOnly (1134463, 1146268)
    
*   Timeline: Fixed record button state not updating when offset modes are changed. ([1142747](https://issuetracker.unity3d.com/issues/timelines-animation-track-does-not-refresh-after-changing-track-offsets), 1150598)
    
*   Timeline: Going to Play Mode while inspecting a Track Asset will no longer throw exceptions. (1141958, 1150599)
    
*   Timeline: Reactions for Signals were not correctly drawn (1134422)
    
*   Timeline: The global/local time referential button will no longer be shown for a top-level timeline. (1080872, 1150607)
    
*   UI: Added support for copying uv2 and uv3 from the UIVertex AddVert overloaded API.
    
*   UI: An animation that updates items no longer dirties the Layout. This fixes some animation-related performance issues.
    
*   UI: Fixed an issue caused by deleting a drop-down list while it is open. ([1106263](https://issuetracker.unity3d.com/issues/deleting-a-dropdown-list-while-it-is-open-breaks-other-ui-objects))
    
*   UI: Fixed an issue where a null TransformHierarchy caused a crash when updating a RectTransform. ([1102234](https://issuetracker.unity3d.com/issues/crash-on-transform-gettransformaccess-when-building-list-of-referenced-assemblies-to-the-android), 1158048)
    
*   UI: Fixed an issue where assigning a togglegroup or changing **isOn** would not set the toggle as dirty. ([1141606](https://issuetracker.unity3d.com/issues/changing-the-group-field-on-a-toggle-component-doesnt-mark-the-scene-as-dirty), 1154185)
    
*   UI: Fixed an issue where enabling a Canvas and polling its RectTransform data in `Awake`/`Start` returned incorrect values for root RectTransforms.
    
*   UI: Fixed an issue where the Editor became unresponsive when the _GICache_ tab was open in the Project Preferences. ([1149001](https://issuetracker.unity3d.com/issues/editor-is-extremely-slow-and-almost-unresposive-when-the-gicache-tab-is-opened), 1152685)
    
*   UI: Fixed an issue where vertices generated for rich text tags led to very large vertex buffers.
    
*   UI: Fixed an issue with Canvas sort order being incorrect when Instantiating a GameObject with a Canvas
    
*   UI: Fixed compilation errors in `.asmdef` files that require a reference to the uGUI package. ([1154163](https://issuetracker.unity3d.com/issues/unityengine-dot-ui-reference-is-missing-in-assembly-definition-assemblies-and-plugins), 1154711)
    
*   UI: Fixed memory leak when rendering to a Camera with a disabled display. ([944603](https://issuetracker.unity3d.com/issues/memory-leak-if-only-one-display-device-is-connected-when-game-is-using-multiple-displays-and-networking))
    
*   UI: Fixed wording in **Advanced** Texture importing options for tiled sprites. ([1040453](https://issuetracker.unity3d.com/issues/tiled-sprites-imported-to-newer-versions-from-versions-5-dot-4-and-lower-throw-an-advanced-texture-error-that-cant-be-fixed))
    
*   UI: Fixing issue with IndexedSet not returning -1 when element is not found in dictionary.
    
*   UI: Made Assembly type check use TypeCache for better performance in Editor ([1099027](https://issuetracker.unity3d.com/issues/using-net-api-4-dot-x-increases-performance-spike-in-scripts-twice-when-selecting-an-object-with-a-script-for-the-first-time), 1163856)
    
*   UI: Made Unity recreate the GFX buffer if the stride size changes. ([1143087](https://issuetracker.unity3d.com/issues/canvas-removing-normal-from-the-additional-shader-channel-drop-down-causes-rendering-issues), 1144234)
    
*   UI: Updated `SetChildAlongAxis` to have a matching `SetChildAlongAxisWithScale` that takes a **Scale**.
    
*   UI Elements: A default asset is now created when a USS file import fails. (1125716)
    
*   UI Elements: Changing the an element's **overflow** after adding it to the visual tree now impacts clipping. ([1141603](https://issuetracker.unity3d.com/issues/overflow-doesnt-work-when-used-with-ui-elements), 1158365)
    
*   UI Elements: Fix the drop area of groups in graph view. (1152487, 1155396)
    
*   UI Elements: Fixed an invalid texture for toolbar elements in Light skin. ([1117232](https://issuetracker.unity3d.com/issues/missing-texture-for-a-pressed-down-ui-dropdown-when-using-the-personal-editor-skin))
    
*   UI Elements: Fixed an issue that caused the Editor to freeze when adding new elements while clearing children. (1102592)
    
*   UI Elements: Fixed an issue where resizing a clipper could leave child clippers with an invalid clipping state. (1119623)
    
*   UI Elements: Fixed an issue where some culled Inspectors and fields were displayed in the Inspector window. ([1123033](https://issuetracker.unity3d.com/issues/additional-metadata-fields-are-revealed-in-inspector-window-after-switching-from-normal-to-debug-mode-and-vice-versa), [1151394](https://issuetracker.unity3d.com/issues/particlesystemrenderer-component-appears-after-particlesystem-component-was-reverted-from-prefab-instance), [1152519](https://issuetracker.unity3d.com/issues/particlesystemrenderer-component-appears-after-added-script-is-deleted), 1153150, 1170579, 1170580)
    
*   UI Elements: Fixed an issue where the Material Editor constantly repainted the Inspector window. (1111923)
    
*   UI Elements: Fixed bound array fields in UIE not properly syncing their array sizes when the same object was being edited elsewhere. ([1141787](https://issuetracker.unity3d.com/issues/ui-elements-array-element-out-of-bounds-exception-thrown-on-undoing-or-redoing-a-change-in-float-array-field), 1153154)
    
*   UI Elements: Fixed broken edge expansion system and tesselation.
    
*   UI Elements: Fixed Play mode tint in the Editor for UIElements. (1129564)
    
*   UI Elements: Fixed the foldout triangle size. (1122034)
    
*   UI Elements: Fixed Unable to set the Foldout.text "text" or "value" attributes through UXML. ([1119589](https://issuetracker.unity3d.com/issues/unable-to-set-the-foldout-dot-text-text-or-value-attributes-through-uxml-schema), 1150532)
    
*   UI Elements: Improved consistency of `MouseEnter` and `MouseLeave` events. (1081998, 1150185)
    
*   UI Elements: Invalid **Scale** values on the Z component are now ignored and do not prevent the VisualElement from disappearing. (1134758, 1147315)
    
*   UI Elements: Picking is now faster in UIElements. (1124338)
    
*   UI Elements: Prevented the activation of Content Dragger from the Blackboard in GraphView. (1146288)
    
*   UI Elements: Prevented zooming in and out with the scroll wheel while the mouse pointer is over the Blackboard in GraphView. (1139333, 1146282)
    
*   UI Elements: Removed support for instantiating elements with `DoCreate()` in UXMLFactories
    
*   UI Elements: Resizing a VisualElement no longer causes unnecessary nudges or repainting of children. (1109689, 1144434)
    
*   UI Elements: UI element that has focus now loses focus when the window loses focus, and gets focus back when window is gets focus back. ([984433](https://issuetracker.unity3d.com/issues/uielements-textfield-still-draw-selection-when-window-is-not-focused))
    
*   Universal Windows Platform: Fixed awaiting async actions and operations on the UI thread continuing on a background thread (the continuations will now run on UI thread). ([1130193](https://issuetracker.unity3d.com/issues/uwp-messagedialog-class-causes-crash-on-il2cpp-backend), 1150948)
    
*   Universal Windows Platform: Fixed IL2CPP crashing when using certain new types (like `Windows.Foundation.GuidHelper.Equals`) in Windows SDK 17763 or newer.
    
*   Version Control: Editor Fix logging when files/folders in the Unity project are excluded from the Perforce client workspace ([1143683](https://issuetracker.unity3d.com/issues/vcs-console-constantly-prints-warning-if-file-is-excluded-from-workspace), 1145762)
    
*   Video: Camera Near Plane mode in a 2D project is not rendering the video clip only audio is heard (1135033, 1146656)
    
*   Video: Fix camera culling mask for VideoPlayer. ([1146620](https://issuetracker.unity3d.com/issues/videoplayer-renders-only-when-default-layer-is-enabled-on-cameras-culling-mask), 1152117)
    
*   WebGL: Fixed a bug when indexedDB timeout would prevent the build from loading. (1134367)
    
*   WebGL: Fixed an issue with saving PlayerPrefs in WebGL. ([1140820](https://issuetracker.unity3d.com/issues/playerprefs-dont-get-saved-in-a-webgl-build), 1145636)
    
*   WebGL: Fixed rendering errors in WebGL when canvas is not displayed. ([1141232](https://issuetracker.unity3d.com/issues/webgl-screen-position-out-of-view-frustum-error-is-thrown-when-using-display-none-style-for-gamecontainer-in-build), 1154630)
    
*   Windows: Fixed an issue that caused an iOS build to fail when a language with non-Latin characters is set as the Windows display language. ([1136098](https://issuetracker.unity3d.com/issues/windows-build-fails-on-ios-and-android-when-language-with-non-latin-characters-is-set-as-windows-display-language), 1160390)
    
*   Windows: Fixed an issue that caused key 9 sending key 8 events in the input system on Windows. ([1132663](https://issuetracker.unity3d.com/issues/windows-editor-alpha-9-key-pressed-always-return-alpha-8-key))
    
*   Windows: Fixed standalone Windows player hanging on startup on machines with strict group policies ([1083303](https://issuetracker.unity3d.com/issues/standalone-build-freezes-at-startup-on-intel-gpus))
    
*   Windows: Improved Windows crash handling reliability.
    
*   XR: Added Incremental GC on Lumin.
    
*   XR: Deprecated `UnityEngine.XR.InputTracking`s `GetLocalPosition` and `GetLocalRotation`.
    
*   XR: Device is Y-flipped when running scene on iOS Cardboard with Metal (1066864, 1153465)
    
*   XR: Final render image on Vulkan is no longer flipped vertically when single-pass stereo instancing is enabled. (1135134)
    
*   XR: Fixed Magic Leap package download in Lightweight Render Pipeline template. (1106219, 1146997)
    
*   XR: Renamed the two types of raycasts in the XRRaycastSubsystem profiler to `XR.RaycastFromScreen` and `XR.RaycastRay` for easier identification.
    
*   XR: The standalone player with Vulkan API and single-pass instanced mode no longer shows a black screen in HMD. (1142602)
    
*   XR: Unity shaders on Vulkan are now set up for stereo instancing. (1129654)
    
*   XR: Vulkan draw calls now draw to the second slice of texture array during stereo instancing. (1129656)
    
*   XR: Vulkan instance extensions are now correctly applied on Oculus. (1123193)