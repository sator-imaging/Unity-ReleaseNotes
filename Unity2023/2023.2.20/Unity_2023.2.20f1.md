# Unity 2023.2.20f1
Thu, 25 Apr 2024 19:29:55 GMT  
https://unity.com/releases/editor/whats-new/2023.2.20

### Known Issues in 2023.2.20f1

- Asset - Database: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene
    ([UUM-66207](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-openasset-because-assertion-fails-on-prefabinstance-dot-getrootgameobject-dot-isvalid-expression-while-opening-a-specific-scene))

- Audio Authoring: Crash on AudioUtil_CUSTOM_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached
    ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))

- IL2CPP: [Android] Crash on Android when AndroidJavaProxy is calling from multiple threads
    ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))

- Lighting: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning
    ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))

- Platform Audio: Crash on FMOD::CodecMPEG::setPositionInternal when a mobile platform is selected and a specific audio clip is played
    ([UUM-62086](https://issuetracker.unity3d.com/issues/crash-on-fmod-codecmpeg-setpositioninternal-when-a-mobile-platform-is-selected-and-a-specific-audio-clip-is-played))

- WebRequest: UnityWebRequest crashes if invoked when player is quitting
    ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))



### 2023.2.20f1 Release Notes

#### Improvements

- Android: Switched to GameActivity 3.0.0 package.



#### Fixes

