# Unity 2023.1.19

https://unity.com/releases/editor/whats-new/2023.1.19

## Known Issues in 2023.1.19f1



*   Asset Bundles: Editor crashes on vector\_map<ConstantString,AssetBundle when using the LoadAssetAsync function ([UUM-49715](https://issuetracker.unity3d.com/issues/editor-crashes-on-vector-map-constantstring-assetbundle-when-using-the-loadassetasync-function))
    
*   Culling: \[Mobile\] Player freezes on "UnityClassic::Baselib\_SystemFutex\_Wait" or silently crashes ([UUM-41806](https://issuetracker.unity3d.com/issues/android-player-freezes-on-unityclassic-baselib-systemfutex-wait-or-silently-crashes))
    
*   GLES: \[Linux\]\[URP\] Crash on GfxFramebufferGLES::Clear when entering the Play Mode when all Renderer Features are disabled, Native RenderPass and MainCamera's Depth Texture is enabled ([UUM-49240](https://issuetracker.unity3d.com/issues/linux-urp-crash-on-gfxframebuffergles-clear-when-entering-the-play-mode-when-all-renderer-features-are-disabled-native-renderpass-and-maincameras-depth-texture-is-enabled))
    
*   Graphics Device Features: Frame Debugger: "A multisampled texture being bound to a non-multisampled sampler" errors when inspecting depth texture with MSAA ([UUM-54792](https://issuetracker.unity3d.com/issues/frame-debugger-a-multisampled-texture-being-bound-to-a-non-multisampled-sampler-errors-when-inspecting-depth-texture-with-msaa))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   Platform Audio: Audio is delayed by ~0,5 sec after starting to play it in the Android/iOS Player ([UUM-41494](https://issuetracker.unity3d.com/issues/audio-is-delayed-by-05-sec-after-starting-to-play-it-in-the-android-slash-ios-player))
    
*   Platform Audio: \[Linux\] No audio output when playing audio ([UUM-53143](https://issuetracker.unity3d.com/issues/linux-no-audio-output-when-playing-audio))
    
*   Serialization: Crash and or slow update when List items are reordered in the Inspector Window ([UUM-46703](https://issuetracker.unity3d.com/issues/crash-and-or-slow-update-when-list-items-are-reordered-in-the-inspector-window))
    
*   Text: Crash on Material::GetShader when the cache is pointing to an invalid material after domain reload ([UUM-53663](https://issuetracker.unity3d.com/issues/crash-on-material-getshader-when-the-cache-is-pointing-to-an-invalid-material-after-domain-reload))
    
*   uGUI: Button triggers another Button when multiple Canvases are used in multiple windows ([UUM-36255](https://issuetracker.unity3d.com/issues/button-triggers-another-button-when-multiple-canvases-are-used-in-multiple-windows))
    
*   UI Toolkit Controls: Adding and removing data from and to Serializable arrays with arrays in them throws errors and exceptions ([UUM-3235](https://issuetracker.unity3d.com/issues/adding-and-removing-data-from-and-to-serializable-arrays-with-arrays-in-them-throws-errors-and-exceptions))
    
*   UI Toolkit Controls: CustomPropertyDrawer throws an "Assertion failed on expression" error when adding the first element to the list ([UUM-34033](https://issuetracker.unity3d.com/issues/custompropertydrawer-throws-an-assertion-failed-on-expression-error-when-adding-the-first-element-to-the-list))
    
*   UnityTLS: UnityWebRequest performance drop when running multiple requests at once ([UUM-49389](https://issuetracker.unity3d.com/issues/unitywebrequestexception-cannot-resolve-destination-host-errors-appear-when-making-multiple-http-get-requests-using-unitywebrequest-and-the-cysharp-dot-threading-dot-tasks))
    
*   Universal RP: Depth pass is rendered with an incorrect matrix in the animation preview when using Universal RP ([UUM-41388](https://issuetracker.unity3d.com/issues/depth-pass-is-rendered-with-an-incorrect-matrix-in-the-animation-preview-when-using-universal-rp))
    
*   Windows: Sometimes the wrong image is displayed when using Cursor.SetCursor in software mode ([UUM-46718](https://issuetracker.unity3d.com/issues/sometimes-the-wrong-image-is-displayed-when-using-cursor-dot-setcursor-in-software-mode))
    
*   XR SRP: \[Quest\] Stutter/Frame Pacing with OculusRuntime.WaitToBeginFrame when the Player is built ([UUM-27247](https://issuetracker.unity3d.com/issues/quest-stutter-slash-frame-pacing-with-oculusruntime-dot-waittobeginframe-when-the-player-is-built))