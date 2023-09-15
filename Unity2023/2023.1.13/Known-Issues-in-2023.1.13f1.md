# Unity 2023.1.13

https://unity.com/releases/editor/whats-new/2023.1.13

## Known Issues in 2023.1.13f1



*   Addressable Assets: The released assets are not unloaded when Resources.UnloadUnusedAssets is called ([UUM-37775](https://issuetracker.unity3d.com/issues/the-released-assets-are-not-unloaded-when-resources-dot-unloadunusedassets-is-called))
    
*   Asset - Database: An Infinite import error is thrown when modifying the contents of a "folder plugin" ([UUM-47972](https://issuetracker.unity3d.com/issues/an-infinite-import-error-is-thrown-when-modifying-the-contents-of-a-folder-plugin))
    
*   Asset Importers: OnImportAsset leaks 5GB of memory ([UUM-43067](https://issuetracker.unity3d.com/issues/onimportasset-leaks-5gb-of-memory))
    
*   Cloth: Cannot use Paint tool ([UUM-35062](https://issuetracker.unity3d.com/issues/cloth-cannot-use-paint-tool))
    
*   Contextual Menu: \[TextMeshPro\] "CONTEXT" menu item appears and Editor crashes when TMP 3.2.0-pre.4 package is imported ([UUM-40410](https://issuetracker.unity3d.com/issues/textmeshpro-context-menu-item-appears-and-editor-crashes-when-tmp-3-dot-2-0-pre-dot-4-package-is-imported))
    
*   Culling: \[Mobile\] Player freezes on "UnityClassic::Baselib\_SystemFutex\_Wait" or silently crashes ([UUM-41806](https://issuetracker.unity3d.com/issues/android-player-freezes-on-unityclassic-baselib-systemfutex-wait-or-silently-crashes))
    
*   DirectX11: \[AMD\] \[DX11\] Additional lights are broken when Spotlight is added to the Scene ([UUM-20625](https://issuetracker.unity3d.com/issues/android-aditional-lights-are-broken-when-built-with-urp))
    
*   Graphics Device Features: Severe performance degradation in Play Mode when using multiple Cameras with “Direct3D12”, “OpenGLCore”, and “OpenGLES3” Graphics APIs in URP & HDRP ([UUM-42795](https://issuetracker.unity3d.com/issues/severe-performance-degradation-in-play-mode-when-using-multiple-cameras-with-direct3d12-openglcore-and-opengles3-graphics-apis-in-urp-and-hdrp))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   OpenGL: \[Linux\]\[URP\]\[OpenGL\] Scene View has a red texture overlay when the project is using URP and OpenGLCore Graphics API ([UUM-44222](https://issuetracker.unity3d.com/issues/linux-urp-opengl-scene-view-has-a-red-texture-overlay-when-the-project-is-using-urp-and-openglcore-graphics-api))
    
*   Scene/Game View: Button triggers another Button when multiple Canvases are used in multiple windows ([UUM-36255](https://issuetracker.unity3d.com/issues/button-triggers-another-button-when-multiple-canvases-are-used-in-multiple-windows))
    
*   Scripting Runtime: "InvalidOperationException" is thrown when creating new Input Action ([UUM-26520](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-when-creating-new-input-action))
    
*   Serialization: Crash and or slow update when List items are reordered in the Inspector Window ([UUM-46703](https://issuetracker.unity3d.com/issues/crash-and-or-slow-update-when-list-items-are-reordered-in-the-inspector-window))
    
*   Serialization: Crash on SerializedProperty\_CUSTOM\_GetStringValueInternal when renaming a ScriptableObject Asset ([UUM-41704](https://issuetracker.unity3d.com/issues/crash-on-serializedproperty-custom-getstringvalueinternal-when-renaming-a-scriptableobject-asset))
    
*   Serialization: Editor Crashes on WalkTypeTreeComplete<`SerializedObjectTypeTreeWalk::ContainsManagedReferences'::`2'::IsManagedReferenceVisitor> when a list with serialize reference fields is re-ordered ([UUM-47108](https://issuetracker.unity3d.com/issues/editor-crashes-on-walktypetreecomplete-serializedobjecttypetreewalk-containsmanagedreferences-2-ismanagedreferencevisitor-when-a-list-with-serialize-reference-fields-is-re-ordered))
    
*   UI Toolkit Framework: "ArgumentNullException" error in the Console when selecting certain ScriptableObjects and entering Play Mode ([UUM-39898](https://issuetracker.unity3d.com/issues/argumentnullexception-error-in-the-console-when-selecting-certain-scriptableobjects-and-entering-play-mode))
    
*   UI Toolkit Framework: Unity Editor is rendered without the toolbar icons on Intel HD Graphics 3000 ([UUM-13134](https://issuetracker.unity3d.com/issues/unity-editor-is-rendered-without-the-toolbar-icons-when-using-it-on-old-hardware-with-integrated-gpu))
    
*   Universal RP: RTHandles in URP causes memory allocation in multi-camera scenarios ([UUM-19089](https://issuetracker.unity3d.com/issues/urp-memory-leak-when-in-play-mode))
    
*   Visual Effects - Legacy: Particles are not adhering to the Mesh shape selected when being spawned by Sub Emitter Particles ([UUM-47307](https://issuetracker.unity3d.com/issues/particles-are-not-adhering-to-the-mesh-shape-selected-when-being-spawned-by-sub-emitter-particles))