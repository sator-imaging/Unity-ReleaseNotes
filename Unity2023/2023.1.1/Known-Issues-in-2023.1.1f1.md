# Unity 2023.1.1

https://unity.com/releases/editor/whats-new/2023.1.1

## Known Issues in 2023.1.1f1



*   Asset Importers: Crash on "'anonymous namespace'::ConvertFBXShapes" when importing an FBX file ([UUM-38104](https://issuetracker.unity3d.com/issues/crash-on-anonymous-namespace-convertfbxshapes-when-importing-an-fbx-file))
    
*   Editor Window Management: 2D projects created with versions from 2023.1.0a25 to 2023.1.0b4 fail to upgrade to 2023.1.0b9 and later 2023.1.0bX versions ([UUM-34312](https://issuetracker.unity3d.com/issues/2d-projects-created-with-versions-from-2023-dot-1-0a25-to-2023-dot-1-0b4-fail-to-upgrade-to-2023-dot-1-0b9-and-later-2023-dot-1-0bx-versions))
    
*   HD RP: The Editor becomes unresponsive and the machine performs worse when the Editor is opened ([UUM-34562](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-the-machine-performs-worse-when-the-editor-is-opened))
    
*   Input: The "Listen" button and input field for action Binding Path is mostly not visible ([UUM-36929](https://issuetracker.unity3d.com/issues/the-listen-button-and-input-field-for-action-binding-path-is-mostly-not-visible))
    
*   MacOS: Crash on objc\_msgSend when the Editor UI gets redrawn ([UUM-34202](https://issuetracker.unity3d.com/issues/macos-crash-on-objc-msgsend-when-ui-gets-redrawn))
    
*   Metal: Editor freezes when exiting Play Mode if the Game window position was changed or undocked during Play Mode ([UUM-36218](https://issuetracker.unity3d.com/issues/editor-freezes-when-exiting-play-mode-if-the-game-window-position-was-changed-or-undocked-during-play-mode))
    
*   Metal: \[iOS\] Rendering freezes when the orientation is changed ([UUM-9480](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-when-the-orientation-is-changed))
    
*   Native Window Management: Crash on core::Join<core::basic\_string<char,core::StringStorageDefault > & \_\_ptr64,char const (& \_\_ptr64)\[2\],core::basic\_string\_ref > when the Editor runs out of memory saving an invalid override ([UUM-36776](https://issuetracker.unity3d.com/issues/crash-on-core-join-core-basic-string-char-core-stringstoragedefault-and-ptr64-char-const-and-ptr64-2-core-basic-string-ref-when-the-editor-runs-out-of-memory-saving-an-invalid-override))
    
*   Physics: Editor crashes on nv::cloth::FabricCookerImpl::cook when entering Play Mode ([UUM-34029](https://issuetracker.unity3d.com/issues/editor-crashes-on-nv-cloth-fabriccookerimpl-cook-when-entering-play-mode))
    
*   Platform Audio: \[WebGL\] A looping audio sounds different on WebGL than in the editor/native desktop player ([UUM-12530](https://issuetracker.unity3d.com/issues/webgl-a-looping-audio-sounds-different-on-webgl-than-in-the-editor-slash-native-desktop-player))
    
*   Project Browser: Project Browser shows package resources when package visibility is disabled ([UUM-32517](https://issuetracker.unity3d.com/issues/project-browser-shows-package-resources-when-package-visibility-is-disabled))
    
*   Shader System: Shader keywords are ignored when using Camera.main.SetReplacementShader ([UUM-40400](https://issuetracker.unity3d.com/issues/shader-keywords-are-ignored-when-using-camera-dot-main-dot-setreplacementshader))
    
*   Shadows/Lights: Directional Light Shadow glitches when the Shadow Strength value is changed ([UUM-34294](https://issuetracker.unity3d.com/issues/directional-light-shadow-glitches-when-the-shadow-strength-value-is-changed))
    
*   Universal RP: Decal is not drawn when using Deferred Rendering, a Rendering Layer, and Screen Space Ambient Occlusion ([UUM-39831](https://issuetracker.unity3d.com/issues/decal-is-not-drawn-when-using-deferred-rendering-a-rendering-layer-and-screen-space-ambient-occlusion))
    
*   Universal RP: RTHandles in URP causes memory allocation in multi-camera scenarios ([UUM-19089](https://issuetracker.unity3d.com/issues/urp-memory-leak-when-in-play-mode))
    
*   Visual Effects: Editor crashes on VFXRenderer::AddAsRenderNode when assigning a Renderer’s materials toits to materials/sharedMaterials ([UUM-37360](https://issuetracker.unity3d.com/issues/editor-crashes-on-vfxrenderer-addasrendernode-when-assigning-a-renderers-materials-toits-to-materials-slash-sharedmaterials))
    
*   Visual Effects: \[VFX Graph\] Crash on VFXBatch::AddInstance when switching to Custom Batch Capacity in Asset Inspector ([UUM-38059](https://issuetracker.unity3d.com/issues/vfx-graph-crash-on-vfxbatch-addinstance-when-switching-to-custom-batch-capacity-in-asset-inspector))
    
*   Visual Effects - Legacy: \[Android\]\[Vulkan\] Visualisation corruption occurs when rendering Particles to Render Texture ([UUM-21106](https://issuetracker.unity3d.com/issues/android-vulkan-visualisation-corruption-occurs-when-rendering-particles-to-render-texture))
    
*   Web Platform: \[WebGL\] Build fails and Shader errors are logged when Code Optimisation is set to Runtime Speed ([UUM-40103](https://issuetracker.unity3d.com/issues/webgl-build-fails-and-shader-errors-are-logged-when-code-optimisation-is-set-to-runtime-speed))
    
*   XR SRP: Editor performance drops as OculusRuntime.WaitToBeginFrame Time ms increases to 150-200 ms in Play Mode when MSAA is enabled and Scene View is opened/focused ([UUM-40249](https://issuetracker.unity3d.com/issues/editor-performance-drops-as-oculusruntime-dot-waittobeginframe-time-ms-increases-to-150-200-ms-in-play-mode-when-msaa-is-enabled-and-scene-view-is-opened-slash-focused))