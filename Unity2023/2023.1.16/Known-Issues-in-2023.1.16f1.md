# Unity 2023.1.16

https://unity.com/releases/editor/whats-new/2023.1.16

## Known Issues in 2023.1.16f1



*   Asset Bundles: Editor crashes on vector\_map<ConstantString,AssetBundle when using the LoadAssetAsync function ([UUM-49715](https://issuetracker.unity3d.com/issues/editor-crashes-on-vector-map-constantstring-assetbundle-when-using-the-loadassetasync-function))
    
*   Cloth: Cannot use Paint tool ([UUM-35062](https://issuetracker.unity3d.com/issues/cloth-cannot-use-paint-tool))
    
*   Contextual Menu: \[TextMeshPro\] "CONTEXT" menu item appears and Editor crashes when TMP 3.2.0-pre.4 package is imported ([UUM-40410](https://issuetracker.unity3d.com/issues/textmeshpro-context-menu-item-appears-and-editor-crashes-when-tmp-3-dot-2-0-pre-dot-4-package-is-imported))
    
*   Culling: \[Mobile\] Player freezes on "UnityClassic::Baselib\_SystemFutex\_Wait" or silently crashes ([UUM-41806](https://issuetracker.unity3d.com/issues/android-player-freezes-on-unityclassic-baselib-systemfutex-wait-or-silently-crashes))
    
*   DirectX11: D3D11 swapchain error pop-up appears and the Editor shuts down when opening a project ([UUM-49251](https://issuetracker.unity3d.com/issues/d3d11-swapchain-error-pop-up-appears-and-the-editor-shuts-down-when-opening-a-project))
    
*   DirectX11: \[AMD\] \[DX11\] Additional lights are broken when Spotlight is added to the Scene ([UUM-20625](https://issuetracker.unity3d.com/issues/android-aditional-lights-are-broken-when-built-with-urp))
    
*   GLES: \[Linux\]\[URP\] Crash on GfxFramebufferGLES::Clear when entering the Play Mode when all Renderer Features are disabled, Native RenderPass and MainCamera's Depth Texture is enabled ([UUM-49240](https://issuetracker.unity3d.com/issues/linux-urp-crash-on-gfxframebuffergles-clear-when-entering-the-play-mode-when-all-renderer-features-are-disabled-native-renderpass-and-maincameras-depth-texture-is-enabled))
    
*   Input: Crash on InputDeviceIOCTL when closing Unity editor ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   OpenGL: \[Linux\]\[URP\]\[OpenGL\] Scene View has a red texture overlay when the project is using URP and OpenGLCore Graphics API ([UUM-44222](https://issuetracker.unity3d.com/issues/linux-urp-opengl-scene-view-has-a-red-texture-overlay-when-the-project-is-using-urp-and-openglcore-graphics-api))
    
*   Optimization: Crash on RendererUpdateManager::RemoveRenderer when undoing painting tiles to the scene ([UUM-48842](https://issuetracker.unity3d.com/issues/crash-on-rendererupdatemanager-removerenderer-when-undoing-painting-tiles-to-the-scene))
    
*   Platform Audio: Audio is delayed by ~0,5 sec after starting to play it in the Android/iOS Player ([UUM-41494](https://issuetracker.unity3d.com/issues/audio-is-delayed-by-05-sec-after-starting-to-play-it-in-the-android-slash-ios-player))
    
*   Scripting Runtime: "InvalidOperationException" is thrown when creating new Input Action ([UUM-26520](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-when-creating-new-input-action))
    
*   Scripting Runtime: Sometimes the wrong image is displayed when using Cursor.SetCursor in software mode ([UUM-46718](https://issuetracker.unity3d.com/issues/sometimes-the-wrong-image-is-displayed-when-using-cursor-dot-setcursor-in-software-mode))
    
*   Serialization: Crash and or slow update when List items are reordered in the Inspector Window ([UUM-46703](https://issuetracker.unity3d.com/issues/crash-and-or-slow-update-when-list-items-are-reordered-in-the-inspector-window))
    
*   Serialization: Editor Crashes on WalkTypeTreeComplete<`SerializedObjectTypeTreeWalk::ContainsManagedReferences'::`2'::IsManagedReferenceVisitor> when a list with serialize reference fields is re-ordered ([UUM-47108](https://issuetracker.unity3d.com/issues/editor-crashes-on-walktypetreecomplete-serializedobjecttypetreewalk-containsmanagedreferences-2-ismanagedreferencevisitor-when-a-list-with-serialize-reference-fields-is-re-ordered))
    
*   UI Builder: The Editor fails to load Layout Preset when it includes the UI Builder ([UUM-48802](https://issuetracker.unity3d.com/issues/the-editor-fails-to-load-layout-preset-when-it-includes-the-ui-builder))
    
*   UI Toolkit Controls: Prefab's scripts are constantly reloaded when trying to enter multiple digits or characters into public fields on custom scripts consecutively ([UUM-51430](https://issuetracker.unity3d.com/issues/prefabs-scripts-are-constantly-reloaded-when-trying-to-enter-multiple-digits-or-characters-into-public-fields-on-custom-scripts-consecutively))
    
*   UI Toolkit Framework: "ArgumentNullException" error in the Console when selecting certain ScriptableObjects and entering Play Mode ([UUM-39898](https://issuetracker.unity3d.com/issues/argumentnullexception-error-in-the-console-when-selecting-certain-scriptableobjects-and-entering-play-mode))
    
*   Universal RP: Meshes are not rendered when building WindowsStandalonePlayer builds from the command line with "batchmode", "nographics" flags ([UUM-47782](https://issuetracker.unity3d.com/issues/linux-meshes-are-not-rendered-when-building-windowsstandaloneplayer-builds-from-the-linux-command-line-with-batchmode-nographics-flags))
    
*   Visual Effects - Legacy: Particles are not adhering to the Mesh shape selected when being spawned by Sub Emitter Particles ([UUM-47307](https://issuetracker.unity3d.com/issues/particles-are-not-adhering-to-the-mesh-shape-selected-when-being-spawned-by-sub-emitter-particles))