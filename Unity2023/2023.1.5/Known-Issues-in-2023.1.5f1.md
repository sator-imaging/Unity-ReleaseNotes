# Unity 2023.1.5

https://unity.com/releases/editor/whats-new/2023.1.5

## Known Issues in 2023.1.5f1



*   3D Physics: Editor crashes on nv::cloth::FabricCookerImpl::cook when entering Play Mode ([UUM-34029](https://issuetracker.unity3d.com/issues/editor-crashes-on-nv-cloth-fabriccookerimpl-cook-when-entering-play-mode))
    
*   Asset Importers: Crash on "'anonymous namespace'::ConvertFBXShapes" when importing an FBX file ([UUM-38104](https://issuetracker.unity3d.com/issues/crash-on-anonymous-namespace-convertfbxshapes-when-importing-an-fbx-file))
    
*   Cloth: Crash on ClothScene::PrepareScene when entering Play mode ([UUM-16091](https://issuetracker.unity3d.com/issues/crash-on-clothscene-preparescene-when-entering-play-mode))
    
*   Graphics Device Features: Severe performance degradation in Play Mode when using multiple Cameras with "Direct3D12", "OpenGLCore", and "OpenGLES3" Graphics APIs in URP & HDRP ([UUM-42795](https://issuetracker.unity3d.com/issues/severe-performance-degradation-in-play-mode-when-using-multiple-cameras-with-direct3d12-openglcore-and-opengles3-graphics-apis-in-urp-and-hdrp))
    
*   HD RP: The Editor becomes unresponsive and the machine performs worse when the Editor is opened ([UUM-34562](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-the-machine-performs-worse-when-the-editor-is-opened))
    
*   Input: The device selection menu does not respond to mouse clicks when trying to add a device in a Control Scheme ([UUM-40635](https://issuetracker.unity3d.com/issues/the-device-selection-menu-does-not-respond-to-mouse-clicks-when-trying-to-add-a-device-in-a-control-scheme))
    
*   iOS: App freezes and the "You can attach a managed debugger now if you want” message doesn’t show up when running the app on iOS devices with the "Wait For Managed Debugger" setting enabled ([UUM-39644](https://issuetracker.unity3d.com/issues/ios-app-freezes-and-the-you-can-attach-a-managed-debugger-now-if-you-want-message-doesnt-show-up-when-running-the-app-on-ios-devices-with-the-wait-for-managed-debugger-setting-enabled))
    
*   MacOS: Crash on objc\_msgSend when the Editor UI gets redrawn ([UUM-34202](https://issuetracker.unity3d.com/issues/macos-crash-on-objc-msgsend-when-ui-gets-redrawn))
    
*   Metal: Editor freezes when exiting Play Mode if the Game window position was changed or undocked during Play Mode ([UUM-36218](https://issuetracker.unity3d.com/issues/editor-freezes-when-exiting-play-mode-if-the-game-window-position-was-changed-or-undocked-during-play-mode))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   Native Window Management: Crash on core::Join<core::basic\_string<char,core::StringStorageDefault > & \_\_ptr64,char const (& \_\_ptr64)\[2\],core::basic\_string\_ref > when the Editor runs out of memory saving an invalid override ([UUM-36776](https://issuetracker.unity3d.com/issues/crash-on-core-join-core-basic-string-char-core-stringstoragedefault-and-ptr64-char-const-and-ptr64-2-core-basic-string-ref-when-the-editor-runs-out-of-memory-saving-an-invalid-override))
    
*   Progressive Lightmapper: Light Probe GPU memory is not deallocated when cancelling a bake ([UUM-41988](https://issuetracker.unity3d.com/issues/light-probe-gpu-memory-is-not-deallocated-when-cancelling-a-bake))
    
*   Scene/Game View: Button triggers another Button when multiple Canvases are used in multiple windows ([UUM-36255](https://issuetracker.unity3d.com/issues/button-triggers-another-button-when-multiple-canvases-are-used-in-multiple-windows))
    
*   Serialization: Crash on SerializedProperty\_CUSTOM\_GetStringValueInternal when renaming a ScriptableObject Asset ([UUM-41704](https://issuetracker.unity3d.com/issues/crash-on-serializedproperty-custom-getstringvalueinternal-when-renaming-a-scriptableobject-asset))
    
*   UI Toolkit Controls: List View automatically collapses when reordering items ([UUM-42365](https://issuetracker.unity3d.com/issues/list-view-automatically-collapses-when-reordering-items))
    
*   UI Toolkit Framework: Unity Editor is rendered without the toolbar icons when using it on old hardware with integrated GPU ([UUM-13134](https://issuetracker.unity3d.com/issues/unity-editor-is-rendered-without-the-toolbar-icons-when-using-it-on-old-hardware-with-integrated-gpu))
    
*   Universal RP: RTHandles in URP causes memory allocation in multi-camera scenarios ([UUM-19089](https://issuetracker.unity3d.com/issues/urp-memory-leak-when-in-play-mode))
    
*   Universal RP: \[URP\]\[XR\] Performance degradation when comparing Android Quest 2 builds across 2020.3 and 2023.x ([UUM-33025](https://issuetracker.unity3d.com/issues/urp-xr-performance-degradation-when-comparing-android-quest-2-builds-across-2020-dot-3-and-2023-dot-x))
    
*   Visual Effects: Editor crashes on VFXRenderer::AddAsRenderNode when assigning a Renderer’s materials toits to materials/sharedMaterials ([UUM-37360](https://issuetracker.unity3d.com/issues/editor-crashes-on-vfxrenderer-addasrendernode-when-assigning-a-renderers-materials-toits-to-materials-slash-sharedmaterials))
    
*   Visual Effects: \[VFX Graph\] Crash on VFXBatch::AddInstance when switching to Custom Batch Capacity in Asset Inspector ([UUM-38059](https://issuetracker.unity3d.com/issues/vfx-graph-crash-on-vfxbatch-addinstance-when-switching-to-custom-batch-capacity-in-asset-inspector))
    
*   Visual Effects - Legacy: \[Android\]\[Vulkan\] Visualisation corruption occurs when rendering Particles to Render Texture ([UUM-21106](https://issuetracker.unity3d.com/issues/android-vulkan-visualisation-corruption-occurs-when-rendering-particles-to-render-texture))
    
*   XR SRP: Editor performance drops as OculusRuntime.WaitToBeginFrame Time ms increases to 150-200 ms in Play Mode when MSAA is enabled and Scene View is opened/focused ([UUM-40249](https://issuetracker.unity3d.com/issues/editor-performance-drops-as-oculusruntime-dot-waittobeginframe-time-ms-increases-to-150-200-ms-in-play-mode-when-msaa-is-enabled-and-scene-view-is-opened-slash-focused))