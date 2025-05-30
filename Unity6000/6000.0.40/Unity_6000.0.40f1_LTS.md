# Unity 6000.0.40f1 LTS
Published at Tue, 25 Feb 2025 16:31:05 GMT  
https://unity.com/releases/editor/whats-new/6000.0.40

# Known Issues in 6000.0.40f1

- 3D Physics: Freeze when calling Rigidbody.SweepTestAll in a specific project
    ([UUM-96080](https://issuetracker.unity3d.com/issues/freeze-when-calling-rigidbody-dot-sweeptestall-in-a-specific-project))

- Analytics: [Android]Crash on lib/arm64/libil2cpp.so when Unity Analytics and Engine Code stripping are enabled
    ([UUM-95408](https://issuetracker.unity3d.com/issues/android-crash-on-lib-slash-arm64-slash-libil2cpp-dot-so-when-unity-analytics-and-engine-code-stripping-are-enabled))

- Android:  [iOS] [UnityWebRequest] Requests with "UnityWebRequest" are open for SSL Proxying
    ([UUM-97194](https://issuetracker.unity3d.com/issues/android-ios-unitywebrequest-requests-with-unitywebrequest-are-open-for-ssl-proxying))

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- Audio Authoring: Audio Reverb Zone still produces sound when the Audio Source volume is 0
    ([UUM-92689](https://issuetracker.unity3d.com/issues/audio-reverb-zone-still-produces-sound-when-the-audio-source-volume-is-0))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DOTS: URP Cascaded Shadows do not have a falloff in Player when the Player is built not in Development Mode
    ([UUM-97415](https://issuetracker.unity3d.com/issues/urp-cascaded-shadows-do-not-have-a-falloff-in-player-when-the-player-is-built-not-in-development-mode))

- HDRP: Graphics Compositor breaks Unity rendering when the "Output Camera" is changed to a scene Camera and one Camera SubLayer is active.<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84610

- Packman: [windows only] Switching Project when importing complete project does not import all assets and project opens incomplete
    ([UUM-88051](https://issuetracker.unity3d.com/issues/switching-project-when-importing-complete-project-does-not-import-all-assets-and-project-opens-incomplete))

- Scripting Runtime: Crash on UnityEditor.AssetDatabase:StopAssetEditing when removing HDRP Package after having imported Water Samples
    ([UUM-78164](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-stopassetediting-when-removing-hdrp-package-after-having-imported-water-samples))

- Serialization: Crash on MonoBehaviour::VirtualRedirectTransfer when closing Editor after removing HDRP and importing Water Samples before
    ([UUM-97847](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-virtualredirecttransfer-when-closing-editor-after-removing-hdpr-and-importing-water-samples-before))

- Serialization: The "UniversalRenderPipelineGlobalSettings.asset" is creating noise in the git diff when building a Player
    ([UUM-80052](https://issuetracker.unity3d.com/issues/the-universalrenderpipelineglobalsettings-dot-asset-is-creating-noise-in-the-git-diff-when-building-a-player))

- Shader System: Crash after the “State comes from an incompatible keyword space“ log when opening the project
    ([UUM-98620](https://issuetracker.unity3d.com/issues/crash-after-the-state-comes-from-an-incompatible-keyword-space-log-when-opening-the-project))

- Shortcut Management: Adding non-context menu item via ContextMenuUtility API can crash Editor down the line
    ([UUM-98587](https://issuetracker.unity3d.com/issues/crash-on-multiple-stack-traces-when-doing-actions-with-probuilder))

- SpeedTree: This release of SpeedTree includes a change to the interface of the SpeedTree8Wind shadergraph node. If you have an animated SpeedTree in the shadergraph, be sure to connect an ObjectSpacePosition node to the input of the SpeedTree8Wind.  If the wind node does not have an input on the ObjectSpacePosition port, the mesh will be shrunk down to a point at origin \(making it seem to vanish\).<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84616

- SRP XR: GPU utilization increases by 20% on Meta Quest headsets when Render Graph is enabled on 6000.0.16f1 and higher
    ([UUM-90118](https://issuetracker.unity3d.com/issues/gpu-utilization-increases-by-20-percent-on-meta-quest-headsets-when-render-graph-is-enabled-on-6000-dot-0-16f1-and-higher))

- SRP XR: The Player renders black on a Quest headset when MSAA, Post Processing, and Spacewarm depth submission are enabled
    ([UUM-84612](https://issuetracker.unity3d.com/issues/the-player-renders-black-on-a-quest-headset-when-msaa-post-processing-and-spacewarm-depth-submission-are-enabled))

- Text: TMP 'Bold' Font Style is rendered with incorrect Font when a Font Asset without Bold typeface is selected
    ([UUM-97382](https://issuetracker.unity3d.com/issues/tmp-bold-font-style-is-rendered-with-incorrect-font-when-a-font-asset-without-bold-typeface-is-selected))

- UI Toolkit Framework: UI Toolkit buttons stop receiving inputs when entering the new Scene while holding a button during Scene change
    ([UUM-98080](https://issuetracker.unity3d.com/issues/ui-toolkit-buttons-stop-receiving-inputs-when-entering-the-new-scene-while-holding-a-button-during-scene-change))

- Vulkan: [Android] [Vulkan] [WebCamTexture] "WebCamTexture.Play" crashes the application when the camera is started
    ([UUM-95365](https://issuetracker.unity3d.com/issues/android-vulkan-webcamtexture-webcamtexture-dot-play-crashes-the-application-when-the-camera-is-started))

- Web Platform: The Player freezes on load when building Web platform
    ([UUM-98296](https://issuetracker.unity3d.com/issues/the-player-freezes-on-load-when-building-web-platform))

- XR SDK: [Quest] Screen flashes for several seconds when enabling microphone permissions
    ([UUM-72660](https://issuetracker.unity3d.com/issues/quest-screen-flashes-for-several-seconds-when-enabling-microphone-permissions))



# 6000.0.40f1 Release Notes

## Features

- Version Control: User can create a code review from the list of branches \(or changesets\) opening either the Desktop App or the Unity Cloud website.

- Version Control: User can Shelve your Pending Changes when switching to another branch \(or changeset\) and decide if you want to apply them automatically after the switch.

- Version Control: Users can Shelve your selected Pending Changes, inspect the shelves content, and apply them to your workspace.



## Improvements

- Build Pipeline: Added pdb files for all platform Editor extensions, this will provide better logs in case there are exceptions in platform Editor code.



## Changes

- Graphics: r8g8b8a8 abd b8g8r8a8 srgb formats now report LoadStore unsupported on intel mac, since srgb writes are explicitly not supported there,
    (UUM-95478)

- Version Control: Added dedicated toolbar buttons to open the list of branches and the Branch Explorer of the Desktop App.

- Version Control: Improve the Create workspace window to suggest the matching Unity Cloud project if it exists.

- Version Control: Moved the 'Unity Version Control' menu item under 'Window'/'Version Control' submenu starting from Unity 6.1.

- Version Control: Optimized incoming changes &amp; merge to only reload the Package Manager when needed.

- Version Control: Reworded the changeset context menu "Undo this change" to "Revert this file to the previous revision" so it's more explicit.

- Version Control: Serialize the Checkin comment and tick selection so they are kept on any domain reload and play mode.



## Fixes

- 2D: Fixed back buffer clear when pixel perfect crop frame is used.
    ([UUM-93255](https://issuetracker.unity3d.com/issues/custom-mouse-sprite-leaving-a-trail-when-moved-outside-of-the-pixel-perfect-cameras-components-windowbox-borders))

- 2D: Fixed camera sorting layer not breaking batch correctly for URP 2D.
    ([UUM-90792](https://issuetracker.unity3d.com/issues/normals-from-other-sorting-layers-are-passed-to-camerasortinglayertexture-when-2d-light-is-used))

- 2D: Fixed depth/stencil errors on Android.
    ([UUM-91055](https://issuetracker.unity3d.com/issues/android-error-rendertexture-dot-create-failed-depth-slash-stencil-format-unsupported-d32-sfloat-s8-uint-94-and-others-shown-and-the-game-view-is-rendered-black-when-using-urp-2d-renderer-with-unity-6))

- 2D: Fixed flickering in the Tile Palette window when the clipboard view is resized.
    ([UUM-93105](https://issuetracker.unity3d.com/issues/tilemap-palette-preview-flickers-when-scaled))

- Android: Fixed the problem with additional streaming assets \(added using BuildPlayerContext.AddAdditionalPathToStreamingAssets\) being compressed in APK/AAB.
    (UUM-96090)

- Android: Fixedmissing pdb files for Android Editor extensions - AndroidPlayerBuildProgram.Data.pdb, AndroidPlayerBuildProgram.pdb, Unity.Android.Gradle.pdb, Unity.Android.Types.pdb, UnityEditor.Android.Extensions.pdb. This will improve Editor.log contents when there's an exception happening in Android editor code.
    (UUM-95520)

- Asset Import: Fixed an issue to handle FBX Skeleton with unsupported RootNode.
    ([UUM-62869](https://issuetracker.unity3d.com/issues/crash-on-gameobject-querycomponentbytype-when-an-fbx-file-gets-imported))

- Documentation: Updated documentation references for URP/HDRP Camera, Decal projector, Probe Volumes.
    ([UUM-91777](https://issuetracker.unity3d.com/issues/camera-sub-dropdown-open-reference-buttons-do-not-work))

- DX12: Fixed the memory of released textures accumulating, when the editor is out of focus.
    ([UUM-86354](https://issuetracker.unity3d.com/issues/allocated-graphics-memory-does-not-get-released-when-the-editor-is-out-of-focus-while-using-d3d12-graphics-api))

- Editor: Fixed a bug that would cause the editor to throw a null reference exception when selecting a Video Clip.
    (UUM-83274)

- Editor: Fixed an issue for missing help button for RenderGraphViewer.
    ([UUM-85773](https://issuetracker.unity3d.com/issues/rendergraphviewer-no-help-button-that-could-lead-to-the-documentation-page))

- Editor: Fixed an issue to hide Edit menu items added by Apple Intelligence.
    (UUM-96160)

- Editor: Fixed an issue where macOS Editor would stutter when navigating Scene View with Middle Mouse Button.
    (UUM-77258)

- Editor: Fixed an issue where the create menu no longer has empty entries after updating packages in the project on Linux or exiting play mode on macOS.
    ([UUM-89106](https://issuetracker.unity3d.com/issues/ubuntu-possible-for-create-menu-to-show-sections-with-no-options-inside))

- Editor: Fixed corrupted uxml file opens in the UI Builder.
    (UUM-71448)

- Editor: Fixed crash related to AudioSource with AudioRandomContainer when performing undo in play mode of clip added in edit mode.
    (UUM-88955)

- Editor: Fixed graphics jobs toggle in projects settings when building for standalone targets.
    ([UUM-91713](https://issuetracker.unity3d.com/issues/graphics-jobs-toggle-in-project-settings-is-ignored-when-building-for-different-standalone-targets))

- Editor: Prevent "Attempting to draw with missing bindings" warning from being reported in some cases
    ([UUM-92382](https://issuetracker.unity3d.com/issues/warnings-attempting-to-draw-with-missing-bindings-are-logged-when-opening-the-hdrp-vfx-template-sample-scene))

- GI: Fixed an issue by not clampping the environment sample count in the lighting window to 2048.
    ([UUM-96953](https://issuetracker.unity3d.com/issues/environment-samples-count-resets-to-2048-when-entering-a-higher-number))

- Graphics: Fixed a rare crash on certain Samsung devices when running GLES.
    (UUM-29705)

- Graphics: Fixed seams visible for non-infinite instanced quads in the water surface.
    ([UUM-86738](https://issuetracker.unity3d.com/issues/seams-are-visible-on-the-water-system-when-multiple-tiles-are-used-and-their-surface-type-is-set-to-river))

- IL2CPP: Fixed a UnityLinker crash when `--enable-report` is used on a large project.
    ([UUM-95599](https://issuetracker.unity3d.com/issues/unitylinker-causes-crash-when-outputting-snapshot-data-for-very-large-projects))

- IL2CPP: Fixed issue where build would fail if the project's root directory contained files named after project assemblies.
    ([UUM-91340](https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-there-are-empty-files-in-projects-root-directory))

- Linux: Fixed assertion failure on ExFAT File systems when "Build and Run" is executed.
    ([UUM-91555](https://issuetracker.unity3d.com/issues/linux-assertion-failed-on-expression-success-and-and-actual-equals-equals-size-error-is-thrown-when-building-project-to-another-partition-with-a-different-file-system))

- Mono: Fixed a crash on domain reload when Windows Form is using a tooltip window.
    ([UUM-79065](https://issuetracker.unity3d.com/issues/crash-on-dispatchmessagew-when-using-folferbrowserdialog))

- Physics: Fixed an issue where calling Physics.IgnoreCollision\(colA, colB, false\) would not trigger PhysX's collision filter to re-evaluate contacts. Effectively allowing the two shapes to still ignore collision until one of them had it's filtering data updated.
    ([UUM-96257](https://issuetracker.unity3d.com/issues/overlapping-objects-do-not-collide-when-setting-physics-dot-ignorecollision-to-false))

- Prefabs: Fixed an issue to reconnect proxy parent in Prefab Stage.
    ([UUM-79087](https://issuetracker.unity3d.com/issues/prefab-mode-in-context-in-the-hierarchy-disappears-when-undoing-the-changes))

- Terrain: Fixed terrain billboard grass rendering when dynamic batching is enabled in the URP asset.
    ([UUM-67798](https://issuetracker.unity3d.com/issues/terrain-details-fail-to-render-correctly-when-dynamic-batching-is-enabled-in-urp-settings))

- UI Toolkit: A BaseField's tooltip now appears only when hovering its label, unless the BaseField has a tooltip set on its label directly.
    (UUM-68606)

- UI Toolkit: Fixed a rendering issue caused by reading worldClip in GeometryChangeEvent.
    ([UUM-93269](https://issuetracker.unity3d.com/issues/stw-6-dot-1-ui-builder-inspector-fields-get-corrupted-when-docked-ui-builder-is-maximized))

- UI Toolkit: Fixed warning when importing UXML "Import of asset setup artifact dependency to but dependency isn't used and therefore not registered in the asset database".
    ([UUM-68160](https://issuetracker.unity3d.com/issues/asset-database-warning-is-thrown-when-declaring-font-variable-in-the-uss-text-file))

- Universal RP: Fixed an issue to prevent the fog pass from being enqueued when the fog pass was not properly initialized.
    ([UUM-90255](https://issuetracker.unity3d.com/issues/point-light-source-stops-lighting-when-moved-out-of-camera-frustum-in-player-while-having-2-directional-lights-in-scene-present-and-a-fog-enabled-by-script))

- Version Control: Fixed a performance issue by preventing the ConfigureLogging call on every domain reload when Unity Version Control is not used, reducing the load time by ~200ms.

- Version Control: Fixed an issue to ensured ignore.conf was not being reformatted when adding or removing an ignore rule, so it keeps empty lines and comments.

- Version Control: Fixed console error GUI Error: Invalid GUILayout state in PlasticWindow view which is caused under some circumstances.

- Version Control: Fixed lock statuses to correctly refresh in Project View and Inspector after merging.

- Version Control: Fixed missing checked-out for renamed assets.

- Version Control: Fixed null exception on entering in Play Mode before creating the workspace.

- Version Control: Fixed rename asset leaves 'Added' + 'Remove locally' status instead of 'Moved'.

- Version Control: Fixed the create branch operation to work in Gluon mode which uses partial workspaces.

- VFX Graph: Fixed an issue by preventing VFXRenderer direct material modification that could lead to crashes.
    ([UUM-89988](https://issuetracker.unity3d.com/issues/crash-on-scriptablerenderloopdraw-when-rendering-a-specific-vfx-in-play-mode))

- VFX Graph: Fixed VFX Graph template window was empty when the Terrain Tool package is installed.
    ([UUM-95871](https://issuetracker.unity3d.com/issues/vfx-template-window-is-empty-because-of-an-exception))

- Web: Fixed the UncaughtReference error when clicking the diagnostics_icon in the Web Diagnostics Overlay on desktop browser
    (UUM-96115)




## Package changes in 6000.0.40f1

## Packages updated

- com.unity.collab-proxy: [2.6.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.6//changelog/CHANGELOG.html) to [2.7.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.7//changelog/CHANGELOG.html)

- com.unity.render-pipelines.core: [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@17.0//changelog/CHANGELOG.html) to [17.0.4](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@17.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition: [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@17.0//changelog/CHANGELOG.html) to [17.0.4](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@17.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition-config: [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@17.0//changelog/CHANGELOG.html) to [17.0.4](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@17.0//changelog/CHANGELOG.html)

- com.unity.render-pipelines.universal: [17.0.3](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@17.0//changelog/CHANGELOG.html) to [17.0.4](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@17.0//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.2.7](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.3//changelog/CHANGELOG.html)

- com.unity.shadergraph: [17.0.3](https://docs.unity3d.com/Packages/com.unity.shadergraph@17.0//changelog/CHANGELOG.html) to [17.0.4](https://docs.unity3d.com/Packages/com.unity.shadergraph@17.0//changelog/CHANGELOG.html)

- com.unity.visualeffectgraph: [17.0.3](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@17.0//changelog/CHANGELOG.html) to [17.0.4](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@17.0//changelog/CHANGELOG.html)

- com.unity.memoryprofiler: [1.1.4](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.5](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)