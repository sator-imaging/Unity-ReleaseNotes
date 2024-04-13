# Unity 2023.2.18

https://unity.com/releases/editor/whats-new/2023.2.18

## Known Issues in 2023.2.18f1



*   Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))
    
*   Asset - Database: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene ([UUM-66207](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-openasset-because-assertion-fails-on-prefabinstance-dot-getrootgameobject-dot-isvalid-expression-while-opening-a-specific-scene))
    
*   Asset - Database: Fix for 2023.2.X: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene (UUM-66278)
    
*   Asset Bundles: Memory leak when building AssetBundle with Sprite Atlas enabled on macOS ([UUM-56323](https://issuetracker.unity3d.com/issues/memory-leak-when-building-assetbundle-with-sprite-atlas-enabled-on-macos))
    
*   Asset Importers: Unity crashes on strtol\_l when importing a specific .obj file ([UUM-42697](https://issuetracker.unity3d.com/issues/unity-crashes-on-strtol-l-when-importing-a-specific-obj-file))
    
*   Audio Authoring: Crash on AudioUtil\_CUSTOM\_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))
    
*   IAP: \[Android\] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Metal: Player hangs when re-focusing the Player window after switching to a window that covers the Player window ([UUM-67400](https://issuetracker.unity3d.com/issues/player-hangs-when-re-focusing-the-player-window-after-switching-to-a-window-that-covers-the-player-window))
    
*   Metal: \[iOS\] App crashes with out of memory exception in UnityGfxDeviceWorker when starting the app ([UUM-55488](https://issuetracker.unity3d.com/issues/ios-app-crashes-with-out-of-memory-exception-in-unitygfxdeviceworker-when-starting-the-app))
    
*   Platform Audio: Crash on FMOD::CodecMPEG::setPositionInternal when a mobile platform is selected and a specific audio clip is played ([UUM-62086](https://issuetracker.unity3d.com/issues/crash-on-fmod-codecmpeg-setpositioninternal-when-a-mobile-platform-is-selected-and-a-specific-audio-clip-is-played))
    
*   Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))
    
*   Scripting Runtime: Crash on RaiseException when selecting "Quit" in a "Fatal Error!" pop-up ([UUM-68119](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-selecting-quit-in-a-fatal-error-pop-up))
    
*   Text: Blurry Text ([UUM-49006](https://issuetracker.unity3d.com/issues/blurry-text))
    
*   Text: Fix for 2023.2.X: Blurry Text (UUM-49008)
    
*   UI Toolkit Controls: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))
    
*   WebRequest: UnityWebRequest crashes if invoked when player is quitting ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))