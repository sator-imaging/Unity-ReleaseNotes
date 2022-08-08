# Unity 2020.2.4

https://unity3d.com/unity/whats-new/2020.2.4

## Known Issues in 2020.2.4f1



*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   uGUI: AspectRatioFitter gives a warning when changing the Components Aspect Ratio if it's attached to a Canvas ([1302464](https://issuetracker.unity3d.com/issues/aspectratiofitter-new-restriction-in-2020-dot-2))
    
*   Templates: \[Linux\] Missing libdl.so library causes crash when entering Playmode for the second time or closing the Editor ([1237642](https://issuetracker.unity3d.com/issues/missing-libdl-dot-so-library-causes-crash-when-entering-playmode-for-the-second-time-or-closing-the-editor))
    
*   Global Illumination: Reflection Probe is not baked after pressing "Bake" button in the per-probe Inspector window ([1311231](https://issuetracker.unity3d.com/issues/reflection-probe-is-not-baked-after-pressing-bake-button-in-the-per-probe-inspector-window))
    
*   Scene Management: Freeze or crash on EditorSceneManager::ReloadScene when importing an Asset and reloading the opened Scene ([1309393](https://issuetracker.unity3d.com/issues/freeze-or-crash-on-editorscenemanager-reloadscene-when-importing-an-asset-and-reloading-the-opened-scene))
    
*   Asset Import Pipeline: Crash on core::StringStorageDefault::append when importing assets from the Asset Store ([1300615](https://issuetracker.unity3d.com/issues/crash-on-core-stringstoragedefault-append-when-importing-assets-from-the-asset-store))
    
*   Scripting: Application.quitting event is not raised when closing build ([1309540](https://issuetracker.unity3d.com/issues/application-dot-quitting-event-is-not-raised-when-closing-build))
    
*   CodeEditors: Crash on System.Net.Sockets.Socket:QueueIOSelectorJob when using a VPN and opening a project that uses Visual Studio ([1308797](https://issuetracker.unity3d.com/issues/crash-on-system-dot-net-dot-sockets-dot-socket-queueioselectorjob-when-using-a-vpn-and-opening-a-project-that-uses-visual-studio))
    
*   Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component ([1209765](https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   Texture: uGUI in Texture2D is different than in the Game view when calling ToTexture2D() method on a RenderTexture ([1301378](https://issuetracker.unity3d.com/issues/ugui-in-texture2d-is-different-than-in-the-game-view-when-calling-totexture2d-method-on-a-rendertexture))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Scene/Game View: \[Wild Crash\] Editor crashes on mono\_aot\_get\_cached\_class\_info when GizmoSetup has cached an outdated data ([1259765](https://issuetracker.unity3d.com/issues/wild-crash-editor-crashes-on-mono-aot-get-cached-class-info-when-gizmosetup-has-cached-an-outdated-data))
    
*   Build Pipeline: \[Cache Server\] Building process freezes on compiling shader variants when connected to Accelerator ([1296800](https://issuetracker.unity3d.com/issues/cache-server-building-process-freezes-on-compiling-shader-variants-when-connected-to-accelerator))
    
*   Input: \[Input System\] MultiplayerEventSystem throws a warning when more than one MultiplayerEventSystem is active ([1303961](https://issuetracker.unity3d.com/issues/input-system-multiplayereventsystem-throws-a-warning-when-more-than-one-multiplayereventsystem-is-active))
    
*   Shuriken: Infinity loop issue about Sub-Emitters of Particle System Editor ([1311111](https://issuetracker.unity3d.com/issues/infinity-loop-issue-about-sub-emitters-of-particle-system-editor))
    
*   UI Toolkit: Editor Crashes when name of Serialized Sprite variable is edited ([1302872](https://issuetracker.unity3d.com/issues/editor-crashes-when-name-of-serialized-sprite-variable-is-edited))
    
*   Windows: The Cursor is visible when Cursor.visible is set to false and new InputSystem package is used ([1273522](https://issuetracker.unity3d.com/issues/the-cursor-dot-visible-equals-false-does-not-work-when-inputsystem-package-is-installed))
    
*   XR: \[XR SDK\]\[Oculus\] EarlyUpdate.XRUpdate spikes inconsistently ([1262597](https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently))