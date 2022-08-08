# Unity 2020.3.26

https://unity3d.com/unity/whats-new/2020.3.26

## Known Issues in 2020.3.26f1



*   AI: NavMesh Agent can not pass through passable area between carving NavMesh Obstacles ([1346325](https://issuetracker.unity3d.com/issues/navmesh-agent-can-not-pass-through-passable-area-between-carving-navmesh-obstacles))
    
*   Asset Bundles: Building process of the AssetBundles is slow when there is a huge filecount. ([1358059](https://issuetracker.unity3d.com/issues/building-process-of-the-assetbundles-is-slow-when-the-file-count-is-huge))
    
*   Build Pipeline: Windows build fails when using Deltatre Magma Engine ([1382217](https://issuetracker.unity3d.com/issues/windows-build-fails-when-using-deltatre-magma-engine))
    
*   GI: If a user is experience lighting coruption they be may required to reimport due to a fix to which correctly fixes a Uv unwrapping issue (1330830).
    
*   IL2CPP: Build fails with 'artifacts/tundra.dag.json does not exist yet' when using UnityEditor.InitializeOnLoadMethod in script ([1385676](https://issuetracker.unity3d.com/issues/il2cpp-build-fails-with-artifacts-slash-tundra-dot-dag-dot-json-does-not-exist-yet-when-using-unityeditor-dot-initializeonloadmethod-in-script))
    
*   Linux: Editor crashes at "\_\_assert\_fail\_base.cold" when opening a project (Linux) ([1375312](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-assert-fail-base-dot-cold-when-opening-a-project))
    
*   MacOS: \[M1\] "System is running out of memory" error is thrown when using Profiler as a Standalone Process with Deep Profile turned on ([1386242](https://issuetracker.unity3d.com/issues/system-is-running-out-of-memory-is-being-thrown-when-using-profiler-as-a-standalone-process-with-deep-profile-turned-on))
    
*   MacOS: \[OSX\]\[Editor\] DirectoryNotFoundException errors appear when a project is created inside a directory with unicode characters ([1377915](https://issuetracker.unity3d.com/issues/multiple-directorynotfoundexception-errors-appear-when-a-project-is-created-inside-a-directory-with-unicode-characters))
    
*   Mesh: Creating a mesh in Play Mode causes an "abnormal mesh bounds" error when using UploadMeshData() ([1364263](https://issuetracker.unity3d.com/issues/error-to-create-a-new-mesh-in-real-time-with-the-advanced-method-on-webgl))
    
*   Metal: Stuttering in Play mode when VSync is disabled ([1373811](https://issuetracker.unity3d.com/issues/metal-stuttering-in-play-mode-when-vsync-is-disabled))
    
*   Metal: Consistent EditorLoop 5-10ms spikes when using Metal API ([1378985](https://issuetracker.unity3d.com/issues/consistent-gfx-dot-waitforpresentongfxthread-5-10ms-spikes-when-using-metal-api))
    
*   Networking: UnityWebRequest.SendWebRequest delay occurring in 2019.4.30f1 and above ([1382113](https://issuetracker.unity3d.com/issues/networking-unitywebrequest-dot-sendwebrequest-delay-occurring-in-2019-dot-4-30f1-and-above))
    
*   OpenGL: Unity crashes when entering "-force-opengl" or "-force-glcore" in the Advanced Project Settings ([1374768](https://issuetracker.unity3d.com/issues/unity-crashes-when-entering-force-opengl-or-force-glcore-in-the-advanced-project-settings))
    
*   Profiling: Profiler's 'Call Stacks' button gets out of sync with PlayerConnection when the button is toggled after connecting to Player ([1377934](https://issuetracker.unity3d.com/issues/profiler-profilers-call-stacks-button-gets-out-of-sync-with-playerconnection-when-its-toggled-after-connecting-to-player))
    
*   Profiling: \[Memory Profiler\] Capturing Player built with higher Unity version crashes the Editor ([1386532](https://issuetracker.unity3d.com/issues/memory-profiler-capturing-player-built-with-higher-unity-version-crashes-the-editor))
    
*   Progressive Lightmapper: \[LightProbes\] Probes lose their lighting data after entering Play mode when Baked and Realtime GI are enabled ([1052045](https://issuetracker.unity3d.com/issues/light-probes-lose-their-lighting-data-after-entering-play-mode-when-baked-and-realtime-gi-are-enabled))
    
*   Progressive Lightmapper: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Scene Management: Crash when calling hideFlags after removing missing nested prefab ([1381563](https://issuetracker.unity3d.com/issues/crash-when-calling-hideflags-after-removing-missing-nested-prefab))
    
*   Scene/Game View: Camera resolution is set to default when opening the Editor ([1378321](https://issuetracker.unity3d.com/issues/camera-resolution-is-set-to-default-when-opening-the-editor))
    
*   Scripting: Editor sometimes crashes when entering Play Mode ([1380226](https://issuetracker.unity3d.com/issues/editor-crashes-sometimes-when-entering-play-mode))
    
*   Scripting: \[MacOS\] An Unhandled exception is thrown in the Editor.log and Console window when trying to build AssetBundles ([1383700](https://issuetracker.unity3d.com/issues/an-unhandled-exception-is-thrown-in-the-editor-dot-log-and-console-window-when-trying-to-build-assetbundles))
    
*   Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time ([1375015](https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time))
    
*   Shuriken: \[Particles\] Inspector breaks and errors are thrown when the Material field is deleted from the Particle System ([1379541](https://issuetracker.unity3d.com/issues/particles-inspector-breaks-and-errors-are-thrown-when-the-material-field-is-deleted-from-the-particle-system))
    
*   Shuriken: \[URP\] Particles are flickering when in Play Mode ([1390346](https://issuetracker.unity3d.com/issues/particles-are-flickering-when-in-play-mode))
    
*   Templates: Specific Actions dropdown tab does not appear when setting the Target of the Touch Trigger in the LEGO Template ([1390097](https://issuetracker.unity3d.com/issues/specific-actions-dropdown-tab-does-not-appear-when-setting-the-target-of-the-touch-trigger-in-the-lego-template))
    
*   Text: Editor crashes on TextCore::FontEngine::GetSystemFontReferencesInternal when opening the project ([1382082](https://issuetracker.unity3d.com/issues/editor-crashes-on-textcore-fontengine-getsystemfontreferencesinternal-when-opening-the-project))
    
*   Windows: Editor crashes or freezes with 'Copying file failed' error when importing a file from WinRAR Archiver ([1325310](https://issuetracker.unity3d.com/issues/editor-crashes-or-freezes-with-copying-file-failed-error-when-importing-a-file-from-winrar-archiver))