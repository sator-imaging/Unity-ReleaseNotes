# Unity 2023.1.17

https://unity.com/releases/editor/whats-new/2023.1.17

## Known Issues in 2023.1.17f1



*   Asset Bundles: Editor crashes on vector\_map<ConstantString,AssetBundle when using the LoadAssetAsync function ([UUM-49715](https://issuetracker.unity3d.com/issues/editor-crashes-on-vector-map-constantstring-assetbundle-when-using-the-loadassetasync-function))
    
*   Cloth: Cannot use Paint tool ([UUM-35062](https://issuetracker.unity3d.com/issues/cloth-cannot-use-paint-tool))
    
*   Culling: \[Mobile\] Player freezes on "UnityClassic::Baselib\_SystemFutex\_Wait" or silently crashes ([UUM-41806](https://issuetracker.unity3d.com/issues/android-player-freezes-on-unityclassic-baselib-systemfutex-wait-or-silently-crashes))
    
*   DirectX11: D3D11 swapchain error pop-up appears and the Editor shuts down when opening a project ([UUM-49251](https://issuetracker.unity3d.com/issues/d3d11-swapchain-error-pop-up-appears-and-the-editor-shuts-down-when-opening-a-project))
    
*   DirectX11: \[AMD\] \[DX11\] Additional lights are broken when Spotlight is added to the Scene ([UUM-20625](https://issuetracker.unity3d.com/issues/android-aditional-lights-are-broken-when-built-with-urp))
    
*   GLES: \[Linux\]\[URP\] Crash on GfxFramebufferGLES::Clear when entering the Play Mode when all Renderer Features are disabled, Native RenderPass and MainCamera's Depth Texture is enabled ([UUM-49240](https://issuetracker.unity3d.com/issues/linux-urp-crash-on-gfxframebuffergles-clear-when-entering-the-play-mode-when-all-renderer-features-are-disabled-native-renderpass-and-maincameras-depth-texture-is-enabled))
    
*   Kernel: Crash on RendererUpdateManager::RemoveRenderer when undoing painting tiles to the scene ([UUM-48842](https://issuetracker.unity3d.com/issues/crash-on-rendererupdatemanager-removerenderer-when-undoing-painting-tiles-to-the-scene))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   OpenGL: \[Linux\]\[URP\]\[OpenGL\] Scene View has a red texture overlay when the project is using URP and OpenGLCore Graphics API ([UUM-44222](https://issuetracker.unity3d.com/issues/linux-urp-opengl-scene-view-has-a-red-texture-overlay-when-the-project-is-using-urp-and-openglcore-graphics-api))
    
*   Platform Audio: Audio is delayed by ~0,5 sec after starting to play it in the Android/iOS Player ([UUM-41494](https://issuetracker.unity3d.com/issues/audio-is-delayed-by-05-sec-after-starting-to-play-it-in-the-android-slash-ios-player))
    
*   Scene Management: Crash on RuntimeSceneManager::UnloadAllScenesWithoutDestroyingGameObjects when exiting Play Mode ([UUM-53145](https://issuetracker.unity3d.com/issues/crash-on-runtimescenemanager-unloadallsceneswithoutdestroyinggameobjects-when-exiting-play-mode))
    
*   Serialization: Crash and or slow update when List items are reordered in the Inspector Window ([UUM-46703](https://issuetracker.unity3d.com/issues/crash-and-or-slow-update-when-list-items-are-reordered-in-the-inspector-window))
    
*   Serialization: Editor Crashes on WalkTypeTreeComplete<`SerializedObjectTypeTreeWalk::ContainsManagedReferences'::`2'::IsManagedReferenceVisitor> when a list with serialize reference fields is re-ordered ([UUM-47108](https://issuetracker.unity3d.com/issues/editor-crashes-on-walktypetreecomplete-serializedobjecttypetreewalk-containsmanagedreferences-2-ismanagedreferencevisitor-when-a-list-with-serialize-reference-fields-is-re-ordered))
    
*   Text: \[TextMeshPro\] "CONTEXT" menu item appears and Editor crashes when TMP 3.2.0-pre.4 package is imported ([UUM-40410](https://issuetracker.unity3d.com/issues/textmeshpro-context-menu-item-appears-and-editor-crashes-when-tmp-3-dot-2-0-pre-dot-4-package-is-imported))
    
*   Universal RP: Depth pass is rendered with an incorrect matrix in the animation preview when using Universal RP ([UUM-41388](https://issuetracker.unity3d.com/issues/depth-pass-is-rendered-with-an-incorrect-matrix-in-the-animation-preview-when-using-universal-rp))
    
*   Universal RP: Meshes are not rendered when building WindowsStandalonePlayer builds from the command line with "batchmode", "nographics" flags ([UUM-47782](https://issuetracker.unity3d.com/issues/linux-meshes-are-not-rendered-when-building-windowsstandaloneplayer-builds-from-the-linux-command-line-with-batchmode-nographics-flags))