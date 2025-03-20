# Unity 2021.3.50f1 LTS
Published at Wed, 19 Mar 2025 09:23:25 GMT  
https://unity.com/releases/editor/whats-new/2021.3.50

# Known Issues in 2021.3.50f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Input: Touch Input is not registered correctly when using multiple displays
    ([UUM-99077](https://issuetracker.unity3d.com/issues/touch-input-is-not-registered-correctly-when-using-multiple-displays))

- Vulkan:  Application crashes with Vulkan when restoring from background on Linux
    ([UUM-90287](https://issuetracker.unity3d.com/issues/vulkan-android-application-crashes-on-android-devices-with-vulkan-when-restoring-from-background))



# 2021.3.50f1 Release Notes

## Features

- Version Control: You can now create a code review from the list of branches \(or changesets\) opening either the Desktop App or the Unity Cloud website.

- Version Control: You can now Shelve your Pending Changes when switching to another branch \(or changeset\) and decide if you want to apply them automatically after the switch.

- Version Control: You can now Shelve your selected Pending Changes, inspect the shelves content, and apply them to your workspace.



## API Changes

- iOS: Added: Added iPhone 16e device generation enums and screen cutouts.



## Changes

- Version Control: Added dedicated toolbar buttons to open the list of branches and the Branch Explorer of the Desktop App.

- Version Control: Improved the Create workspace window to suggest the matching Unity Cloud project if it exists.

- Version Control: Moved the 'Unity Version Control' menu item under 'Window'/'Version Control' submenu starting from Unity 6.1.

- Version Control: Optimized incoming changes &amp; merge to only reload the Package Manager when needed.

- Version Control: Reworded the changeset context menu "Undo this change" to "Revert this file to the previous revision" so it's more explicit.

- Version Control: Serialize the Checkin comment and tick selection so they are kept on any domain reload and play mode.

- XR: Updated com.unity.xr.openxr version to 1.14.1.



## Fixes

- 2D: Fixed camera sorting layer not breaking batch correctly for URP 2D.
    ([UUM-90792](https://issuetracker.unity3d.com/issues/normals-from-other-sorting-layers-are-passed-to-camerasortinglayertexture-when-2d-light-is-used))

- 2D: Fixed sprite instancing with 2d shaders.
    ([UUM-87636](https://issuetracker.unity3d.com/issues/graphics-dot-drawmeshinstanced-does-not-work-when-2d-renderer-and-2d-shaders-are-used))

- 2D: Fixed warning 'GetControlID at event ValidateCommand returns a controlID different from the one in the Layout event' is logged when undoing the deletion of an Edited Freeform 2D Light.
    ([UUM-90726](https://issuetracker.unity3d.com/issues/warning-getcontrolid-at-event-validatecommand-returns-a-controlid-different-from-the-one-in-the-layout-event-is-logged-when-undoing-the-deletion-of-an-edited-freeform-2d-light))

- Android: Fixed builds when having incompatible cmdline-tools version \(higher than `10.0`\).
    (UUM-96041)

- Android: Fixed the problem with additional streaming assets \(added using BuildPlayerContext.AddAdditionalPathToStreamingAssets\) being compressed in APK/AAB.
    (UUM-96090)

- Asset Import: Handle FBX Skeleton with unsupported RootNode.
    ([UUM-62869](https://issuetracker.unity3d.com/issues/crash-on-gameobject-querycomponentbytype-when-an-fbx-file-gets-imported))

- Editor: Added shared parameter indicator "*" to the name "Use incremental GC".
    ([UUM-86940](https://issuetracker.unity3d.com/issues/use-incremental-gc-is-a-shared-parameter-but-not-identified-as-one-with-a-star-when-displayed-in-the-player-settings))

- Editor: Disabled splatmaps for shadows-only terrain.
    ([UUM-79364](https://issuetracker.unity3d.com/issues/the-terrain-itself-with-layer-5-or-up-is-visible-when-the-in-terrain-settings-cast-shadows-is-set-to-shadows-only))

- Editor: Fixed graphics jobs toggle in projects settings when building for standalone targets.
    ([UUM-91713](https://issuetracker.unity3d.com/issues/graphics-jobs-toggle-in-project-settings-is-ignored-when-building-for-different-standalone-targets))

- Editor: Fixed offscreen rendering flags to be added only when the "Offscreen Rendering \(Vulkan\)" OpenXR UI setting is enabled.
    ([OXRB-358](https://issuetracker.unity3d.com/issues/mobile-the-player-displays-a-black-screen-when-the-openxr-is-used-as-the-plug-in-provider))

- Editor: Fixed to dylib files to appear in Xcode project for iOS/tvOS/visionOS.
    ([UUM-72675](https://issuetracker.unity3d.com/issues/ios-appletv-dylib-plugin-is-not-visible-in-the-xcode-but-is-added-in-the-project-folder))

- Editor: Warning about uncompressed atlas should only appear when there are compressed and uncompressed textures in the atlas. Also improve the text clarity.
    ([UUM-91216](https://issuetracker.unity3d.com/issues/a-warning-is-displayed-in-the-inspector-when-a-mesh-with-any-material-is-added-as-a-terrain-detail))

- Mobile: Fixed user certificates included in the app by default.
    ([UUM-97194](https://issuetracker.unity3d.com/issues/android-ios-unitywebrequest-requests-with-unitywebrequest-are-open-for-ssl-proxying))

- Scripting: Fixed play state change callback not being invoked when domain reload forces playmode exit.
    ([UUM-85334](https://issuetracker.unity3d.com/issues/playmodestatechange-dot-exitingplaymode-is-not-logged-when-play-mode-is-exited-due-to-recompilation))

- Shadergraph: Fixed the generation of new artifact ID of ShaderGraph on every reimport.
    ([UUM-86662](https://issuetracker.unity3d.com/issues/a-different-artifact-is-produced-every-time-when-importing-a-shadergraph-asset))

- UI Toolkit: Changed editor PopupField style to match IMGUI and have the same height as other fields.
    ([UUM-81522](https://issuetracker.unity3d.com/issues/ui-toolkit-popupfields-are-19px-when-all-the-other-fields-are-18px))

- Version Control: Ensured ignore.conf is not being reformatted when adding or removing an ignore rule, so it keeps empty lines and comments.

- Version Control: Fixed a performance issue by preventing the ConfigureLogging call on every domain reload when Unity Version Control is not used, reducing the load time by ~200ms.

- Version Control: Fixed console error GUI Error: Invalid GUILayout state in PlasticWindow view which is caused under some circumstances.

- Version Control: Fixed lock statuses to correctly refresh in Project View and Inspector after merging.

- Version Control: Fixed missing checked-out for renamed assets.

- Version Control: Fixed null exception on entering in Play Mode before creating the workspace.

- Version Control: Fixed rename asset leaves 'Added' + 'Remove locally' status instead of 'Moved'.

- Version Control: Fixed the create branch operation to work in Gluon mode which uses partial workspaces.

- Version Control: When modifying the mergespecfile.tx to use Beyond Compare, it continues to fall back to FileMerge.
    ([UUM-91595](https://issuetracker.unity3d.com/issues/unityyamlmerge-does-not-open-fallback-merge-tool-when-encountering-merge-conflicts))

- Web: Fixed bug where calling RequestUserAuthorization\(UserAuthorization.Microphone\) in the Web player would prompt the user for webcam permissions instead of microphone permissions. The microphone API is not yet supported in Web, so a warning message has been added to inform developers of this limitation.
    ([UUM-75678](https://issuetracker.unity3d.com/issues/webcam-permissions-are-asked-instead-of-microphone-permissions-when-using-requestuserauthorization-userauthorization-dot-microphone-in-the-webgl-player))

- Windows: Fixed issue with Windows Player was not calling wide character functions for DispatchMessageW, PeekMessageW, GetMessageW.
    ([UUM-90999](https://issuetracker.unity3d.com/issues/windows-unicode-custom-text-input-window-shows-question-marks-when-inserting-an-emoji))

- XR: Updated XR Interaction Toolkit \(com.unity.xr.interaction.toolkit\) to version 2.6.4.




## Package changes in 2021.3.50f1

## Packages updated

- com.unity.collab-proxy: [2.6.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.6//changelog/CHANGELOG.html) to [2.7.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.7//changelog/CHANGELOG.html)

- com.unity.render-pipelines.core: [12.1.15](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.core@12.1//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition: [12.1.15](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@12.1//changelog/CHANGELOG.html)

- com.unity.render-pipelines.high-definition-config: [12.1.15](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition-config@12.1//changelog/CHANGELOG.html)

- com.unity.render-pipelines.universal: [12.1.15](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@12.1//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.2.6](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.3//changelog/CHANGELOG.html)

- com.unity.shadergraph: [12.1.15](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.shadergraph@12.1//changelog/CHANGELOG.html)

- com.unity.visualeffectgraph: [12.1.15](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@12.1//changelog/CHANGELOG.html) to [12.1.16](https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@12.1//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [2.6.3](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.6//changelog/CHANGELOG.html) to [2.6.4](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.6//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.14.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html) to [1.14.1](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html)

**Packages deprecated**

- com.unity.purchasing.udp