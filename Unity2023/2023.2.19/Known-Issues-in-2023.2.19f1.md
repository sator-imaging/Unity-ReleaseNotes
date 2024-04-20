# Unity 2023.2.19

https://unity.com/releases/editor/whats-new/2023.2.19

## Known Issues in 2023.2.19f1



*   Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))
    
*   Asset - Database: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene ([UUM-66207](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-openasset-because-assertion-fails-on-prefabinstance-dot-getrootgameobject-dot-isvalid-expression-while-opening-a-specific-scene))
    
*   Asset - Database: Fix for 2023.2.X: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene (UUM-66278)
    
*   Asset Bundles: Memory leak when building AssetBundle with Sprite Atlas enabled on macOS ([UUM-56323](https://issuetracker.unity3d.com/issues/memory-leak-when-building-assetbundle-with-sprite-atlas-enabled-on-macos))
    
*   Audio Authoring: Crash on AudioUtil\_CUSTOM\_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))
    
*   IAP: \[Android\] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Metal: Player hangs when re-focusing the Player window after switching to a window that covers the Player window ([UUM-67400](https://issuetracker.unity3d.com/issues/player-hangs-when-re-focusing-the-player-window-after-switching-to-a-window-that-covers-the-player-window))
    
*   Platform Audio: Crash on FMOD::CodecMPEG::setPositionInternal when a mobile platform is selected and a specific audio clip is played ([UUM-62086](https://issuetracker.unity3d.com/issues/crash-on-fmod-codecmpeg-setpositioninternal-when-a-mobile-platform-is-selected-and-a-specific-audio-clip-is-played))
    
*   Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))
    
*   Scripting Runtime: \[TypeCache\] Crash on RaiseException when selecting "Quit" in a "Fatal Error!" pop-up ([UUM-68119](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-selecting-quit-in-a-fatal-error-pop-up))
    
*   SRP Architecture & API: Stacked camera is not rendering when using custom post effects is done in PreRender PostRender and Camera is not in HDR ([UUM-22444](https://issuetracker.unity3d.com/issues/ios-stacked-camera-is-not-rendering-when-using-custom-post-effects-and-build-target-is-set-to-ios))
    
*   Text: Blurry Text ([UUM-49006](https://issuetracker.unity3d.com/issues/blurry-text))
    
*   Text: Fix for 2023.2.X: Blurry Text (UUM-49008)
    
*   WebRequest: UnityWebRequest crashes if invoked when player is quitting ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))