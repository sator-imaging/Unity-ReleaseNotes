# Unity 2022.3.69f1 LTS
Published at Wed, 19 Nov 2025 14:05:02 GMT  
https://unity.com/releases/editor/whats-new/2022.3.69f1

# Known Issues in 2022.3.69f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- Metal:  Game freezes after command buffer Timeout error
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- Video: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)

- Vulkan: Crashes in the wild on Vulkan in CreateDepthSurfaceImpl 
    ([UUM-114531](https://issuetracker.unity3d.com/issues/crashes-in-the-wild-on-vulkan-in-createdepthsurfaceimpl))



# 2022.3.69f1 Release Notes

## API Changes

- uGUI: Added: Added protected bool BaseInputModule.sendPointerHoverToParent property getter and setter.
    ([ISXB-586](https://issuetracker.unity3d.com/issues/the-pointer-event-is-called-on-the-parent-object-even-when-the-send-pointer-hover-to-parent-is-off))



## Fixes

- 2D: Fixed NullReferenceException with LightBatchingDebugger.
    ([UUM-116667](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-on-a-new-project-when-creating-a-new-project-after-exiting-a-project-with-light-batching-debugger-window-docked))

- Animation: Fixed issues where normalized time would not be incrementing on some animator states, along with excessive errors being logged.
    ([UUM-121440](https://issuetracker.unity3d.com/issues/animator-is-still-spamming-too-much-when-states-stay-active-too-long))

- Editor: Fixed a race condition in the licensing client where the Editor would succeed to make the client acquire a floating license faster than it had finished loading licenses at startup, which would make it fail to pick up the new license.
    ([UUM-121408](https://issuetracker.unity3d.com/issues/file-watcher-does-not-trigger-after-the-acquirefloatinglease-and-before-the-entitlement-check))

- Editor: Fixed an Editor crash happening when .shader files contain raygeneration, miss or callable shaders. These shader types are supported in .raytrace files only.
    ([UUM-109230](https://issuetracker.unity3d.com/issues/dx12-crash-on-shaderlab-subprogram-compile-or-freeze-when-compiling-a-specific-ray-tracing-shader))

- Editor: Fixed for missing "Some values driven by GridLayoutGroup" when users alter elements under parent/sibling LayoutGroup.
    ([UUM-100091](https://issuetracker.unity3d.com/issues/some-values-driven-by-gridlayoutgroup-message-disappears-on-a-child-ui-gameobject-when-disabling-a-non-parent-gameobject))

- Editor: Fixed GameView not rendering on Quest when hidden in Editor.
    ([UUM-119451](https://issuetracker.unity3d.com/issues/quest-game-view-is-no-longer-rendered-in-the-hmd-if-its-hidden-in-the-editor-when-using-meta-link))

- Editor: Fixed Tesselation plus Quad topology plus SRP Batcher.
    ([UUM-121990](https://issuetracker.unity3d.com/issues/automatic-lod-fails-and-srp-batcher-incompatibility-occurs-when-using-spline-based-quad-topology-meshes))

- Editor: Fixed the link that opens when clicking on the ? icon in the RayTracingShader \(.raytrace\) inspector in the Editor.
    ([UUM-122368](https://issuetracker.unity3d.com/issues/ray-tracing-shader-link-to-the-documentation-isnt-working))

- Editor: Prevent logging session tokens in the editor log.
    (UUM-121872)

- Editor: Prevented a crash when an internal source generated method is missing.
    ([UUM-117749](https://issuetracker.unity3d.com/issues/crash-on-do-runtime-invoke-when-reopening-a-specific-project-after-failing-to-build-it))

- Editor: Removed missing scripts in SplitScreen and OcclusionEffect scenes from the URP samples.
    ([UUM-71852](https://issuetracker.unity3d.com/issues/urp-package-samples-missing-scripts-in-unity-2022-plus))

- Graphics: Applied workaround for video black screen issue on Mali GPUs with OpenGLES.
    (UUM-116491)

- Graphics: Color Picker - Swatches - HDR - Was storing the color.gamma instead of the color.
    ([UUM-121056](https://issuetracker.unity3d.com/issues/incorrect-color-values-are-saved-for-swatches-when-using-hdr-color-picker))

- Graphics: Color Picker - Swatches - HDR - Was storing the color.gamma instead of the color.
    ([UUM-121056](https://issuetracker.unity3d.com/issues/incorrect-color-values-are-saved-for-swatches-when-using-hdr-color-picker))

- Graphics: Disabled the CAMetalDisplayLink on iOS as using it might cause GPU hangs and rendering freeze. It will be enabled again once we find the underlying cause.
    ([UUM-123207](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error))

- Graphics: Fixed sporadic crash when using Cloth rendering with Vulkan.
    ([UUM-90932](https://issuetracker.unity3d.com/issues/android-crash-on-gfxdevicevkbase-drawbuffersbatchmode-in-the-player-when-loading-slash-unloading-character-models))

- Graphics: When UpdateExternalTexture is called it will Unregister the previous texture to free the memory.
    ([UUM-105771](https://issuetracker.unity3d.com/issues/memory-increases-indefinitely-when-playing-vlc-video-stream))

- iOS: Fixed arg typo in updateLayerDrawableSizeFromBounds.
    (UUM-125390)

- iOS: Fixed arg typo in updateLayerDrawableSizeFromBounds.
    (UUM-125390)

- Linux: Fixed Steam Deck D-Pad is either not working or sometimes working when UI-&gt;Navigation is set to "Pass Through" in Input Actions.
    ([UUM-97138](https://issuetracker.unity3d.com/issues/linux-d-pad-is-either-not-working-or-sometimes-working-when-ui-navigation-is-set-to-pass-through-in-input-actions))

- Services: Fixed exception events not appearing on the Diagnostics dashboard.
    (ULO-7366)

- Shaders: Fixed unnecessary shader warnings and errors being logged when running with -batchmode -nographics.
    ([UUM-114187](https://issuetracker.unity3d.com/issues/unnecessary-warnings-are-logged-when-running-player-with-batchmode-nographics))

- UI Toolkit: Fixed the behaviour of stretchable columns in a MultiColumn control with StretchMode.Grow.
    (UUM-101267)

- Version Control: Fixed a NullReferenceException that was raised on double-clicking an asset that is "Copied \(new\)" \(new file added from a shelve\).

- Version Control: Fixed a NullReferenceException that was raised when the workspace is removed with Pending Changes.

- Version Control: Fixed Inspector and Project's Asset Menu to allow to Check in "Changed" items.

- Version Control: Fixed Inspector and Project's Asset Menu to allow to Undo "Changed" items.

- Version Control: Fixed Library folder that was sometimes wrongly added to source control on a new project created from the Hub.

- Version Control: Fixed the "unknown" status displayed after restoring a workspace that was previously removed.

- Version Control: Fixed the alignment of Unity Version Control's settings with the title of the window.
    ([UUM-122499](https://issuetracker.unity3d.com/issues/version-control-information-does-not-align-with-window-title))

- Version Control: Fixed the Changesets view that could crash the Editor when displaying a very long changeset comment, with "PPtr&lt;Shader&gt;::operator Shader*\(\) const".

- Version Control: Fixed the console error that occured when using CTRL-H keyboard shortcut to Hide a branch.

- Version Control: Fixed the Controlled and Private overlay icons reverted back to earlier versions, based on user feedback.

- Version Control: Fixed the diff panel keyboard shortcuts that didn't take into account the focus to open the diff on the correct item.

- Version Control: Fixed the GUILayout error that occured when applying a shelve with pending merge link.

- Version Control: Fixed the icon that was blurry and pixelated when displayed in our Unity Version Control window's tab.
    ([UUM-122495](https://issuetracker.unity3d.com/issues/unity-version-control-icon-is-blurry-and-pixalated))

- Version Control: Fixed the Item checkbox that was unresponsive when the Pending Changes list is empty. It is now disabled.

- Version Control: Fixed the merge error message that didn't fit in available space and was truncated.

- Version Control: Fixed the merge link text that was not centered vertically with its icon.

- Version Control: Fixed the new "Create Branch based on" dialog variant that was truncated, hiding the buttons, in 2.10.0.

- Version Control: Fixed the pending changes success message appearing in the status bar instead of the main area when this one is empty.

- Version Control: Fixed the Pending changes view that was refreshed on window activation for no reason.

- Version Control: Fixed the Project Settings window to automatically refresh when the plugin is enabled.
    ([UUM-122519](https://issuetracker.unity3d.com/issues/unity-version-control-window-lets-vcs-workspace-get-created-even-when-unity-vcs-is-disabled-in-project-settings-and-switches-to-vcs-being-enabled-after-reopening-the-project-settings-window))

- Version Control: Fixed the Shelve view that was missing a keyboard shortcut to open the diff in the Desktop Application.

- Version Control: Fixed the Toolbar button icon that was not visible for uncontrolled projects for Editor older than Unity 6.3.

- Version Control: Fixed the Toolbar button showing an "unknown" status after removal of the workspace.

- Version Control: Fixed the Toolbar button that should be visible by default in 6.3+.

- Version Control: Fixed the Toolbar button to correctly hide when disabling the Unity Version Control package.
    ([UUM-122521](https://issuetracker.unity3d.com/issues/version-control-customizable-toolbar-is-fully-functioning-and-has-no-visual-changes-or-indication-when-vcs-is-disabled-in-project-settings-after-creating-a-workspace))

- Version Control: Fixed the Undo changes operation so that it can now apply to the selection even if it contains some Private files.

- WebGL: Fixed an issue where `DownloadHandlerScript.CompleteContent` was called twice in WebGL builds.
    ([UUM-109862](https://issuetracker.unity3d.com/issues/downloadhandlerscript-dot-completecontent-is-called-twice-when-building-for-webgl))




## Package changes in 2022.3.69f1

## Packages updated

- com.unity.collab-proxy: [2.10.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.10//changelog/CHANGELOG.html) to [2.10.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.10//changelog/CHANGELOG.html)

- com.unity.services.user-reporting: [2.0.11](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) to [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.4.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.4//changelog/CHANGELOG.html) to [1.7.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- com.unity.xr.management: [4.4.0](https://docs.unity3d.com/Packages/com.unity.xr.management@4.4//changelog/CHANGELOG.html) to [4.5.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html)

- com.unity.profiling.systemmetrics.mali: [1.0.3](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.0//changelog/CHANGELOG.html) to [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)

- com.unity.services.levelplay: [8.10.1](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html) to [8.10.2](https://docs.unity3d.com/Packages/com.unity.services.levelplay@8.10//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.cloud.draco@5.4.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- [com.unity.cloud.ktx@3.6.0](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)

**Packages deprecated**

- com.unity.muse.common - "This package is no longer supported. Muse is being replaced with Unity AI."

- com.unity.muse.sprite - "This package is no longer supported. Muse is being replaced with Unity AI."

- com.unity.muse.texture - "This package is no longer supported. Muse is being replaced with Unity AI."

- com.unity.muse.chat - "This package is no longer supported. Muse is being replaced with Unity AI."