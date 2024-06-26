# Unity 2023.2.18f1
Tue, 09 Apr 2024 21:11:33 GMT  
https://unity.com/releases/editor/whats-new/2023.2.18

### Known Issues in 2023.2.18f1

- Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode
    ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))

- Asset - Database: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene
    ([UUM-66207](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-openasset-because-assertion-fails-on-prefabinstance-dot-getrootgameobject-dot-isvalid-expression-while-opening-a-specific-scene))

- Asset - Database: Fix for 2023.2.X: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene
    (UUM-66278)

- Asset Bundles: Memory leak when building AssetBundle with Sprite Atlas enabled on macOS
    ([UUM-56323](https://issuetracker.unity3d.com/issues/memory-leak-when-building-assetbundle-with-sprite-atlas-enabled-on-macos))

- Asset Importers: Unity crashes on strtol_l when importing a specific .obj file
    ([UUM-42697](https://issuetracker.unity3d.com/issues/unity-crashes-on-strtol-l-when-importing-a-specific-obj-file))

- Audio Authoring: Crash on AudioUtil_CUSTOM_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached
    ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))

- IAP: [Android] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener
    ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))

- IL2CPP: [Android] Crash on Android when AndroidJavaProxy is calling from multiple threads
    ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))

- Metal: Player hangs when re-focusing the Player window after switching to a window that covers the Player window
    ([UUM-67400](https://issuetracker.unity3d.com/issues/player-hangs-when-re-focusing-the-player-window-after-switching-to-a-window-that-covers-the-player-window))

- Metal: [iOS] App crashes with out of memory exception in UnityGfxDeviceWorker when starting the app
    ([UUM-55488](https://issuetracker.unity3d.com/issues/ios-app-crashes-with-out-of-memory-exception-in-unitygfxdeviceworker-when-starting-the-app))

- Platform Audio: Crash on FMOD::CodecMPEG::setPositionInternal when a mobile platform is selected and a specific audio clip is played
    ([UUM-62086](https://issuetracker.unity3d.com/issues/crash-on-fmod-codecmpeg-setpositioninternal-when-a-mobile-platform-is-selected-and-a-specific-audio-clip-is-played))

- Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning
    ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))

- Scripting Runtime: Crash on RaiseException when selecting "Quit" in a "Fatal Error!" pop-up
    ([UUM-68119](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-selecting-quit-in-a-fatal-error-pop-up))

- Text: Blurry Text
    ([UUM-49006](https://issuetracker.unity3d.com/issues/blurry-text))

- Text: Fix for 2023.2.X: Blurry Text
    (UUM-49008)

- UI Toolkit Controls: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- WebRequest: UnityWebRequest crashes if invoked when player is quitting
    ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))



### 2023.2.18f1 Release Notes

#### Features

- iOS: Added .xcframework plugins support



#### Improvements

- Documentation: Updates for the Animation and Math API.
    (UUM-67920)

- DX12: Added documentation on how to use the Screen Space Overlay render mode alongside the Graphics Compositor.
    ([UUM-65397](https://issuetracker.unity3d.com/issues/ui-element-is-not-displayed-when-canvas-render-mode-is-set-to-screen-space-overlay))

- VFX Graph: Improve compilation times with VFX Graph using Subgraphs.



#### Fixes

- 2D: Fixed error log when the user enters play mode and sets a Tile on a Tilemap using MonoBehaviour.Start.
    ([UUM-67583](https://issuetracker.unity3d.com/issues/rendererupdatemanager-dot-updateall-must-be-called-first-error-is-thrown-when-entering-the-play-mode))

- 2D: Fixed hint text not showing when trying to slice compress texture in Sprite Editor Window slice menu.
    ([UUM-59303](https://issuetracker.unity3d.com/issues/sprites-are-sliced-wrong-when-they-are-being-sliced-automatically-on-iossupport-platform-for-macos))

- 2D: Fixed usage of a Tile Palette with the XZ orientation in the Tile Palette window.
    (UUM-67593)

- Android: Disable MemoryAdvice library integration since it crashes on some devices.
    (UUM-57044)

- Animation: Fixed a crash when deleting states in some state machines. If a state machine contained a state machine transition with a null source state \(which should not happen under normal circumstances\), unity would crash when deleting any state within the same state machine. It does not crash anymore.
    ([UUM-66549](https://issuetracker.unity3d.com/issues/crash-on-animatorstatemachine-removetransitionswithdeletingobject-when-deleting-a-newly-created-empty-state-in-animator-controller))

- Animation: Fixed display of muscle values in the AnimationWindow when linked to Timeline.
    (UUM-66112)

- Audio: Fixed an issue where entering play mode would make an open editor window for the AudioRandomContainer asset show garbled UI for the clip list.
    ([UUM-63543](https://issuetracker.unity3d.com/issues/audio-clips-list-shows-its-asset-guid-instead-of-its-name-when-entering-play-mode))

- Audio: Fixed issue where editing a script \(i.e. domain reload\) while the editor window for the AudioRandomContainer asset would throw a null reference exception.
    ([UUM-63858](https://issuetracker.unity3d.com/issues/audio-random-container-window-throws-a-nullreferenceexception-if-docked-when-editing-a-script))

- Editor: Fixed an issue where Deep Profiling Support label was labeled differently depending on if Development Build was enabled.
    ([UUM-61605](https://issuetracker.unity3d.com/issues/deep-profiling-support-is-labeled-differently-depending-on-if-development-build-is-enabled-or-disabled-in-build-settings))

- Editor: Fixed an issue where the Inspector window controls became unresponsive after exiting playmode.
    ([UUM-64580](https://issuetracker.unity3d.com/issues/unable-to-interact-with-material-inspector-window-when-entering-and-exiting-play-mode))

- Editor: Fixed an issue where the property window was throwing an error if opened when launching Unity.
    (UUM-64529)

- Editor: Fixed driver version in documentation of optix.
    ([UUM-66825](https://issuetracker.unity3d.com/issues/optix-minimum-driver-version-number-is-incorrect))

- Editor: Hide `DataMode` controller information from Inspector.
    ([UUM-67001](https://issuetracker.unity3d.com/issues/unnecessary-information-about-serialized-data-mode-controller-is-shown-when-a-custom-window-is-created))

- Graphics: Fixed a regression where creating a RenderTexture with RenderTextureFormat.Shadowmap would unintentionally fail.
    (UUM-64340)

- Graphics: Fixed ReadPixels\(\) using different Y positions.
    ([UUM-58287](https://issuetracker.unity3d.com/issues/readpixels-uses-different-y-positions-when-built-with-vulkan))

- Graphics: \[Project Settings Window \| Graphics Settings\] Fixed the default RP asset field was changing value on click, not on double click or when the object selector was closed.
    (UUM-60252)

- HDRP: Fixed an issue where Graphics Compositor Limitation section for VR was missing.
    (UUM-65373)

- HDRP: Fixed an issue where internally created Game Objects were being deallocated on scene changes.
    ([UUM-53128](https://issuetracker.unity3d.com/issues/realtime-reflection-probes-in-hdrp-stop-working-and-nullreferenceexceptions-are-thrown-in-the-player-log-when-the-scene-is-reloaded))

- HDRP: Fixed scene modification when exiting play mode with the graphics compositor enabled.
    ([UUM-58350](https://issuetracker.unity3d.com/issues/scene-is-modified-after-exiting-play-mode-when-graphics-compositor-is-enabled-in-hd-rp))

- HDRP: Fixed screen node not returning correct resolution after post-processing when dynamic resolution was enabled.

- HDRP: Fixed specular blend in premultiplied alpha.
    (UUM-48661)

- HDRP: Restore `EditorGUIUtility.labelWidth` to default after drawing Material GUI.
    ([UUM-66215](https://issuetracker.unity3d.com/issues/entity-baking-preview-gui-indentation-changes-when-the-material-gui-is-opened-or-closed))

- Scripting: Fixed  crashes that were due to an excessive use of thread local data slots.
    ([UUM-58965](https://issuetracker.unity3d.com/issues/android-crash-on-slash-data-slash-app-slash-com-dot-defaultcompany-dot-webviewandroid-7upuhqo4grf2kpmrmcjrdg-equals-equals-slash-lib-slash-arm64-slash-libxul-dot-so-libxul-dot-so-offset-0x518000-on-android-devices-when-using-webview))

- Security: Fixed some security vulnerablities by updating MbedTLS to 2.28.7.
    (UUM-63880)

- Shaders: Fixed ShaderLab-specific \#pragma directives being reported in shader source files when \#include is used.
    ([UUM-62756](https://issuetracker.unity3d.com/issues/number-pragma-directives-in-hlsl-files-are-not-being-ignored-when-number-include-is-used))

- uGUI: Fixed an issue where renderer layer properties reset to default in prefab mode.
    ([UUM-62507](https://issuetracker.unity3d.com/issues/renderer-dot-sortinglayer-renderer-dot-sortinglayerid-and-renderer-dot-sortinglayername-is-set-to-default-0-and-when-adding-a-canvas-component-to-a-prefab-in-prefab-mode))

- uGUI: Fixed issue with the input-field which was causing a performance issues in the editor.

- UI Toolkit: Fixed  an issue where TreeView with dynamic height clipped items erratically when expanding/collapsing items.
    ([UUM-34553](https://issuetracker.unity3d.com/issues/treeview-with-dynamic-height-clips-items-erratically-when-expanding-slash-collapsing-items))

- UI Toolkit: Fixed "margin: auto" applied even when the visual Element has it's Display is set to none.
    ([UUM-40647](https://issuetracker.unity3d.com/issues/visualelement-is-applying-margin-auto-even-when-display-is-set-to-none))

- UI Toolkit: Fixed a issue with the shrink algorithm when an element height was smaller min-height.

- UI Toolkit: Fixed an issue when in Runtime on mobile, a ScrollView would no longer scroll if the touch interaction needed to be treated by a child element first \(ex: a menu from a DropdownField\).
    ([UUM-39969](https://issuetracker.unity3d.com/issues/scrollview-scrolls-when-clicking-a-button-after-selecting-the-dropdownfield-item))

- UI Toolkit: Fixed an issue where ManagedReference fields with a custom PropertyDrawer were not refreshed properly when the type changed.
    ([UUM-66550](https://issuetracker.unity3d.com/issues/managedreference-fields-with-a-custom-propertydrawer-arent-refreshed-properly-when-changing-properties))

- UI Toolkit: Fixed an issue where Nested PropertyDrawer did not work when there was both an Attribute drawer and a Drawer for the type.
    ([UUM-66687](https://issuetracker.unity3d.com/issues/nested-propertydrawer-doesnt-work-when-theres-both-an-attribute-drawer-and-a-drawer-for-the-type))

- UI Toolkit: Fixed attribute overrides when it's multiple levels deep in the Hierarchy in the UI Builder.
    ([UUM-59501](https://issuetracker.unity3d.com/issues/cannot-override-uxml-attributes-when-its-multiple-levels-deep-in-the-hierarchy))

- UI Toolkit: Fixed dimensions of a parent element did not include padding when calculating the top/left/right/bottom values of an absolute element.
    ([UUM-25738](https://issuetracker.unity3d.com/issues/ui-toolkit-dimensions-of-a-parent-element-do-not-include-padding-when-used-in-anchors-of-an-absolute-positioned-children-element))

- UI Toolkit: Fixed inspector elements from being culled in secondary inspector window and avoid unexpected behavioral errors been thrown when selecting an Asset then selecting another type of asset and deselecting it.
    ([UUM-35998](https://issuetracker.unity3d.com/issues/textureimporterinspector-dot-oninspectorgui-must-call-applyrevertgui-to-avoid-unexpected-behaviour-dot-thrown-when-selecting-asset-then-selecting-and-deselecting-texture-2d))

- UI Toolkit: Fixed SendMessage warning when changing scene with UIDocuments present in the scene.
    ([UUM-57741](https://issuetracker.unity3d.com/issues/sendmessage-cannot-be-called-during-awake-warnings-appear-when-loading-a-scene-with-loadsceneasync-if-using-ui-toolkit-in-the-scene))

- UI Toolkit: Fixed underline shadows.
    ([UUM-54791](https://issuetracker.unity3d.com/issues/the-underline-fades-away-when-you-zoom-in-slash-out-in-the-ui-builder))

- UI Toolkit: \[Properties\] Fixed an issue where explicit interface properties would have an invalid property name.
    ([UUM-63548](https://issuetracker.unity3d.com/issues/console-errors-are-shown-when-generating-a-propertybag-for-a-type-with-an-explicit-interface-property))

- UI Toolkit: \[Properties\] Fixed an issue where the source generator would generate invalid code for partial generic types.
    ([UUM-62692](https://issuetracker.unity3d.com/issues/cs0117-and-cs0426-errors-are-thrown-when-generating-a-propertybag-for-a-generic-type-designated-as-partial))

- Universal RP: Fixed a depth buffer disappearing after using SwapColorBuffer.
    ([UUM-44446](https://issuetracker.unity3d.com/issues/depthtarget-disappears-when-calling-swapcolorbuffer))

- Universal RP: Fixed depth only cameras trying to render renderer features which requires depth.
    ([UUM-14679](https://issuetracker.unity3d.com/issues/errors-thrown-in-the-console-window-when-decal-renderer-feature-is-enabled))

- Universal RP: Fixed false-negative missing RendererFeatures errors.
    ([UUM-58944](https://issuetracker.unity3d.com/issues/importing-urp-samples-throwns-errors))

- Universal RP: Fixed preview windows no longer renders render objects features.
    ([UUM-59428](https://issuetracker.unity3d.com/issues/urp-material-preview-color-is-affected-when-the-renderobjects-feature-is-enabled))

- Universal RP: Fixed shadow flickering when using Screen Space shadows and have depth priming enabled.
    ([UUM-48838](https://issuetracker.unity3d.com/issues/screen-space-shadows-render-feature-draws-incorrect-shadowing-on-opaques-when-depth-priming-mode-is-set-to-auto-or-forced))

- Universal RP: Fixed the NativeRenderPass camera target MSAA logic to match the non-NRP path.
    ([UUM-56396](https://issuetracker.unity3d.com/issues/errors-are-thrown-when-native-renderpass-is-enabled))

- Universal RP: Scriptable TAA settings.
    ([UUM-49324](https://issuetracker.unity3d.com/issues/api-to-change-taa-settings-is-internal))

- URP: Restore `EditorGUIUtility.labelWidth` to default after drawing MaterialHeaderScopes.
    ([UUM-66215](https://issuetracker.unity3d.com/issues/entity-baking-preview-gui-indentation-changes-when-the-material-gui-is-opened-or-closed))

- VFX Graph: Fixed an issue where some VFX was always being considered dirty.
    ([UUM-21302](https://issuetracker.unity3d.com/issues/vfx-file-gets-modified-without-making-changes-when-saving-project))

- VFX Graph: Fixed Construct Matrix operator serialization issue.
    ([UUM-57915](https://issuetracker.unity3d.com/issues/construct-matrix-operator-is-causing-serialization-issues))

- VFX Graph: Fixed unexpected error message when compiling some VFX "Expression graph was marked as dirty".
    ([UUM-54689](https://issuetracker.unity3d.com/issues/error-expression-graph-was-marked-as-dirty-after-compiling-context-for-ui-logged-in-console-when-creating-firework-and-head-and-trails-vfx-templates))




#### Package changes in 2023.2.18f1

#### Packages updated

- com.unity.services.cloudcode: [2.5.0](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.5//changelog/CHANGELOG.html) &#x2192; [2.6.1](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.6//changelog/CHANGELOG.html)

- com.unity.xr.arcore: [5.1.2](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.1//changelog/CHANGELOG.html) &#x2192; [5.1.3](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.1//changelog/CHANGELOG.html)

- com.unity.xr.arfoundation: [5.1.2](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.1//changelog/CHANGELOG.html) &#x2192; [5.1.3](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.1//changelog/CHANGELOG.html)

- com.unity.xr.arkit: [5.1.2](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.1//changelog/CHANGELOG.html) &#x2192; [5.1.3](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.1//changelog/CHANGELOG.html)