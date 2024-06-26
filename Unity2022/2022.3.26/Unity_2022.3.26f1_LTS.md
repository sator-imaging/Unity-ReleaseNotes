# Unity 2022.3.26f1 LTS
Tue, 23 Apr 2024 17:47:02 GMT  
https://unity.com/releases/editor/whats-new/2022.3.26

### Known Issues in 2022.3.26f1

- Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode
    ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))

- Asset - Database: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene
    ([UUM-66207](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-openasset-because-assertion-fails-on-prefabinstance-dot-getrootgameobject-dot-isvalid-expression-while-opening-a-specific-scene))

- Asset Importers: Crash on StackAllocator<0>::GetOverheadSize when importing the “POLYGON City - Low Poly 3D Art by Synty“ asset pack
    ([UUM-55981](https://issuetracker.unity3d.com/issues/crash-on-stackallocator-getoverheadsize-when-importing-the-polygon-city-low-poly-3d-art-by-synty-asset-pack))

- Graphics Optimization: Crash on PrepareDrawShadowsCommandStep1 when selecting a camera while the Occlusion Culling window is open
    ([UUM-506](https://issuetracker.unity3d.com/issues/crash-on-preparedrawshadowscommandstep1-when-selecting-a-camera-while-the-occlusion-culling-window-is-open))

- IAP: [Android] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener
    ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))

- IL2CPP: [Android] Crash on Android when AndroidJavaProxy is calling from multiple threads
    ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))

