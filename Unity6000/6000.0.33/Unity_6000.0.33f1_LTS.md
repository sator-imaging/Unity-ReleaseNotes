# Unity 6000.0.33f1 LTS
Published at Wed, 08 Jan 2025 10:15:44 GMT  
https://unity.com/releases/editor/whats-new/6000.0.33

# Known Issues in 6000.0.33f1

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- Audio Authoring: Audio Source clip is not audible when exceeding a high number of active Audio Sources
    ([UUM-91256](https://issuetracker.unity3d.com/issues/audio-source-clip-is-not-audible-when-exceeding-a-high-number-of-active-audio-sources))

- Build Settings Window: Application Cloud Connection Id is incorrect when using Build Profile with Player Setting Overrides.
    ([UUM-90426](https://issuetracker.unity3d.com/issues/application-cloud-connection-id-is-incorrect-when-using-build-profile-with-player-setting-overrides))

- Build Settings Window: The Editor spams the error message "Unexpected transport error from import worker 247. Code=2, error=End of file," causing the Asset Importer to crash
    ([UUM-82880](https://issuetracker.unity3d.com/issues/the-editor-spams-the-error-message-unexpected-transport-error-from-import-worker-247-code-equals-2-error-equals-end-of-file-causing-the-asset-importer-to-crash))

- DirectX12: Allocated graphics memory does not get released when the Editor is out of focus while using D3D12 graphics API
    ([UUM-86354](https://issuetracker.unity3d.com/issues/allocated-graphics-memory-does-not-get-released-when-the-editor-is-out-of-focus-while-using-d3d12-graphics-api))

- DirectX12: The Camera does not render correctly when the Camera.Rect() is changed and HDR is enabled and DX12 graphics API is selected
    ([UUM-86917](https://issuetracker.unity3d.com/issues/the-camera-does-not-render-correctly-when-the-camera-dot-rect-is-changed-and-hdr-is-enabled-and-dx12-graphics-api-is-selected))

- Editor Platform: Crash on OverridingParameterPreparer::OnPrepareVector when repeatedly saving changes made to a Shader Graph
    ([UUM-89067](https://issuetracker.unity3d.com/issues/crash-on-overridingparameterpreparer-onpreparevector-when-repeatedly-saving-changes-made-to-a-shader-graph))

- HDRP: Graphics Compositor breaks Unity rendering when the "Output Camera" is changed to a scene Camera and one Camera SubLayer is active.<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84610

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Packman: Unable to install ProBuilder package when project is located in an external FAT32/exFAT drive
    ([UUM-86351](https://issuetracker.unity3d.com/issues/unable-to-install-probuilder-package-when-project-is-located-in-an-external-fat32-slash-exfat-drive))

- Packman: [windows only] Switching Project when importing complete project does not import all assets and project opens incomplete
    ([UUM-88051](https://issuetracker.unity3d.com/issues/switching-project-when-importing-complete-project-does-not-import-all-assets-and-project-opens-incomplete))

- Scene Management: [MacOS] Crash on [NSApplication endModalSession:] when saving while Play Mode is loading
    ([UUM-87930](https://issuetracker.unity3d.com/issues/macos-crash-on-nsapplication-endmodalsession-when-saving-while-play-mode-is-loading))

- Scene View: Can not navigate through the Scene view when using a drawing tablet
    ([UUM-90436](https://issuetracker.unity3d.com/issues/can-not-navigate-through-the-scene-view-when-using-a-drawing-tablet))

- SpeedTree: This release of SpeedTree includes a change to the interface of the SpeedTree8Wind shadergraph node. If you have an animated SpeedTree in the shadergraph, be sure to connect an ObjectSpacePosition node to the input of the SpeedTree8Wind.  If the wind node does not have an input on the ObjectSpacePosition port, the mesh will be shrunk down to a point at origin \(making it seem to vanish\).<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84616

- Terrain: Trees do not render in 'Unity Terrain - URP Demo Scene'
    ([UUM-84616](https://issuetracker.unity3d.com/issues/trees-do-not-render-in-unity-terrain-urp-demo-scene))

- Text: Crash on tlsf_free when generating the Font Atlas
    ([UUM-91956](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-the-font-atlas))

- Text: Text is rendered with a different font when the "FallbackBoldItalic" font is selected
    ([UUM-87529](https://issuetracker.unity3d.com/issues/text-is-rendered-with-a-different-font-when-the-fallbackbolditalic-font-is-selected))

- Texture: Sprite Atlas Override for iOS setting remains disabled when saving its change to enabled
    ([UUM-90066](https://issuetracker.unity3d.com/issues/sprite-atlas-override-for-ios-setting-remains-disabled-when-saving-its-change-to-enabled))

- uGUI: TMP Input Field is moving Text and Caret UI positions for each new line when 'Auto Size' and 'Multi Line Newline' are used 
    ([UUM-89963](https://issuetracker.unity3d.com/issues/tmp-input-field-is-moving-text-and-caret-ui-positions-for-each-new-line-when-auto-size-and-multi-line-newline-are-used))

- Windows: Player remains in Windows Background processes when the application is closed
    ([UUM-87775](https://issuetracker.unity3d.com/issues/urp-player-remains-in-windows-background-processes-when-the-application-is-closed))



# 6000.0.33f1 Release Notes

## Improvements

- Serialization: Added -typeinfo to binary2text to allow debugging issues with corrupt type info in AssetBundles.



## Fixes

- Android: Bump Android Logcat Package to 1.4.4.

- Android: Fixed build failure problem when building AAB with Texture Compression targeting support using Clean Build option.
    (UUM-90997)

- Build System: The BEE_BUILD_THREADS environment variable has been extended to the Bee backend driver. This variable limits the maximum job count for Bee-based builds on your machine, user account, or session, preventing it from consuming all available CPU resources regardless of how builds are run.".

- Editor: Dont output compile errors when we automatically will retry the compilation, as they will be rerun and potentially fixed.
    (UUM-72688)

- Editor: Error messages in dialogs are no longer cut off when using high DPI monitors on MS Windows.
    ([UUM-87585](https://issuetracker.unity3d.com/issues/incomplete-warning-when-native-platform-backends-for-the-new-input-system-are-not-enabled))

- Editor: Fixed a crash is some Linux configurations where a notification from X11 can be raised before the application is initialized.
    ([UUM-91116](https://issuetracker.unity3d.com/issues/linux-crash-on-application-handleeditorfocuschange-when-opening-a-project-in-specific-environments))

- Editor: Fixed an issue where the TextureImporter "Alpha From Grayscale" and non-default Swizzle settings would have no effect when used with R16 grayscale source images.
    ([UUM-89039](https://issuetracker.unity3d.com/issues/unsupported-texture-format-r16-for-a-swizzle-error-and-texture-is-not-correctly-rendered-when-using-texture-swizzle-and-reimporting-texture-asset))

- Editor: Fixed C\# script imported leading to missing documentation.
    ([UUM-87334](https://issuetracker.unity3d.com/issues/c-number-script-help-button-leads-to-missing-documentation))

- Editor: Fixed help button tooltip text for some components.

- Editor: Fixed unable to parse build profile error.
    ([UUM-83673](https://issuetracker.unity3d.com/issues/unable-to-parse-file-error-is-thrown-when-opening-a-specific-project-with-custom-build-profiles))

- Editor: Removed faulty GlobalVolumeFeature renderer feature from the Mobile_Renderer asset in the blank URP template.
    ([UUM-84504](https://issuetracker.unity3d.com/issues/script-associated-with-globalvolumefeature-is-missing-when-inspecting-mobile-renderer-asset))

- Graphics: Fixed Reset of the default VolumeProfile in ProjectSettings &gt; Graphics.
    (UUM-77760)

- HDRP: HDRP Wizard do not show FixAll button anymore when no automated fix is available.
    ([UUM-84977](https://issuetracker.unity3d.com/issues/fix-all-button-does-not-disappear-after-applying-fixes-when-setting-up-dxr))

- IL2CPP: Fixed case where IL2CPP can allocate more memory than needed.
    ([UUM-83219](https://issuetracker.unity3d.com/issues/il2cpp-metadata-allocates-more-memory-when-testing-with-2022-dot-3-compared-to-2021-dot-3))

- Kernel: Optimized job system scheduling to scale better as thread count increases.
    (UUM-90028)

- Linux: Fixed mouse wheel input inversion on Legacy Input System and IMGUI.
    ([UUM-89968](https://issuetracker.unity3d.com/issues/linux-the-mouse-wheel-input-is-inverted-when-scrolling-in-the-build))

- Scripting: Added InstantiateParameters struct, this adds support for local space and target scenes to Object.InstantiateAsync.
    ([UUM-83002](https://issuetracker.unity3d.com/issues/cube-instantiated-by-the-instantiateasync-method-spawns-on-the-world-center-when-in-the-arguments-the-parent-is-passed-in))

- Scripting: Fixed an issue where multiple call to NextFrameAsync in edit mode within the same frame would cancel each other.
    ([UUM-86897](https://issuetracker.unity3d.com/issues/awaitable-dot-nextframeasync-fails-to-resume-when-invoked-multiple-times-from-the-playmodestatechanged-event))

- Serialization: Fixed serialized types with no namespace having their fields stripped.
    ([UUM-90913](https://issuetracker.unity3d.com/issues/the-player-crashes-when-there-are-unused-fields-in-serializereference-and-the-managed-stripping-level-is-set-to-medium-or-high))

- Shaders: Fixed implicit randomwrite shader requirement for compute shaders.
    (UUM-85545)

- Text: Added spacing properties to ATG.
    (UUM-90101)

- Text: Fixed ATG tab support.
    (UUM-87903)

- UI Toolkit: Added an error log to detect recursive SetParent calls that assign a VisualElement to a different parent.
    ([UUM-87366](https://issuetracker.unity3d.com/issues/user-is-not-notified-of-unsupported-behavior-nested-setparent))

- UI Toolkit: Enhanced USS Selector performance for numerous style sheets, in particular those with multiple wildcards and `:root` selectors.
    (UUM-91234)

- UI Toolkit: Fixed an issue where entering play mode could break dependencies between certain UXML files.
    ([UUM-90739](https://issuetracker.unity3d.com/issues/argumentexception-thrown-and-reference-to-template-gets-unset-when-opening-uxml-file-after-editing-referenced-template-in-play-mode))

- UI Toolkit: Fixed layout issues that sometimes occurred between scene changes.
    ([UUM-87950](https://issuetracker.unity3d.com/issues/ui-elements-shrinking-misaligned-buttons-swapped-icons-or-incorrect-styles-when-rapidly-cycling-through-scenes-in-the-player))

- UI Toolkit: Improved performance for layout in UITK.
    (UUM-90732)

- UI Toolkit: \[UI Builder\] Fixed Dropdown search icon is used next to the UI Builders Library search when the search has no dropdown functionality.
    ([UUM-90081](https://issuetracker.unity3d.com/issues/dropdown-search-icon-is-used-next-to-the-ui-builders-library-search-when-the-search-has-no-dropdown-functionality))

- Version Control: By default, the additional line breaks are not getting added to asset files when merging with UnityYAMLMerge with an extra option for user to get the line breaks.
    ([UUM-72934](https://issuetracker.unity3d.com/issues/additional-line-breaks-are-added-to-asset-files-when-merging-with-unityyamlmerge))

- Web: Fixed bug in `config.autoSyncPersistentDataPath` option in Unity Web.
    ([UUM-87753](https://issuetracker.unity3d.com/issues/webgl-typeerror-cannot-read-properties-of-undefined-reading-length-error-is-thrown-when-starting-the-player-when-config-dot-autosyncpersistentdatapath-is-set-to-true))

- WebGL: \[WebGPU\] Fix render error from shadergraph shaders with 3D textures.




## Package changes in 6000.0.33f1

## Packages updated

- com.unity.mobile.android-logcat: [1.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) to [1.4.4](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.performance.profile-analyzer: [1.2.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) to [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html)

- com.unity.recorder: [5.1.1](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) to [5.1.2](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- com.unity.services.economy: [3.5.0](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) to [3.5.1](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html)

- com.unity.services.leaderboards: [2.2.0](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.2//changelog/CHANGELOG.html) to [2.2.1](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.2//changelog/CHANGELOG.html)

- com.unity.xr.core-utils: [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.4//changelog/CHANGELOG.html) to [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)

- com.unity.xr.openxr: [1.13.2](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.13//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.xr.openxr@1.14//changelog/CHANGELOG.html)

- com.unity.multiplayer.playmode: [1.3.2](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.3//changelog/CHANGELOG.html) to [1.3.3](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.3//changelog/CHANGELOG.html)

- com.unity.dedicated-server: [1.3.2](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.3//changelog/CHANGELOG.html) to [1.3.3](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.3//changelog/CHANGELOG.html)