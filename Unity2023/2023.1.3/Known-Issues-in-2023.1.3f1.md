# Unity 2023.1.3

https://unity.com/releases/editor/whats-new/2023.1.3

## Known Issues in 2023.1.3f1



*   3D Physics: Editor crashes on nv::cloth::FabricCookerImpl::cook when entering Play Mode ([UUM-34029](https://issuetracker.unity3d.com/issues/editor-crashes-on-nv-cloth-fabriccookerimpl-cook-when-entering-play-mode))
    
*   Asset Importers: Crash on "'anonymous namespace'::ConvertFBXShapes" when importing an FBX file ([UUM-38104](https://issuetracker.unity3d.com/issues/crash-on-anonymous-namespace-convertfbxshapes-when-importing-an-fbx-file))
    
*   HD RP: The Editor becomes unresponsive and the machine performs worse when the Editor is opened ([UUM-34562](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-the-machine-performs-worse-when-the-editor-is-opened))
    
*   iOS: App freezes and the "You can attach a managed debugger now if you want” message doesn’t show up when running the app on iOS devices with the "Wait For Managed Debugger" setting enabled ([UUM-39644](https://issuetracker.unity3d.com/issues/ios-app-freezes-and-the-you-can-attach-a-managed-debugger-now-if-you-want-message-doesnt-show-up-when-running-the-app-on-ios-devices-with-the-wait-for-managed-debugger-setting-enabled))
    
*   MacOS: Crash on objc\_msgSend when the Editor UI gets redrawn ([UUM-34202](https://issuetracker.unity3d.com/issues/macos-crash-on-objc-msgsend-when-ui-gets-redrawn))
    
*   Metal: Editor freezes when exiting Play Mode if the Game window position was changed or undocked during Play Mode ([UUM-36218](https://issuetracker.unity3d.com/issues/editor-freezes-when-exiting-play-mode-if-the-game-window-position-was-changed-or-undocked-during-play-mode))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   Native Window Management: Crash on core::Join<core::basic\_string<char,core::StringStorageDefault > & \_\_ptr64,char const (& \_\_ptr64)\[2\],core::basic\_string\_ref > when the Editor runs out of memory saving an invalid override ([UUM-36776](https://issuetracker.unity3d.com/issues/crash-on-core-join-core-basic-string-char-core-stringstoragedefault-and-ptr64-char-const-and-ptr64-2-core-basic-string-ref-when-the-editor-runs-out-of-memory-saving-an-invalid-override))
    
*   Platform Audio: \[WebGL\] A looping audio sounds different on WebGL than in the editor/native desktop player ([UUM-12530](https://issuetracker.unity3d.com/issues/webgl-a-looping-audio-sounds-different-on-webgl-than-in-the-editor-slash-native-desktop-player))
    
*   Project Browser: Project Browser shows package resources when package visibility is disabled ([UUM-32517](https://issuetracker.unity3d.com/issues/project-browser-shows-package-resources-when-package-visibility-is-disabled))
    
*   Scene/Game View: Button triggers another Button when multiple Canvases are used in multiple windows ([UUM-36255](https://issuetracker.unity3d.com/issues/button-triggers-another-button-when-multiple-canvases-are-used-in-multiple-windows))
    
*   Universal RP: A memory leak occurs in the Player when Two Cameras are used and one of them has an "Output Texture" set ([UUM-40695](https://issuetracker.unity3d.com/issues/a-memory-leak-occurs-in-the-player-when-two-cameras-are-used-and-one-of-them-has-an-output-texture-set))
    
*   Universal RP: ArgumentNullException and Assertion failed errors thrown when enabling Opaque Texture, using the Hierarchy search bar, and viewing the Scene tab in Play Mode ([UUM-36458](https://issuetracker.unity3d.com/issues/argumentnullexception-and-assertion-failed-errors-thrown-when-enabling-opaque-texture-using-the-hierarchy-search-bar-and-viewing-the-scene-tab-in-play-mode))
    
*   Universal RP: Decal is not drawn when using Deferred Rendering, a Rendering Layer, and Screen Space Ambient Occlusion ([UUM-39831](https://issuetracker.unity3d.com/issues/decal-is-not-drawn-when-using-deferred-rendering-a-rendering-layer-and-screen-space-ambient-occlusion))
    
*   Universal RP: RTHandles in URP causes memory allocation in multi-camera scenarios ([UUM-19089](https://issuetracker.unity3d.com/issues/urp-memory-leak-when-in-play-mode))
    
*   Universal RP: \[URP\]\[XR\] Performance degradation when comparing Android Quest 2 builds across 2020.3 and 2023.x ([UUM-33025](https://issuetracker.unity3d.com/issues/urp-xr-performance-degradation-when-comparing-android-quest-2-builds-across-2020-dot-3-and-2023-dot-x))
    
*   Visual Effects: Editor crashes on VFXRenderer::AddAsRenderNode when assigning a Renderer’s materials toits to materials/sharedMaterials ([UUM-37360](https://issuetracker.unity3d.com/issues/editor-crashes-on-vfxrenderer-addasrendernode-when-assigning-a-renderers-materials-toits-to-materials-slash-sharedmaterials))
    
*   Visual Effects: \[VFX Graph\] Crash on VFXBatch::AddInstance when switching to Custom Batch Capacity in Asset Inspector ([UUM-38059](https://issuetracker.unity3d.com/issues/vfx-graph-crash-on-vfxbatch-addinstance-when-switching-to-custom-batch-capacity-in-asset-inspector))
    
*   Web Platform: \[WebGL\] Build fails and Shader errors are logged when Code Optimisation is set to Runtime Speed ([UUM-40103](https://issuetracker.unity3d.com/issues/webgl-build-fails-and-shader-errors-are-logged-when-code-optimisation-is-set-to-runtime-speed))
    
*   XR SRP: Editor performance drops as OculusRuntime.WaitToBeginFrame Time ms increases to 150-200 ms in Play Mode when MSAA is enabled and Scene View is opened/focused ([UUM-40249](https://issuetracker.unity3d.com/issues/editor-performance-drops-as-oculusruntime-dot-waittobeginframe-time-ms-increases-to-150-200-ms-in-play-mode-when-msaa-is-enabled-and-scene-view-is-opened-slash-focused))