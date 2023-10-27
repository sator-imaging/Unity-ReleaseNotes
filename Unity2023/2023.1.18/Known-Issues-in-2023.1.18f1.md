# Unity 2023.1.18

https://unity.com/releases/editor/whats-new/2023.1.18

## Known Issues in 2023.1.18f1



*   Asset Bundles: Editor crashes on vector\_map<ConstantString,AssetBundle when using the LoadAssetAsync function ([UUM-49715](https://issuetracker.unity3d.com/issues/editor-crashes-on-vector-map-constantstring-assetbundle-when-using-the-loadassetasync-function))
    
*   Culling: \[Mobile\] Player freezes on "UnityClassic::Baselib\_SystemFutex\_Wait" or silently crashes ([UUM-41806](https://issuetracker.unity3d.com/issues/android-player-freezes-on-unityclassic-baselib-systemfutex-wait-or-silently-crashes))
    
*   GLES: \[Linux\]\[URP\] Crash on GfxFramebufferGLES::Clear when entering the Play Mode when all Renderer Features are disabled, Native RenderPass and MainCamera's Depth Texture is enabled ([UUM-49240](https://issuetracker.unity3d.com/issues/linux-urp-crash-on-gfxframebuffergles-clear-when-entering-the-play-mode-when-all-renderer-features-are-disabled-native-renderpass-and-maincameras-depth-texture-is-enabled))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   Platform Audio: Audio is delayed by ~0,5 sec after starting to play it in the Android/iOS Player ([UUM-41494](https://issuetracker.unity3d.com/issues/audio-is-delayed-by-05-sec-after-starting-to-play-it-in-the-android-slash-ios-player))
    
*   Serialization: Crash and or slow update when List items are reordered in the Inspector Window ([UUM-46703](https://issuetracker.unity3d.com/issues/crash-and-or-slow-update-when-list-items-are-reordered-in-the-inspector-window))
    
*   Serialization: Editor Crashes on WalkTypeTreeComplete<`SerializedObjectTypeTreeWalk::ContainsManagedReferences'::`2'::IsManagedReferenceVisitor> when a list with serialize reference fields is re-ordered ([UUM-47108](https://issuetracker.unity3d.com/issues/editor-crashes-on-walktypetreecomplete-serializedobjecttypetreewalk-containsmanagedreferences-2-ismanagedreferencevisitor-when-a-list-with-serialize-reference-fields-is-re-ordered))
    
*   Text: Crash on Material::GetShader when the cache is pointing to an invalid material after domain reload ([UUM-53663](https://issuetracker.unity3d.com/issues/crash-on-material-getshader-when-the-cache-is-pointing-to-an-invalid-material-after-domain-reload))
    
*   uGUI: Button triggers another Button when multiple Canvases are used in multiple windows ([UUM-36255](https://issuetracker.unity3d.com/issues/button-triggers-another-button-when-multiple-canvases-are-used-in-multiple-windows))
    
*   UnityTLS: UnityWebRequest performance drop when running multiple requests at once ([UUM-49389](https://issuetracker.unity3d.com/issues/unitywebrequestexception-cannot-resolve-destination-host-errors-appear-when-making-multiple-http-get-requests-using-unitywebrequest-and-the-cysharp-dot-threading-dot-tasks))
    
*   Universal RP: Meshes are not rendered when building WindowsStandalonePlayer builds from the command line with "batchmode", "nographics" flags ([UUM-47782](https://issuetracker.unity3d.com/issues/linux-meshes-are-not-rendered-when-building-windowsstandaloneplayer-builds-from-the-linux-command-line-with-batchmode-nographics-flags))
    
*   Windows: Sometimes the wrong image is displayed when using Cursor.SetCursor in software mode ([UUM-46718](https://issuetracker.unity3d.com/issues/sometimes-the-wrong-image-is-displayed-when-using-cursor-dot-setcursor-in-software-mode))
    
*   XR SRP: \[Quest\] Stutter/Frame Pacing with OculusRuntime.WaitToBeginFrame when the Player is built ([UUM-27247](https://issuetracker.unity3d.com/issues/quest-stutter-slash-frame-pacing-with-oculusruntime-dot-waittobeginframe-when-the-player-is-built))