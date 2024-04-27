# Unity 2023.2.20

https://unity.com/releases/editor/whats-new/2023.2.20

## Known Issues in 2023.2.20f1



*   Asset - Database: Crash on UnityEditor.AssetDatabase:OpenAsset because assertion fails on prefabInstance.GetRootGameObject().IsValid() expression while opening a specific Scene ([UUM-66207](https://issuetracker.unity3d.com/issues/crash-on-unityeditor-dot-assetdatabase-openasset-because-assertion-fails-on-prefabinstance-dot-getrootgameobject-dot-isvalid-expression-while-opening-a-specific-scene))
    
*   Audio Authoring: Crash on AudioUtil\_CUSTOM\_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Lighting: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))
    
*   Platform Audio: Crash on FMOD::CodecMPEG::setPositionInternal when a mobile platform is selected and a specific audio clip is played ([UUM-62086](https://issuetracker.unity3d.com/issues/crash-on-fmod-codecmpeg-setpositioninternal-when-a-mobile-platform-is-selected-and-a-specific-audio-clip-is-played))
    
*   WebRequest: UnityWebRequest crashes if invoked when player is quitting ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))