- Metal: Player hangs when re-focusing the Player window after switching to a window that covers the Player window
    ([UUM-67400](https://issuetracker.unity3d.com/issues/player-hangs-when-re-focusing-the-player-window-after-switching-to-a-window-that-covers-the-player-window))

- Platform Audio: Crash on FMOD::CodecMPEG::setPositionInternal when a mobile platform is selected and a specific audio clip is played
    ([UUM-62086](https://issuetracker.unity3d.com/issues/crash-on-fmod-codecmpeg-setpositioninternal-when-a-mobile-platform-is-selected-and-a-specific-audio-clip-is-played))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- WebRequest: UnityWebRequest crashes if invoked when player is quitting
    ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))



### 2022.3.26f1 Release Notes

#### Improvements

- Build System: Serialise concurrent overlapping bee standalone driver processes to avoid build failures.



#### Changes

- Build System: Upgraded unity-unpacker and bsdtar binaries to use libarchive 3.7.3.

- Package: Updated Cinemachine package to 2.10.0.



#### Fixes

- 2D: Fixed unable to create Sprite in Sprite Editor Window in certain cases.
    ([UUM-67197](https://issuetracker.unity3d.com/issues/sprite-editor-does-not-allow-creating-new-sprite-tiles-in-a-sprite-sheet-with-a-specific-name))

- Android: Bump Android Logcat Package to 1.4.1.

- Asset Bundles: Fixed performance regression when clearing bundle cache folders.
    ([UUM-60063](https://issuetracker.unity3d.com/issues/long-load-times-when-large-asset-bundles-are-discarded))

- Core: Fixed floating point issue in APV sampling.
    ([UUM-47714](https://issuetracker.unity3d.com/issues/white-pixel-fragments-and-spots-randomly-appear-and-flicker-when-a-specific-reflection-probe-is-enabled))

- Documentation: Fixed EditorUtility.OpenFilePanelWithFilters documentation.
    (UUM-44679)

- Documentation: Fixed EditorUtility.SetDialogOptOutDecision documentation.
    (UUM-43878)

- Editor: Default assets should not be uploaded to the Accelerator.
    ([UUM-66975](https://issuetracker.unity3d.com/issues/editor-uploads-broken-assets-to-unity-accelerator-when-it-crashes-during-an-import))

- Editor: Errors related to the sqlite dll when using the Windows ARM64 Editor.

- Editor: Fixed crash when entering and leaving play mode while UnityWebRequest is downloading texture using DownloadHandlerTexture.
    (UUM-68555)

- Editor: Fixed flickering when using baked gi node and TAA.
    ([UUM-65682](https://issuetracker.unity3d.com/issues/hd-rp-shader-graph-with-a-baked-gi-node-flickers-when-probe-volumes-and-taa-are-enabled))

- Editor: Fixed how SearchPRoviders are enabled and setup/disabled in search window.
    ([UUM-62165](https://issuetracker.unity3d.com/issues/enable-asset-database-adb-provider-doesnt-update-the-search-window))

- Editor: Fixed how tags and labels thumbnails are displayed in Search Propositions.
    ([UUM-62795](https://issuetracker.unity3d.com/issues/search-labels-and-tags-icons-dont-look-neat))

- Editor: Fixed issue where dialog box with a progress bar can cause a crash when entering play mode on macOS.
    ([UUM-66854](https://issuetracker.unity3d.com/issues/crash-on-overridingparameterpreparer-onpreparevector-when-entering-play-mode))

- Editor: Fixed performance regression introduced by SO Library detection change.
    (UUM-25880)

- Editor: Fixed temp memory leak inside Memory Profiler GUI element.
    ([UUM-62793](https://issuetracker.unity3d.com/issues/malloc-temp-pool-keeps-increasing-when-executing-the-job-dot-run-in-a-thread))

- Editor: HDRP: Fixed out-of-range errors that can happen when using decals with multiple cameras.
    ([UUM-66021](https://issuetracker.unity3d.com/issues/game-freezes-and-indexoutofrangeexception-errors-are-thrown-in-the-console-when-putting-many-hdrp-decals-quickly))

- Editor: Removed "Autofill" menu item from the "Edit" menu.
    ([UUM-62774](https://issuetracker.unity3d.com/issues/autofill-menu-item-is-presented-in-edit))

- Editor: Removed "Close All" menu item from the "File" menu.
    (UUM-65192)

- HDRP: Banding in IES importer.
    (UUM-68033)

- HDRP: Fixed cinematic eye shader lighting from directional lights.
    ([UUM-65500](https://issuetracker.unity3d.com/issues/eye-shader-lighting-depends-on-world-position-when-using-eyecinematic-material-type))

- HDRP: Fixed realloc of history buffer when XR is enabled.
    ([UUM-41386](https://issuetracker.unity3d.com/issues/quest-2-xr-plugin-management-the-physically-based-sky-and-volumetric-clouds-are-rendered-only-for-the-left-eye-when-xr-is-initialized-manually))

- HDRP: Fixed TAA post sharpen in XR.
    ([UUM-32872](https://issuetracker.unity3d.com/issues/xr-only-1-eye-is-rendered-when-single-pass-instanced-and-taa-post-sharpen-is-used))

- HDRP: Fixed underwater applied when water is disabled.
    ([UUM-61413](https://issuetracker.unity3d.com/issues/the-under-water-effect-continues-to-be-applied-when-you-exit-a-gameobject-with-the-water-surface-component-from-the-side))

- iOS: Fixed ProjectCapabilityManager.AddHealthKit API not adding HealthKit capability to PBXProject correctly.
    ([UUM-65393](https://issuetracker.unity3d.com/issues/ios-projectcapabilitymanager-dot-addhealthkit-doesnt-correctly-add-healthkit-capability))

- iOS: UnityWebRequest URLs with unescaped symbols \[ and \] in query and containing other spec characters like space will now fail on iOS 17 instead of sending request to improperly escaped \(and as such - wrong\) url. URLs that are properly percent-escaped are recommended and will work correctly.
    (UUM-66942)

- Linux: Fixed Multi-touch events not recognizing on Linux Player.
    (UUM-49191)

- Linux: Prevent crash when shader compiler steals focus from preview texture window.
    (UUM-59278)

- macOS: Fixed custom cursor not used if mouse leaves the window.
    ([UUM-67592](https://issuetracker.unity3d.com/issues/cursor-does-not-switch-back-to-the-custom-cursor-when-the-mouse-is-moved-back-into-the-player-window-on-macos))

- Prefabs: Crash on PhysicsManager::SetBodyTransformChangeInterest when opening a scene.
    ([UUM-56057](https://issuetracker.unity3d.com/issues/crash-on-physicsmanager-setbodytransformchangeinterest-when-opening-a-scene))

- Shadergraph: Added issues where shaders generated for iOS or Android may not compile correctly due to precision.
    ([UUM-64863](https://issuetracker.unity3d.com/issues/shader-is-rendered-pink-or-not-rendered-at-all-in-the-editor-and-player-when-the-precision-is-set-to-half-in-the-shader-graph-and-the-android-or-ios-platform-is-selected))

- Shaders: Fixed shaders marked incompatible with the SRP Batcher when shaders with a lot of similar properties were loaded.
    (UUM-69238)

- SRP Core: Fixed PackFloat2To8  in packing.hlsl.
    ([UUM-62724](https://issuetracker.unity3d.com/issues/corerp-packfloat2to8-is-broken-in-packing-dot-hlsl))

- UI Toolkit: Fixed large memory allocation sometimes happening when processing style variables.
    (UUM-69741)

- UI Toolkit: Fixed UIDocument component not showing on some Inspector windows when multiple inspectors are open.
    (UUM-67033)

- Undo System: Fixed crash when undoing an action in a graph using Undo.RecordObject.
    (UUM-58380)

- Universal RP: Removed duplicated code in UniversalRenderer.cs.
    ([UUM-69481](https://issuetracker.unity3d.com/issues/duplicate-code-in-the-universalrenderer-dot-cs-file-of-the-urp-package))

- Universal Windows Platform: Syncing capabilities to update the manifest is only necessary if the manifest already exists.
    (UUM-68424)

- Video: Fixed the Video Player to play the video after seeking back to frame 0 when Loop and Skip On Drop are enabled and the video has looped once.
    ([UUM-66728](https://issuetracker.unity3d.com/issues/the-video-player-does-not-play-the-video-after-seeking-back-to-frame-0-when-loop-and-skip-on-drop-are-enabled-and-the-video-has-looped-once))

- Video: Video repeats the first frame on Android when it is played via Unity's Video Player component.
    ([UUM-45914](https://issuetracker.unity3d.com/issues/android-video-repeats-the-first-frame-on-android-when-it-is-played-via-unitys-video-player-component))

- VisionOS: Fixed the Pause/Resume callbacks from being invoked twice when resuming from pause, causing a crash.

- XR: Updated XR Hands package to 1.4.0 and set 1.5.0-pre.1 as available next version.

- XR: Updated XR Interaction Toolkit package to 2.5.4.




#### Package changes in 2022.3.26f1

#### Packages updated

- com.unity.cinemachine: [2.9.5](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.9//changelog/CHANGELOG.html) &#x2192; [2.10.0](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat: [1.4.0](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) &#x2192; [1.4.1](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.visualscripting: [1.9.2](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) &#x2192; [1.9.4](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.3.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.3//changelog/CHANGELOG.html) &#x2192; [1.4.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.4//changelog/CHANGELOG.html)

- com.unity.xr.interaction.toolkit: [2.5.2](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.5//changelog/CHANGELOG.html) &#x2192; [2.5.4](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.5//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.services.vivox@16.2.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.2//changelog/CHANGELOG.html)