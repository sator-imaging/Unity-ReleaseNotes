# Unity 2020.2.5

https://unity3d.com/unity/whats-new/2020.2.5

## Known Issues in 2020.2.5f1



*   Serialization: Editor crashes on RaiseException when allocating huge amount of memory ([1313492](https://issuetracker.unity3d.com/issues/editor-crashes-on-raiseexception-when-allocating-huge-amount-of-memory))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Mobile: Screen.dpi returns 0 on iPad Pro for projects built from 2019.4.16f1 ([1300359](https://issuetracker.unity3d.com/issues/screen-dot-dpi-returns-0-on-ipad-pro-for-projects-built-from-2019-dot-4-16f1))
    
*   MacOS: macOS builds no longer run when with a quarantine attribute due to incorrect codesigning ([1304455](https://issuetracker.unity3d.com/issues/macos-builds-now-contain-a-quarantine-attribute))
    
*   Global Illumination: Reflection Probe is not baked after pressing "Bake" button in the per-probe Inspector window ([1311231](https://issuetracker.unity3d.com/issues/reflection-probe-is-not-baked-after-pressing-bake-button-in-the-per-probe-inspector-window))
    
*   Physics: Crash in physx::NpArticulationReducedCoordinate::createCache() when calling JointState.SaveJointState for unparented bodies ([1264800](https://issuetracker.unity3d.com/issues/crash-in-physx-nparticulationreducedcoordinate-createcache-when-calling-jointstate-dot-savejointstate-for-unparented-bodies))
    
*   Scene Management: Freeze or crash on EditorSceneManager::ReloadScene when importing an Asset and reloading the opened Scene ([1309393](https://issuetracker.unity3d.com/issues/freeze-or-crash-on-editorscenemanager-reloadscene-when-importing-an-asset-and-reloading-the-opened-scene))
    
*   Scripting: Application.quitting event is not raised when closing build ([1309540](https://issuetracker.unity3d.com/issues/application-dot-quitting-event-is-not-raised-when-closing-build))
    
*   CodeEditors: Crash on System.Net.Sockets.Socket:QueueIOSelectorJob when using a VPN and opening a project that uses Visual Studio ([1308797](https://issuetracker.unity3d.com/issues/crash-on-system-dot-net-dot-sockets-dot-socket-queueioselectorjob-when-using-a-vpn-and-opening-a-project-that-uses-visual-studio))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Templates: \[Linux\] Missing libdl.so library causes crash when entering Playmode for the second time or closing the Editor ([1237642](https://issuetracker.unity3d.com/issues/missing-libdl-dot-so-library-causes-crash-when-entering-playmode-for-the-second-time-or-closing-the-editor))
    
*   Windows: The Cursor is visible when Cursor.visible is set to false and new InputSystem package is used ([1273522](https://issuetracker.unity3d.com/issues/the-cursor-dot-visible-equals-false-does-not-work-when-inputsystem-package-is-installed))
    
*   Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component ([1209765](https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Texture: uGUI in Texture2D is different than in the Game view when calling ToTexture2D() method on a RenderTexture ([1301378](https://issuetracker.unity3d.com/issues/ugui-in-texture2d-is-different-than-in-the-game-view-when-calling-totexture2d-method-on-a-rendertexture))
    
*   uGUI: AspectRatioFitter gives a warning when changing the Components Aspect Ratio if it's attached to a Canvas ([1302464](https://issuetracker.unity3d.com/issues/aspectratiofitter-new-restriction-in-2020-dot-2))
    
*   XR: \[XR SDK\]\[Oculus\] EarlyUpdate.XRUpdate spikes inconsistently ([1262597](https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently))