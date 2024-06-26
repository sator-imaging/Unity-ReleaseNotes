# Unity 2023.2.17f1
Thu, 04 Apr 2024 01:45:09 GMT  
https://unity.com/releases/editor/whats-new/2023.2.17

### Known Issues in 2023.2.17f1

- Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode
    ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))

- Asset - Database: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene
    ([UUM-66207](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-openasset-because-assertion-fails-on-prefabinstance-dot-getrootgameobject-dot-isvalid-expression-while-opening-a-specific-scene))

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

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- License: Editor exits Play mode when another project is being created using Unity Hub 3.8.0-beta.1
    ([UUM-68141](https://issuetracker.unity3d.com/issues/editor-exits-play-mode-when-another-project-is-being-created-using-unity-hub-3-dot-8-0-beta-dot-1))

- Metal: Player hangs when re-focusing the Player window after switching to a window that covers the Player window
    ([UUM-67400](https://issuetracker.unity3d.com/issues/player-hangs-when-re-focusing-the-player-window-after-switching-to-a-window-that-covers-the-player-window))

- Metal: [iOS] App crashes with out of memory exception in UnityGfxDeviceWorker when starting the app
    ([UUM-55488](https://issuetracker.unity3d.com/issues/ios-app-crashes-with-out-of-memory-exception-in-unitygfxdeviceworker-when-starting-the-app))

- Platform Audio: Crash on FMOD::CodecMPEG::setPositionInternal when a mobile platform is selected and a specific audio clip is played
    ([UUM-62086](https://issuetracker.unity3d.com/issues/crash-on-fmod-codecmpeg-setpositioninternal-when-a-mobile-platform-is-selected-and-a-specific-audio-clip-is-played))

- Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning
    ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))

- RP Foundation: Stacked camera is not rendering when using custom post effects is done in PreRender PostRender and Camera is not in HDR
    ([UUM-22444](https://issuetracker.unity3d.com/issues/ios-stacked-camera-is-not-rendering-when-using-custom-post-effects-and-build-target-is-set-to-ios))

- Text: Blurry Text
    ([UUM-49006](https://issuetracker.unity3d.com/issues/blurry-text))

- Text: Crash on invalid_parameter_internal when entering Play Mode
    ([UUM-68490](https://issuetracker.unity3d.com/issues/crash-on-invalid-parameter-internal-when-entering-play-mode))

- WebRequest: UnityWebRequest crashes if invoked when player is quitting
    ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))



### 2023.2.17f1 Release Notes

#### Features

- Package: Adds Apple privacy manifest in moderation package.



#### Improvements

- Editor: Throw a warning when RenderPipelineAsset.renderPipelineShaderTag hasn't been overriden.
    ([UUM-61556](https://issuetracker.unity3d.com/issues/shaders-are-not-rendered-properly-after-blitting-in-player-when-creating-a-custom-render-pipeline-based-on-urp))

- VisionOS: Add support for Burst with the VisionOS simulator SDK. This requires Burst version 1.8.13.



#### Fixes

- 2D: Fixed flickering for 2D Renderer on macOS silicon.
    (UUM-67306)

- Android: Fixed an issue where a black frame flashes when returning to Unity Game Activity from the home screen.
    ([UUM-58966](https://issuetracker.unity3d.com/issues/android-a-black-frame-flashes-when-returning-to-the-unity-game-activity-from-the-home-screen))

- Android: Fixed issue with updating the minimum value of maxAspectRatio value.
    (UUM-66208)

- Asset Pipeline: Fixed crash loading Content Archive from different version.
    ([UUM-64609](https://issuetracker.unity3d.com/issues/crash-when-loading-content-archive-from-a-different-unity-version))

- Audio: Fixed AudioRandomContainer crash after domain reload and playing an audiosource in edit mode.
    ([UUM-60125](https://issuetracker.unity3d.com/issues/crash-triggering-arc-in-edit-mode))

- Audio: Fixed AudioRandomContainer crash after domain reload if scene reloading disabled / already in playmode.
    ([UUM-63433](https://issuetracker.unity3d.com/issues/crash-on-audioplayableoutput-settargetaudiosource-when-enabling-the-audio-source-component-in-play-mode-enter-play-mode-options-is-enabled-and-audio-source-has-its-audio-resource-set-as-an-audio-random-container))

- Editor: Capitalize the compiler generated name of serialized field.
    ([UUM-45789](https://issuetracker.unity3d.com/issues/applying-the-serializefield-attribute-to-the-field-generated-by-the-property-doesnt-capitalize-it-in-the-inspector))

- Editor: Fixed a crash on BucketAllocator::Allocate when entering Play mode.
    ([UUM-65101](https://issuetracker.unity3d.com/issues/crash-on-bucketallocator-allocate-when-entering-play-mode))

- Editor: Fixed an error in the calculation of the available space for the children when min/max were involved and margin were set on the parent.
    ([UUM-29965](https://issuetracker.unity3d.com/issues/borders-of-an-element-dont-match-its-childrens-borders-when-the-element-has-max-width-specified))

- Editor: Fixed an issue where Joint components would never wake up ArticulationBody components, when the constraint data was changed.
    ([UUM-64395](https://issuetracker.unity3d.com/issues/changes-on-configurablejoint-dont-apply-when-the-rigidbody-has-fallen-asleep))

- Editor: Fixed an issue where Joint components wouldn't properly wake up Rigidbody components, when the constraint data was changed.
    ([UUM-64395](https://issuetracker.unity3d.com/issues/changes-on-configurablejoint-dont-apply-when-the-rigidbody-has-fallen-asleep))

- Editor: Fixed an issue with context menu in scene hierarchy when multiple objects are selected.

- Editor: Fixed an opening style tag overflow issue.
    ([UUM-30205](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-index-was-outside-the-bounds-of-the-array-error-when-selecting-text))

- Editor: Fixed crash in FBX importer when importing Blender file.
    ([UUM-63758](https://issuetracker.unity3d.com/issues/crash-on-convertblendertofbx-while-importing-a-specific-blend-file))

- Editor: Fixed issue with GUI.skin.font not being applied properly.
    ([UUM-65857](https://issuetracker.unity3d.com/issues/text-font-doesnt-change-in-play-mode-when-using-gui-dot-skin-dot-font))

- Editor: Fixed issue with incorrect font size when renaming an asset.
    ([UUM-66104](https://issuetracker.unity3d.com/issues/font-of-file-name-in-renaming-mode-expands-in-project-view))

- Editor: Fixed issue with overriden prefab field not being bold.
    ([UUM-61084](https://issuetracker.unity3d.com/issues/overriden-prefab-field-text-in-the-inspector-window-is-not-bold-when-the-prefab-has-overridden-fields))

- Editor: Fixed LOD Group Cross Fade effect does not function when the GameObject is dynamically loaded.
    ([UUM-65463](https://issuetracker.unity3d.com/issues/lod-group-cross-fade-effect-is-not-working-when-the-gameobject-is-loaded-dynamically))

- Editor: Fixed unrelated Objects/Metadata that showed up assigned to samples in the CPU Timeline view and were repeating the data from the last sample in the thread &amp; frame that had valid Object/Metadata information associated with it.
    ([UUM-66592](https://issuetracker.unity3d.com/issues/unrelated-objects-slash-metadata-are-assigned-to-samples-past-the-last-one-with-valid-object-slash-metadata-information-as-observed-in-cpu-usage-timeline))

- Editor: Updated the FBX SDK version to 2020.3.4.
    ([UUM-60185](https://issuetracker.unity3d.com/issues/silicon-modelimporter-dot-import-takes-a-long-time-when-opening-a-project-in-batch-mode))

- Graphics: Fixed a crash in Mesh bounds recalculation when not enough vertices are assigned to the mesh for each sub-mesh.
    ([UUM-5812](https://issuetracker.unity3d.com/issues/crash-on-mesh-recalculatebounds-when-assigning-not-enough-vertices-for-two-submeshes))

- HDRP: Fixed game view flicker while on HDR and Reflection probe.
    ([UUM-64343](https://issuetracker.unity3d.com/issues/the-game-view-flickers-on-play-mode-when-using-reflection-probe-and-hdr-display))

- HDRP: HDRP: Fixed invalid AABB error in the console when using the APV with reflection probes.
    ([UUM-64617](https://issuetracker.unity3d.com/issues/clearable-invalid-aabb-inaabb-errors-thrown-in-the-console-when-creating-project-using-3d-sample-scene-hdrp-template))

- iOS: Fixed potential memory leak when reallocating memory.
    (UUM-64048)

- Package: Fixes an issue in moderation package where initialization would fail on certain occasion.

- Physics: Fixed an issue where Rigidbody::Move and Rigidbody::MoveRotation would not respect position constraints when used with Rigidbody components set to kinematic.
    ([UUM-61558](https://issuetracker.unity3d.com/issues/kinematic-rigidbodies-can-move-despite-having-constraints-enabled-when-using-rigidbody-dot-moveposition))

- Physics 2D: Ensure that certain overloads of Rigidbody2D.Cast\(\) correctly use the implicit body rotation.
    ([UUM-65646](https://issuetracker.unity3d.com/issues/some-rigidbody2d-dot-cast-overloads-do-not-correct-use-the-rigidbody2d-angle))

- Shaders: Fixed a rare crash when rendering using a replacement shader that has dynamic keywords.
    ([UUM-66898](https://issuetracker.unity3d.com/issues/crash-on-dynamicbranchstate-preparestate-when-renderpipeline-dot-submitrenderrequest-is-called))

- SRP Core: Fixed DebugUI.Button not working in Rendering Debugger runtime UI.
    ([UUM-65457](https://issuetracker.unity3d.com/issues/debugui-dot-button-does-not-invoke-action-when-clicked))

- Universal RP: Added logic to enforce consistent hardware dynamic resolution settings during rendering to avoid issues when external code changes the global setting.
    ([UUM-58686](https://issuetracker.unity3d.com/issues/using-both-rthandle-and-dynamic-resolution-outputs-argumentnullexception-eventually-causing-a-crash))

- Universal RP: Fixed an issue where an incorrect WorldToCamera matrix was used in the main and additional light shadow passes.
    ([UUM-63267](https://issuetracker.unity3d.com/issues/incorrect-unity-worldtocamera-and-unity-cameratoworld-matrices-are-set-when-performing-the-shadowcaster-pass))

- Universal RP: Fixed an issue where logging an error gave a NullReferenceException for Server Builds.
    ([UUM-56965](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-running-a-dedicated-server-build-with-checked-enable-dedicated-server-optimizations-player-settings-checkbox))

- VFX Graph: Fixed an issue when trying to connect incompatible types, the error popup was left over if the action was canceled with Escape key.
    ([UUM-61583](https://issuetracker.unity3d.com/issues/vfx-wrong-type-popup-gets-stuck))

- VFX Graph: Fixed an issue where tooltips to the VFX Control panel were missing.
    ([UUM-8907](https://issuetracker.unity3d.com/issues/vfx-graph-vfx-control-window-does-not-have-tooltips))

- WebGL: Fixed an issue that prevented multithreaded builds from working if user repeatedly upgraded and then downgraded their project.
    ([UUM-33218](https://issuetracker.unity3d.com/issues/the-index-dot-html-file-is-generated-incorrectly-when-building-a-webgl-project))

- WebGL: Fixed issue using WebcamTexture.GetPixel\(s\) functions would return blank textures using the WebGL graphics API.
    ([UUM-46144](https://issuetracker.unity3d.com/issues/webcamtexture-dot-getpixels32-returns-black-pixels-when-in-webgl-player))

- WebGL: Improved IndexedDB filesystem performance by avoiding redundant filesystem persistence operations.
    (UUM-65276)

- WebGL: Remove "The PlayerLoop has been called recursively." error message spam.
    (UUM-55075)




#### Package changes in 2023.2.17f1

#### Packages updated

- com.unity.2d.aseprite: [1.1.1](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) &#x2192; [1.1.2](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- com.unity.services.qos: [1.2.0](https://docs.unity3d.com/Packages/com.unity.services.qos@1.2//changelog/CHANGELOG.html) &#x2192; [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.qos@1.3//changelog/CHANGELOG.html)

- com.unity.services.wire: [1.2.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html) &#x2192; [1.2.3](https://docs.unity3d.com/Packages/com.unity.services.wire@1.2//changelog/CHANGELOG.html)