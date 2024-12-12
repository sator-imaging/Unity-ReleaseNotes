# Unity 2021.3.47f1 LTS
Published at Wed, 11 Dec 2024 10:43:30 GMT  
https://unity.com/releases/editor/whats-new/2021.3.47

# Known Issues in 2021.3.47f1

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Vulkan: [Android] Particles not rendered in the Player on some Android devices with Android 14
    ([UUM-68080](https://issuetracker.unity3d.com/issues/android-particles-not-rendered-in-the-player-on-some-android-devices-with-android-14))



# 2021.3.47f1 Release Notes

## Features

- Version Control: Added an menu entry to 'Open in Unity Cloud' showing the repository in the Unity Dashboard.

- Version Control: Added copy path &amp; history context menu actions in all menus where they apply.

- Version Control: Added diff and merge settings in Project Settings -&gt; Version Control -&gt; Unity Version Control Settings.

- Version Control: Added file conflict &amp; dir conflict context menu actions to the merge view.

- Version Control: Added merge options dialog to the merge view.

- Version Control: Added the ability to merge a branch or a changeset, using a new context menu actions.



## Changes

- Version Control: Automatically add UnityDirMonSyncFile rule for existing ignore.conf to avoid triggering unnecessary finding changes operation.

- Version Control: Improved the "search" edit box so it can resize when there is not enough space in the toolbar.

- Version Control: Optimized incoming changes to only reload the Package Manager when needed \(Gluon/partial workspace only for now\).

- Version Control: Optimized switching operations to only triggers the Package Manager to reinstall packages when needed.

- Version Control: Removed from the public documentation all internal APIs that were previously visible by mistake.

- Version Control: Removed support for migrating old Collaborate workspaces to Unity Version Control.

- Version Control: Replaced the "D" DevOps icon by the branching icon used in the Hub.

- Version Control: Replaced the logo of Unity in the Sign in to Unity VCS window.

- Version Control: Updated the minimum supported version to Unity 2021.3.0f1.

- XR: Updated xr.sdk.openxr package version to 1.13.1.

- XR: Updated xr.sdk.openxr package version to 1.13.2.



## Fixes

- 2D: Fixed Sprite broken Sprite references in TextureImporter when SpriteRect are defined outside of it's texture.
    (UUM-84276)

- Documentation: Updated ScriptableObject and ScriptableSingleton documentation.
    ([UUM-84568](https://issuetracker.unity3d.com/issues/you-may-not-pass-in-objects-that-are-already-persistent-error-is-thrown-when-calling-save-on-scriptablesingleton-inside-onvalidate))

- Editor: Export window maintains initial selection after selecting different items in the Project Browser.
    (UUM-82656)

- Editor: Fixed an issue where horizontal scrolling would not work when using a trackpad gesture.
    ([UUM-84867](https://issuetracker.unity3d.com/issues/light-explorer-window-cant-be-scrolled-horizontally-by-using-a-trackpad-gesture-when-there-is-no-vertical-scrollbar))

- Editor: Fixed bug where .meta files were copied to .xcframework folders in iOS builds.
    ([UUM-79113](https://issuetracker.unity3d.com/issues/ios-meta-files-within-a-xcframework-are-included-in-a-build))

- Editor: Fixed for Linux crash on right click in the middle of a window drag.
    ([UUM-82814](https://issuetracker.unity3d.com/issues/linux-crash-on-containerwindow-togglemaximize-when-clicking-rmb-while-moving-window-inside-the-editor))

- Editor: Fixed issues with world space canvases rendered in offscreen cameras when in play mode and with a user defined application target frame rate. These could display flickering with transparent canvas UI components or ghosting for moving components.
    ([UUM-86486](https://issuetracker.unity3d.com/issues/objects-flickering-in-play-mode-when-using-rendertexture-with-canvas))

- Editor: Fixed null ref exception when trying to maximize a pop-up window.
    ([UUM-76218](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-trying-to-maximize-view-in-anchor-presets-menu))

- Editor: Fixed some settings Asset icons that were missing in the selection window.
    ([UUM-83464](https://issuetracker.unity3d.com/issues/lighting-settings-asset-icon-is-missing-in-the-selection-window))

- Editor: Fixed where the asset icon selected in the Object Selector not initially showing up.
    ([UUM-83464](https://issuetracker.unity3d.com/issues/lighting-settings-asset-icon-is-missing-in-the-selection-window))

- Editor: Updated 7-Zip to 24.09.

- Graphics: Android Vulkan: Add transient usage flag while creating image even if lazily allocated memory is not available on the device.
    ([UUM-71363](https://issuetracker.unity3d.com/issues/android-vulkan-vk-image-usage-transient-attachment-bit-not-added-on-some-android-devices-in-com-dot-unity3d-dot-player-dot-unityplayeractivity-slash-2d-colour-attachement))

- Graphics: Fixed a problem with Texture Streaming where a material could remain blurry and not streamed in for an undefined amount of time.
    ([UUM-73384](https://issuetracker.unity3d.com/issues/the-material-variant-is-rendered-blurry-after-reopening-unity-when-the-mipmap-streaming-is-enabled))

- Graphics: Fixed an issue where "glClientWaitSync: Expected application to have kicked everything until job" error is spammed when disabling Raw Image.
    ([UUM-35986](https://issuetracker.unity3d.com/issues/android-opengl-glclientwaitsync-expected-application-to-have-kicked-everything-until-job-error-is-spammed-when-disabling-raw-image))

- Graphics: Fixed cases where drawing line primitives would draw triangles instead.
    ([UUM-66524](https://issuetracker.unity3d.com/issues/graphics-dot-renderprimitives-with-meshtopology-dot-lines-renders-triangles-when-the-shader-has-a-variable-with-position-semantic))

- iOS: Fixed plugin framework folders showing up red in exported iOS Xcode project.
    (UUM-84687)

- Mono: Fixed crash when mixed callstack debugging was enabled on non-windows platforms.
    ([UUM-16791](https://issuetracker.unity3d.com/issues/editor-crashes-on-startup-when-mixed-callstacks-diagnostics-switch-is-enabled))

- Package Manager: Fixed the issue where quick start button does not link to the document page for the current unity version.
    ([UUM-78210](https://issuetracker.unity3d.com/issues/quickstart-buttons-for-unity-registry-feature-sets-links-to-outdated-documentation))

- Scripting: Fixed early player loop overrides being reset to default when initialization is fully done.
    ([UUM-57619](https://issuetracker.unity3d.com/issues/playerloop-dot-setplayerloop-function-is-ignored-when-playing-game-in-player))

- Scripting: Fixed Update being called after the script is disabled in Start.
    ([UUM-72366](https://issuetracker.unity3d.com/issues/the-update-method-gets-called-on-a-disabled-script-when-added-and-disabled-during-runtime))

- Shadergraph: Fixed so that pasting an empty group positions it based on the cursor's location.
    (UUM-76254)

- Shaders: Fixed shader compiler crashing when encountering a kernel directive without a provided name.
    ([UUM-85898](https://issuetracker.unity3d.com/issues/internal-shader-error-is-shown-when-a-corrupted-shader-is-imported))

- SpeedTree: Fixed an issue where undo was not possible when the branch was rotated.
    ([UUM-82599](https://issuetracker.unity3d.com/issues/branch-rotation-cant-be-undone))

- UI Toolkit: UI Builder can now be open during a package reimport.
    ([UUM-77727](https://issuetracker.unity3d.com/issues/errors-are-thrown-when-using-the-at-import-directive-in-uss-files))

- URP: Fixed sorting the Reflection Probe by resolution.
    ([UUM-83862](https://issuetracker.unity3d.com/issues/error-type-is-not-a-enum-value-logged-when-ordering-reflection-probes-by-resolution-in-light-explorer))

- Version Control: Added a warning message to inform users about mismatching cloud project.

- Version Control: Fixed a crash in the create workspace window when unable to resolve a @unity organization.

- Version Control: Fixed files getting checked out even though they are in hidden_changes.conf.

- Version Control: Fixed incoming changes view that was not kept as selected after resolving some conflicts.

- Version Control: Fixed link to invite members in Unity Cloud.

- Version Control: Fixed manual login to Cloud that didn't work with an Enterprise installation.

- Version Control: Fixed new child branch not created from HEAD after update.

- Version Control: Fixed resolve conflicts not informing about lack of UVCS installation.

- Version Control: Fixed the Invite users to cloud organization when using an Enterprise installation.

- Version Control: Fixed the learn more \(here\) link that showed the hex color value in Unity 6.

- Version Control: Fixed workspace name that was not refreshed after repository manual creation or selection.

- Version Control: Removed from the Create Workspace window the Local server that was present with no installation of UVCS.

- Version Control: Replaced hardcoded urls pointing to plasticscm.com.

- WebGL: Fixed video playing issue in WebGL when another video is still loading in Firefox.
    ([UUM-79406](https://issuetracker.unity3d.com/issues/av1-videos-do-not-play-in-webgl-when-another-video-is-still-loading-and-firefox-browser-is-used))

- Windows: Fixed issue where changing the default icon is not refreshed by Windows Explorer when re-building a project into the same build folder used previously.
    ([UUM-71022](https://issuetracker.unity3d.com/issues/changing-the-default-icon-does-not-change-the-executables-icon-when-re-building-the-project))




## Package changes in 2021.3.47f1

## Packages updated

- com.unity.cinemachine: [2.10.1](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) to [2.10.3](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.collab-proxy: [2.5.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.5//changelog/CHANGELOG.html) to [2.6.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.6//changelog/CHANGELOG.html)

- com.unity.services.core: [1.12.5](https://docs.unity3d.com/Packages/com.unity.services.core@1.12//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.14//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.3.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.3//changelog/CHANGELOG.html) to [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.4//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.13.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.13//changelog/CHANGELOG.html) to [1.13.2](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.13//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk: [1.2.3](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.3//changelog/CHANGELOG.html)

- com.unity.microsoft.gdk.tools: [1.2.3](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.2//changelog/CHANGELOG.html) to [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.3//changelog/CHANGELOG.html)