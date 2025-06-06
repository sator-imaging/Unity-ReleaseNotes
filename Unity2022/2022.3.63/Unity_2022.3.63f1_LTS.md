# Unity 2022.3.63f1 LTS
Published at Thu, 05 Jun 2025 08:33:00 GMT  
https://unity.com/releases/editor/whats-new/2022.3.63

# Known Issues in 2022.3.63f1

- DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when opening a project after changing the Graphics API to DirectX12
    ([UUM-77757](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-opening-a-project-after-changing-the-graphics-api-to-directx12))

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))

- DirectX12: The Player hangs when unloading a scene using the UnloadUnusedAssets() method
    ([UUM-79718](https://issuetracker.unity3d.com/issues/the-player-hangs-when-unloading-a-scene-using-the-unloadunusedassets-method))

- Graphics Device Features: Graphics.RenderMeshIndirect does not issue multi-draw rendering commands when using a graphics API capable of multi-draw commands
    ([UUM-91617](https://issuetracker.unity3d.com/issues/graphics-dot-rendermeshindirect-does-not-issue-multi-draw-rendering-commands-when-using-a-graphics-api-capable-of-multi-draw-commands))

- Lighting: Android Player freezes on some Mali GPU devices when Lighting Cast Shadows changed to OFF at runtime
    ([UUM-105246](https://issuetracker.unity3d.com/issues/android-player-freezes-on-some-mali-gpu-devices-when-lighting-cast-shadows-changed-to-off-at-runtime))

- Mono: Crash on scripting_method_invoke when the Player is build before entering the Play mode in the Editor
    ([UUM-108338](https://issuetracker.unity3d.com/issues/crash-on-scripting-method-invoke-when-the-player-is-build-before-entering-the-play-mode-in-the-editor))

- Mono: UnmanagedReadOrWrite objects are not disposed off when GZipStream is used in the "using" statement
    ([UUM-105139](https://issuetracker.unity3d.com/issues/unmanagedreadorwrite-objects-are-not-disposed-off-when-gzipstream-is-used-in-the-using-statement))

- OpenGL: [Linux] Crash on glXCreateGLXPixmap when hovering over labels in the Inspector window
    ([UUM-87106](https://issuetracker.unity3d.com/issues/linux-crash-on-glxcreateglxpixmap-when-hovering-over-labels-in-the-inspector-window))

- Packman: Editor crashes on "MonoBehaviour::Transfer<GenerateTypeTreeTransfer>" when resetting package defaults in VR Template project
    ([UUM-107869](https://issuetracker.unity3d.com/issues/editor-crashes-on-monobehaviour-transfer-when-resetting-package-defaults-in-vr-template-project))

- Scene Management: Editor hangs when cutting and pasting a Script to another folder during Play Mode
    ([UUM-104031](https://issuetracker.unity3d.com/issues/editor-hangs-when-cutting-and-pasting-a-script-to-another-folder-during-play-mode))

- Video: Editor crashes with PlatformWebCamTexture::GetDeviceNames when a Virtual Camera is present and FriendlyName property is deleted from Registry
    ([UUM-105563](https://issuetracker.unity3d.com/issues/editor-crashes-with-platformwebcamtexture-getdevicenames-when-a-virtual-camera-is-present-and-friendlyname-property-is-deleted-from-registry))



# 2022.3.63f1 Release Notes

## Features

- Version Control: Added to most dialogs an "Enter" keyboard shortcut to confirm the operation like the corresponding button.

- Version Control: Added to the check-in and shelve notification a link to go to the list of changesets/shelves. The user can also copy the direct diff link.

- Version Control: Added to the history a context action to diff changes for files that were moved/renamed.

- Version Control: Added to the history of a folder a context action to revert changes.

- Version Control: Added to the list of branches a context action to diff the branch.

- Version Control: Added to the list of branches a context action to hide branches. You can use the filter to list the hidden branches and unhide them from the context menu.

- Version Control: Added to the list of changesets a context action to create a new branch from a specific changeset.

- Version Control: Added to the merge operation a notification with a link to go to the pending changes.

- Version Control: Added to the merge view the avatars for authors of changes.

- Version Control: Added to the pending changes view the user avatar if available from Gravatar.

- Version Control: Added to the status bar an action to copy to the clipboard the name of the current branch.

- Version Control: Added to the undo and update workspace operations an ephemeral notification.



## Improvements

- Graphics: Improved CopyTexture documentation \(warning about using Apply, mentions of the readability property, and general improvements\).

- Graphics: Optimized Skinned Mesh Renderer matrix calculations to enable Unity to parallelize matrix calculations even when using the non-optimized import setting.
    (UUM-105251)



## Changes

- XR: Updated com.untiy.xr.openxr package version to 1.15.0-pre.2.



## Fixes

- 2D: Fixed hdr encoding and postprocess resolve for rendergraph 2d.
    ([UUM-105392](https://issuetracker.unity3d.com/issues/game-view-is-rendered-white-when-viewing-the-editor-with-hdr-display-and-post-proccesing-is-enabled-on-the-main-camera-with-2d-urp))

- 2D: Fixed Sprite Meta contains invalid internal ID during creation via TextureImporter.
    ([UUM-90488](https://issuetracker.unity3d.com/issues/ui-source-image-property-gets-set-to-none-when-using-a-specific-sprite-and-play-mode-is-entered))

- AI: The HeightMesh was sometimes containing faulty polygons that stretched between arbitrary vertices over long distances.
    ([UUM-78065](https://issuetracker.unity3d.com/issues/height-mesh-generation-results-in-unexpected-spikes-slash-streaks-across-the-whole-map-in-the-generated-navmesh-surface-when-re-baking))

- Android: Fixed issue preventing DXC from being used for Android Vulkan.

- Animation: Fixed an issue where undoing the creation of an AnimatorController layer while the layer view was not visible in the Animator Window would throw exceptions.
    ([UUM-104017](https://issuetracker.unity3d.com/issues/animator-controller-throws-missingreferenceexception-after-undoing-layer-creation))

- Audio: Fixed dsp stuck in one note loop when behaviour is disabled with OAFR.
    ([UUM-82219](https://issuetracker.unity3d.com/issues/audiolistener-is-stuck-on-a-single-audio-note-when-disabling-the-dsp))

- Editor: Avoid calling AnyTargetMaterialHasChildren \(which loads assets\) when deleting assets.
    ([UUM-79129](https://issuetracker.unity3d.com/issues/significant-time-is-taken-by-the-anytargetmaterialhaschildren-method-when-a-large-non-material-asset-is-deleted))

- Editor: Before running the macOS Editor, perform a check if Rosetta is installed and if not then prompt to install it.
    (UUM-104562)

- Editor: Editor can crash when playable graph topology is changed by an animation event callback.
    ([UUM-104081](https://issuetracker.unity3d.com/issues/crash-on-mecanim-animation-transformvaluesfromclip-when-entering-the-play-mode-in-a-project-with-animancer-pro-v8))

- Editor: Fixed a bug where the 'RectTransform' component values were set to NaN when scaling UI elements using the Scene Rect Tool.
    ([UUM-102690](https://issuetracker.unity3d.com/issues/rect-transform-values-are-set-to-nan-when-scaling-ui-element-with-centered-scaling))

- Editor: Fixed a bug whereby when evaluating an interrupted transition, the Animator writes the last evaluated values for all values instead of correctly defaulting to the state's current configuration.
    ([UUM-99493](https://issuetracker.unity3d.com/issues/all-animators-previous-animations-are-activated-while-transitioning-when-a-second-split-off-transition-overrides-the-first-split-off-transition))

- Editor: Fixed an issue where passing a long string label for a dialog box could cause an editor crash.
    ([UUM-90434](https://issuetracker.unity3d.com/issues/crash-on-editordisplaydialogproc-when-opening-dialog-box-containing-buttons-with-unusually-long-labels))

- Editor: Fixed dx12 crash when executing ReadPixelsWithInvalidActiveDepthSlice_ShouldNotCrash internal test.
    (UUM-69594)

- Editor: Fixed OverlayMenu behaviour when deleting or reverting presets.
    ([UUM-103066](https://issuetracker.unity3d.com/issues/when-reverting-all-presets-or-deleting-the-currently-chosen-preset-the-overlay-preset-is-not-switched-to-the-default-preset))

- Editor: Fixed some performance issues when moving Terrain objects \(eg. for shifting world origin to support large worlds\) while Tree rendering is disabled. Renderers for tree instances would still be updated but this is not particularly useful or wanted if you are using some other system to render Tree instances. So now the updating of tree instances is bypassed in this scenario. Re-enabling tree rendering will resume updating tree instance and detail renderers. When tree rendering is enabled, performance remains roughly the same as before.
    ([UUM-98086](https://issuetracker.unity3d.com/issues/frame-spike-due-to-many-treerenderer-dot-treeupdated-calls-when-repositioning-terrains-in-large-scenes))

- Editor: The icon for editor plugin settings now uses the correct icon when using the dark theme.
    (UUM-104115)

- GI: Converted the 'Failed to fallback to CPU lightmapper' error to a warning. Even when fallback from GPU lightmapper to CPU lightmapper fails, we don't want to break strict mode builds.
    (UUM-103390)

- GI: Fixed a bug where the unity_RendererBounds_Min and unity_RendererBounds_Max uniforms would be set to random uninitialized memory in the ShadowCaster pass.
    ([UUM-100264](https://issuetracker.unity3d.com/issues/shadows-flicker-and-cause-visual-artifacts-when-modifying-a-gameobjects-bounds-using-swizzle-y-mask-and-sine-time-nodes))

- Graphics: Corrected bounding box transformations in SkinnedMeshRenderer when "Update When Offscreen" is enabled and scaling is applied.
    ([UUM-69984](https://issuetracker.unity3d.com/issues/point-light-does-not-affect-skinnedmeshrenderer-when-its-deformed-has-update-when-offscreen-enabled-and-rendering-path-is-set-to-forward))

- Graphics: Fixed an issue where ASTC compression can have different results if called multiple times within the same process.
    ([UUM-96066](https://issuetracker.unity3d.com/issues/calling-texture2d-dot-getrawdata-on-a-texture-with-astc-format-returns-different-results-when-the-editor-is-started-without-library-folder-and-then-restarted-with-library-folder))

- Graphics: Fixed an issue where the value reported by "Texture.nonStreamingTextureMemory" would not update when mipmap limits were modified.
    ([UUM-79327](https://issuetracker.unity3d.com/issues/texture-dot-nonstreamingtexturememory-value-does-not-update-when-qualitysettings-dot-globaltexturemipmaplimit-is-changed))

- Graphics: Fixed glFramebufferTexture2DMultisampleEXT failure on Adreno drivers when per-format max MSAA limit exceeds global max MSAA limit.
    (UUM-76807)

- Graphics: Fixed infinite progress bar when converting PostProcess v2 from Built-in Render Pipeline to Universal Render Pipeline in the Converter.
    ([UUM-102790](https://issuetracker.unity3d.com/issues/editor-freezes-when-initializing-converters-with-post-processing-stack-v2-converter-enabled))

- Graphics: Fixed libGLES.so crash on small subset of PowerVR devices.
    (UUM-102249)

- Graphics: Fixed PowerVR GPUs crashing on GLES depth clear.
    ([UUM-103970](https://issuetracker.unity3d.com/issues/android-opengl-a-native-crash-on-gfxframebuffergles-clear-in-the-specific-project-when-using-powervr-gpus))

- HLSLcc: Fixed a bug where the int variable's data type was assumed to be a uint and not explicitly checked before attempting to be used with uintBitsToFloat.
    ([UUM-100116](https://issuetracker.unity3d.com/issues/compilation-errors-occur-when-uintbitstofloat-int-gets-used-in-opengles))

- IL2CPP: Fixed finalizers being called in a reentrant manner on the Web platform. Finalizers are now invoked explicitly at the end of each frame if needed.
    ([UUM-99176](https://issuetracker.unity3d.com/issues/native-code-called-abort-is-thrown-in-webgl-player-when-loading-first-scene))

- IL2CPP: Fixed incorrect exception handler generation when an exception handler with a filter throws an exception.
    ([UUM-91180](https://issuetracker.unity3d.com/issues/exception-block-is-being-rewritten-to-throw-an-incorrect-number-of-exceptions-when-running-a-project-built-using-il2cpp-scripting-backend))

- iOS: Fixed "Unexpected duplicate tasks" error when appending builds.
    ([UUM-104527](https://issuetracker.unity3d.com/issues/ios-xcode-project-building-fails-when-the-build-is-appended))

- iOS: Fixed a crash when loading achievements from GameCenter multiple times.
    ([UUM-105560](https://issuetracker.unity3d.com/issues/ios-application-frequently-crashes-on-social-dot-loadachievements-call-when-many-achievements-are-registered))

- iOS: Fixed errors when removing ODR variant in Player Settings.
    (UUM-103892)

- iOS: Fixed UI behavior when entering custom ODR variant settings in PlayerSettings.
    (UUM-103881)

- iOS: Fixed warning in the Xcode console when keyboard is open and changing orientation on iPad.
    (UUM-95530)

- Networking: Updated our version of MbedTLS to 3.6.3 to address possible security vulnerabilities.
    (UUM-103889)

- Package Manager: Make GetPatckagesPath thread/serialization safe.
    (UUM-104998)

- SRP Core: Fixed a memory leak when entering and leaving editor playmode.
    (UUM-104541)

- Terrain: Ensure that TreeRenderer position is initialized when creating Terrain camera render data.
    (UUM-104978)

- UI Elements: Assertion error thrown when discarding changes in builder.
    ([UUM-99290](https://issuetracker.unity3d.com/issues/assertion-error-is-thrown-when-discarding-the-changes-made-to-the-selectors-overriding-the-default-controls))

- UI Elements: Fixed a bug where some serialized fields were not always displayed in the inspector.
    (UUM-103578)

- URP: Fixed an issue that caused the empty shadowmap texture to not be properly cleared on console platforms.

- Version Control: Added the option to add a folder by path to the ignore or hidden changes list, instead of the incorrect option "Using the item extension".

- Version Control: Fixed a null exception that could occur on Revert to this revision if the selected change triggered a domain reload.

- Version Control: Fixed a null exception that could occur when switching to the changesets tab very quickly after checkin.

- Version Control: Fixed a null exception that occured when using the diff search filter without any shelve in the repository.

- Version Control: Fixed an error that was showing when deleting a shelveset that wasn't the one selected in the list.

- Version Control: Fixed bulk editing meta files that was only performing a single checkout for the last element.

- Version Control: Fixed false positive error showing in console if creating a workspace from the Hub with a version of the Unity Editor shipping with a default Version Control package older than version 2.7.1.

- Version Control: Fixed incorrect branch name in the history of a file for a revision where it was moved, displaying details of the move instead of the name of the branch.

- Version Control: Fixed merge success notification that was showing in the view potentially colliding with contents.

- Version Control: Fixed project download from the Hub that was silently skipped when trying to download inside another workspace. It's now logging an explicit error in the console.

- Version Control: Fixed the apply shelve operation so that it checks for dirty changes and warn the user before applying the shelve.

- Version Control: Fixed the auto checkout for assets to only apply for file containing actual changes.

- Version Control: Fixed the scroll that was not at the top when opening the branches or the shelves view.

- Version Control: Fixed the UI that could start refreshing forever, never completing the ongoing operations.

- Version Control: Fixed the Unity Editor crashing on macOS when opening the Unity Version Control window with the PiXYZ Plugin installed.

- Version Control: Fixed Undo changes of a Moved asset using the Asset Context Menu from the Project View that was leaving an inconsistent .meta file.

- Version Control: Implemented a mechanism to fix the path to UnityYAMLMerge.exe in the client.conf so it always points to an existing Unity installation.

- Web: Fixed a bug where rapid touch inputs could caused performance degradation.
    ([UUM-26629](https://issuetracker.unity3d.com/issues/a-webgl-build-with-complex-shaders-has-a-performance-drop-when-tapping-the-screen))

- Web: Fixed handling of multiple touch inputs and the computation of Touch.deltaPostion and Touch.deltaTime.
    ([UUM-83348](https://issuetracker.unity3d.com/issues/touch-input-is-inversed-and-otherwise-broken-on-a-touch-screen-monitor-when-a-project-is-built-for-webgl))

- Web: Fixed the diagnostic overlay to be available for PWA and minimal Web template builds.
    ([UUM-103203](https://issuetracker.unity3d.com/issues/the-web-diagnostics-overlay-only-works-with-the-default-template))

- Windows: Fixed for saving corrupted PlayerPrefs when application is closed when out of focus.
    ([UUM-100970](https://issuetracker.unity3d.com/issues/playerprefs-get-corrupted-when-a-minimized-fullscreen-player-is-closed-through-the-taskbar))

- XR: Fixed issue where Quest Link would fail when using DX12 and single pass rendering.




## Package changes in 2022.3.63f1

## Packages updated

- com.unity.collab-proxy: [2.7.1](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.7//changelog/CHANGELOG.html) to [2.8.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.8//changelog/CHANGELOG.html)

- com.unity.scriptablebuildpipeline: [1.21.25](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.21//changelog/CHANGELOG.html) to [1.22.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.22//changelog/CHANGELOG.html)

- com.unity.splines: [2.8.0](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) to [2.8.1](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)

- com.unity.netcode.gameobjects: [1.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.12//changelog/CHANGELOG.html) to [1.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.13//changelog/CHANGELOG.html)

- com.unity.polyspatial: [1.3.12](https://docs.unity3d.com/Packages/com.unity.polyspatial@1.3//changelog/CHANGELOG.html) to [1.3.13](https://docs.unity3d.com/Packages/com.unity.polyspatial@1.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.visionos: [1.3.12](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@1.3//changelog/CHANGELOG.html) to [1.3.13](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@1.3//changelog/CHANGELOG.html)

- com.unity.polyspatial.xr: [1.3.12](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@1.3//changelog/CHANGELOG.html) to [1.3.13](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@1.3//changelog/CHANGELOG.html)

- com.unity.xr.visionos: [1.3.12](https://docs.unity3d.com/Packages/com.unity.xr.visionos@1.3//changelog/CHANGELOG.html) to [1.3.13](https://docs.unity3d.com/Packages/com.unity.xr.visionos@1.3//changelog/CHANGELOG.html)