- 2D: Fixed unable to create Sprite in Sprite Editor Window in certain cases.
    ([UUM-67197](https://issuetracker.unity3d.com/issues/sprite-editor-does-not-allow-creating-new-sprite-tiles-in-a-sprite-sheet-with-a-specific-name))

- Accessibility: Fixed an issue where accessibility frame is shifted when "render outside safe area" is unchecked.
    (UUM-63896)

- Android: Fixed an issue where the back button did not correctly close TouchScreenkeyboard with GameActivity.
    (UUM-37017)

- Android: Fixed an issue where TouchScreenkeyboard type for GameActivity, previously it was stuck on text keyboard even though Numerical keyboard was requested.
    (UUM-43150)

- Android: Fixed issue where TouchScreenkeyboard couldn't be reopened with GameActivity once closed via Navigational button.
    (UUM-31651)

- Android: Fixed issue where TouchScreenkeyboard would act as multiline, even though multiline was not requested, this happens with GameActivity.
    ([UUM-65277](https://issuetracker.unity3d.com/issues/ui-toolkit-android-text-field-becomes-multiline-during-edition-in-the-player-when-the-multiline-option-is-disabled-in-the-ui-document-texfield-settings))

- Android: Fixed logic for overriding builtin java file, Unity will also now respect package name inside java file. Previously the logic was driven only by java file name.
    ([UUM-67826](https://issuetracker.unity3d.com/issues/android-cannot-find-symbol-public-class-unityplayeractivity-extends-com-dot-unity3d-dot-player-dot-unityplayeractivity-error-is-thrown-when-building-for-the-android-platform))

- Asset Bundles: Fixed performance regression when clearing bundle cache folders.
    ([UUM-60063](https://issuetracker.unity3d.com/issues/long-load-times-when-large-asset-bundles-are-discarded))

- Audio: Fixed an issue that would cause the transport buttons in the ARC editor window to be displayed wrongly after the window is focused.
    ([UUM-66290](https://issuetracker.unity3d.com/issues/preview-transport-controls-of-the-audio-random-container-dont-update-on-tab-switching))

- Audio: Fixed an issue that would cause Unity to crash when you manually destroy a streamed audio clip.
    ([UUM-14330](https://issuetracker.unity3d.com/issues/crash-on-purecall-when-repeatedly-creating-playing-stopping-and-deleting-audio))

- Audio: Fixed AudioMixer.SetFloat not working correctly on assets loaded from an asset bundle in play mode in the editor.
    ([UUM-68181](https://issuetracker.unity3d.com/issues/audio-mixer-does-not-change-volume-when-lowering-volume-on-an-audio-mixer-loaded-from-assetbundles))

- Core: Fixed floating point issue in APV sampling.
    ([UUM-47714](https://issuetracker.unity3d.com/issues/white-pixel-fragments-and-spots-randomly-appear-and-flicker-when-a-specific-reflection-probe-is-enabled))

- Documentation: Fixed EditorUtility.OpenFilePanelWithFilters documentation.
    (UUM-44679)

- Documentation: Fixed EditorUtility.SetDialogOptOutDecision documentation.
    (UUM-43878)

- Editor: Changed the behaviour of the slider range trackers in the Audio Random Container window, so that they're greyed out when randomisation is disabled.
    ([UUM-55692](https://issuetracker.unity3d.com/issues/sliders-yellow-randomization-indicators-are-shown-when-randomization-is-turned-off))

- Editor: Disable minimise if the Windows general Preference "Show All Windows in Taskbar" is unchecked to work around a MS Windows limitation.
    ([UUM-63821](https://issuetracker.unity3d.com/issues/undocked-editor-windows-do-not-have-name-labels-when-minimized))

- Editor: Fixed a crash when entering and leaving play mode while UnityWebRequest is downloading texture using DownloadHandlerTexture.
    (UUM-68555)

- Editor: Fixed an issue where the ObjectPool counter returned wrong count if returning instance to full pool.
    ([UUM-49060](https://issuetracker.unity3d.com/issues/wrong-number-is-returned-when-using-target-dot-pool-dot-countactive-in-objectpool-if-objects-are-destroyed))

- Editor: Fixed crash of an import worker process during asset importing which results in "Unexpected transport error from import worker 0" error in the Editor log
    ([UUM-64341](https://issuetracker.unity3d.com/issues/unexpected-transport-error-from-import-worker-0-error-is-thrown-when-importing-an-asset))

- Editor: Fixed Drag and Drop changing order when reparenting multiple gameobjects.
    (UUM-67905)

- Editor: Fixed flickering when using baked gi node and TAA.
    ([UUM-65682](https://issuetracker.unity3d.com/issues/hd-rp-shader-graph-with-a-baked-gi-node-flickers-when-probe-volumes-and-taa-are-enabled))

- Editor: Fixed for an AMD crash when using virtual offset computation in APV.
    ([UUM-59522](https://issuetracker.unity3d.com/issues/amd-crash-on-gfxdeviced3d12base-drawbufferscommon-when-baking-light-with-virtual-offset-on-probe-volumes))

- Editor: Fixed issue where dialog box with a progress bar can cause a crash when entering play mode on macOS.
    ([UUM-66854](https://issuetracker.unity3d.com/issues/crash-on-overridingparameterpreparer-onpreparevector-when-entering-play-mode))

- Editor: Removed "Autofill" menu item from the "Edit" menu.
    ([UUM-62774](https://issuetracker.unity3d.com/issues/autofill-menu-item-is-presented-in-edit))

- Editor: Removed "Close All" menu item from the "File" menu.
    (UUM-65192)

- Graphics: Fixed a rare crash that can happen when using procedural geometries \(intersections shaders\) in ray tracing effects.
    ([UUM-68610](https://issuetracker.unity3d.com/issues/crash-on-nvdev-thunk-when-using-directx12))

- Graphics: Fixed artifacts along the borders of a texture with transparency when the legacy ETC compressor is used.
    ([UUM-65381](https://issuetracker.unity3d.com/issues/ui-texture-is-rendered-with-artifacts-when-etc-compressor-is-set-to-legacy-and-the-texture-format-is-set-to-rgba-compressed-etc2-8-bits))

- Graphics: Fixed screen flickering when depth/stencil is disabled in player settings and graphics API is set to Vulkan.
    ([UUM-66721](https://issuetracker.unity3d.com/issues/android-graphics-the-screen-is-flickering-or-the-player-crashes-after-rotating-the-device-when-disable-depth-and-stencil-is-enabled-and-graphics-api-is-set-to-vulkan))

- HDRP: Fixed a Banding in IES importer issue.
    (UUM-68033)

- HDRP: Fixed a scaling issue with the recorder.
    ([UUM-58379](https://issuetracker.unity3d.com/issues/hdrp-recorder-crops-the-view-of-images-and-videos-when-recording-a-targeted-camera-with-dynamic-resolution-enabled))

- HDRP: Fixed cinematic eye shader lighting from directional lights.
    ([UUM-65500](https://issuetracker.unity3d.com/issues/eye-shader-lighting-depends-on-world-position-when-using-eyecinematic-material-type))

- HDRP: Fixed HDRP clouds \(volumetrics and background\) not being affected by main directionnal light intensity multiplier.
    (UUM-68313)

- HDRP: Fixed invalid AABB errors in some other cases.
    ([UUM-69928](https://issuetracker.unity3d.com/issues/invalid-aabb-inaabb-errors-still-happening-in-some-projects))

- HDRP: Fixed Move water specific global shader variables to separate file.
    ([UUM-68132](https://issuetracker.unity3d.com/issues/hdrp-water-is-leaking-uniforms))

- HDRP: Fixed realloc of history buffer when XR was enabled.
    ([UUM-41386](https://issuetracker.unity3d.com/issues/quest-2-xr-plugin-management-the-physically-based-sky-and-volumetric-clouds-are-rendered-only-for-the-left-eye-when-xr-is-initialized-manually))

- HDRP: Fixed TAA post sharpen in XR.
    ([UUM-32872](https://issuetracker.unity3d.com/issues/xr-only-1-eye-is-rendered-when-single-pass-instanced-and-taa-post-sharpen-is-used))

- iOS: Fixed UnityWebRequest URLs with unescaped symbols \[ and \] in query and containing other spec characters like space will now fail on iOS 17 instead of sending request to improperly escaped \(and as such - wrong\) url. URLs that are properly percent-escaped are recommended and will work correctly.
    (UUM-66942)

- License: Don't exit play-mode when another project is being created \(using Unity Hub 3.8.0-beta.1\)
    ([UUM-68141](https://issuetracker.unity3d.com/issues/editor-exits-play-mode-when-another-project-is-being-created-using-unity-hub-3-dot-8-0-beta-dot-1))

- Linux: In our Linux Pulse audio driver, make sure to select the correct default output device. Previously, on some systems and some versions of Linux, we could end up with no audio output or audio output being routed to an unexpected device.
    ([UUM-53143](https://issuetracker.unity3d.com/issues/linux-no-audio-output-when-playing-audio))

- macOS: Fixed custom cursor not used if mouse leaves the window.
    ([UUM-67592](https://issuetracker.unity3d.com/issues/cursor-does-not-switch-back-to-the-custom-cursor-when-the-mouse-is-moved-back-into-the-player-window-on-macos))

- Mono: Fixed InvalidProgramException \(Invalid IL code in \(wrapper managed-to-native\) &lt;METHOD&gt;: IL_0004: ldloc     65535\)getting thrown when calling COM interop methods.
    ([UUM-62035](https://issuetracker.unity3d.com/issues/windows-com-throws-the-invalidprogramexception-when-using-ookii-dot-dialogs-library))

- Mono: Fixed issue where incorrect TimeZones would be returned on some devices due to an exception being thrown.
    ([UUM-67254](https://issuetracker.unity3d.com/issues/mobile-timezone-dot-currenttimezone-returns-utc-0-when-peru-time-zone-5-utc-is-set-on-mobile-devices))

- Package: Undo the Vuforia deprecation.
    ([UUM-65386](https://issuetracker.unity3d.com/issues/package-manager-com-dot-ptc-dot-vuforia-dot-engine-is-deprecated-this-package-is-no-longer-supported-on-this-editor-version-warning-appears-when-vuforia-engine-package-is-imported))

- Prefabs: Fixed a crash on PhysicsManager::SetBodyTransformChangeInterest when opening a scene.
    ([UUM-56057](https://issuetracker.unity3d.com/issues/crash-on-physicsmanager-setbodytransformchangeinterest-when-opening-a-scene))

- Search: Fixed GUIStyle error when installing/uninstalling a package.
    ([UUM-65607](https://issuetracker.unity3d.com/issues/unable-to-use-a-named-guistyle-without-a-current-skin-error-appears-when-installing-slash-uninstalling-a-package-if-the-search-window-has-any-text-in-the-search-field))

- UI Toolkit: Fixed dynamic height TreeView does not refresh when resizing.
    ([UUM-54787](https://issuetracker.unity3d.com/issues/visual-effects-graph-treeview-does-not-refresh-when-resizing-undocked-vfx-template-window))

- UI Toolkit: Fixed Inspector sometimes becoming black when displaying nested lists.
    ([UUM-69458](https://issuetracker.unity3d.com/issues/nested-lists-in-scriptable-objects-crash-the-inspector-and-the-assertion-failed-console-error-appears-when-expanding-an-empty-nested-list-in-the-inspector))

- UI Toolkit: Fixed InvalidOperationException sometimes thrown when calling property.NextVisible in a CustomPropertyDrawer's CreatePropertyGUI.
    ([UUM-12851](https://issuetracker.unity3d.com/issues/propertydrawer-throws-an-exception-when-iterating-over-the-createpropertygui-serializedproperty))

- UI Toolkit: Fixed justify-content doesn't align content properly when min-width is used with borders or padding on the parent.
    ([UUM-19900](https://issuetracker.unity3d.com/issues/justify-content-doesnt-align-content-properly-when-min-width-is-used-with-borders-in-ui-toolkit))

- UI Toolkit: Fixed large memory allocation sometimes happening when processing style variables.
    (UUM-69741)

- UI Toolkit: Fixed renaming not working when changing selection.
    (UUM-62652)

- UI Toolkit: Fixed rendering of UI Toolkit when using LLVMpipe.
    ([UUM-68128](https://issuetracker.unity3d.com/issues/the-scene-toolbar-is-not-rendered-in-the-ubuntu-editor-when-using-nvidia-a100-tensor-core-gpu))

- UI Toolkit: Fixed UI Builder Spacing/Border widgets are missing labels.
    ([UUM-68447](https://issuetracker.unity3d.com/issues/ui-builder-spacing-slash-border-widgets-are-missing-labels))

- UI Toolkit: Fixed UIDocument component not showing on some Inspector windows when multiple inspectors are open.
    (UUM-67033)

- UI Toolkit: Make the label of any BaseField elided with ellipsis when needed.
    ([UUM-42121](https://issuetracker.unity3d.com/issues/variable-name-overlaps-range-slider-in-inspector-window-when-having-a-long-variable-name-and-a-range-attribute))

- Undo System: Fixed crash when undoing an action in a graph using Undo.RecordObject.
    (UUM-58380)

- Universal RP: Fixed an issue where the built in error shader didn't work correctly with depth priming.
    ([UUM-62825](https://issuetracker.unity3d.com/issues/error-shaders-not-visible-when-depth-priming-is-enabled))

- Universal RP: Fixed broken setting shadow rendering layer is not changing shadow when using shadowRenderingLayers in the script.
    ([UUM-28061](https://issuetracker.unity3d.com/issues/setting-shadow-rendering-layer-is-not-changing-shadow-when-using-shadowrenderinglayers-in-the-script))

- URP: Fixed an issue where Runtime intensity of non real-time reflection probes were not immediately reflected in scene view.
    ([UUM-67982](https://issuetracker.unity3d.com/issues/urp-changes-to-the-intensity-of-reflectionprobe-are-not-immediately-reflected-when-using-forward-plus))

- VFX Graph: Fixed an issue where selected gizmo for nodes with multiple gizmos \(for instance: Set Position Sequential Line\) did not change.
    (UUM-52509)

- VFX Graph: Fixed gizmo overlay's drop down was cut at the bottom.
    ([UUM-48125](https://issuetracker.unity3d.com/issues/visual-effects-overlay-menu-additional-item-description-and-blue-selection-indicator-is-not-fully-visible))

- Video: Fixed an issue where Playback becomes erratic in web browsers upon losing and regaining browser focus.
    ([UUM-63591](https://issuetracker.unity3d.com/issues/webgl-video-playback-becomes-erratic-in-web-browsers-upon-losing-and-regaining-browser-focus))

- Video: Fixed an issue where VideoPlayer support of multiple audio tracks was broken on a few platforms.
    (UUM-55268)

- Video: Fixed the Video Player to play the video after seeking back to frame 0 when Loop and Skip On Drop are enabled and the video has looped once.
    ([UUM-66728](https://issuetracker.unity3d.com/issues/the-video-player-does-not-play-the-video-after-seeking-back-to-frame-0-when-loop-and-skip-on-drop-are-enabled-and-the-video-has-looped-once))

- Video: Video repeats the first frame on Android when it is played via Unity's Video Player component.
    ([UUM-45914](https://issuetracker.unity3d.com/issues/android-video-repeats-the-first-frame-on-android-when-it-is-played-via-unitys-video-player-component))

- WebGL: Fixed spatial blend implementation to enable 2D/3D audio ratio.
    ([UUM-57740](https://issuetracker.unity3d.com/issues/audio-source-spatial-blend-value-gets-set-to-1-in-the-webgl-player-when-the-spatial-blend-value-is-bigger-than-0))

- XR: Fixed an issue where, if the render pass count was greater than 0 SPI would use the proper one instead of always using 0.
    ([UUM-57876](https://issuetracker.unity3d.com/issues/birp-getscriptablecullingparameters-uses-the-wrong-projection-matrix-when-rendering-two-forward-plus-passes-in-xr))




#### Package changes in 2023.2.20f1

#### Packages updated

- com.unity.2d.psdimporter: [9.0.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.0//changelog/CHANGELOG.html) &#x2192; [9.0.3](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.0//changelog/CHANGELOG.html)

- com.unity.2d.spriteshape: [10.0.3](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html) &#x2192; [10.0.4](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html)

- com.unity.cinemachine: [2.9.5](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.9//changelog/CHANGELOG.html) &#x2192; [2.10.0](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat: [1.4.0](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) &#x2192; [1.4.1](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.services.cloud-diagnostics: [1.0.6](https://docs.unity3d.com/Packages/com.unity.services.cloud-diagnostics@1.0//changelog/CHANGELOG.html) &#x2192; [1.0.7](https://docs.unity3d.com/Packages/com.unity.services.cloud-diagnostics@1.0//changelog/CHANGELOG.html)

- com.unity.rendering.light-transport: [1.0.1](https://docs.unity3d.com/Packages/com.unity.rendering.light-transport@1.0//changelog/CHANGELOG.html) &#x2192; [1.0.2](https://docs.unity3d.com/Packages/com.unity.rendering.light-transport@1.0//changelog/CHANGELOG.html)

- com.unity.services.authentication: [3.3.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.3//changelog/CHANGELOG.html) &#x2192; [3.3.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.3//changelog/CHANGELOG.html)

- com.unity.services.core: [1.12.4](https://docs.unity3d.com/Packages/com.unity.services.core@1.12//changelog/CHANGELOG.html) &#x2192; [1.12.5](https://docs.unity3d.com/Packages/com.unity.services.core@1.12//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.3.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.3//changelog/CHANGELOG.html) &#x2192; [1.4.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.4//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [2.5.2](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.5//changelog/CHANGELOG.html) &#x2192; [2.5.4](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.5//changelog/CHANGELOG.html)

- com.unity.dt.app-ui: [1.0.2](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.0//changelog/CHANGELOG.html) &#x2192; [1.0.3](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.0//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.services.vivox@16.2.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.2//changelog/CHANGELOG.html)