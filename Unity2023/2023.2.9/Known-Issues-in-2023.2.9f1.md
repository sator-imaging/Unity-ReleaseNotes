# Unity 2023.2.9

https://unity.com/releases/editor/whats-new/2023.2.9

## Known Issues in 2023.2.9f1



*   3D Physics: inertiaTensor does not reset to the original value when setting Rigidbody constraints from FreezeAll to None ([UUM-59748](https://issuetracker.unity3d.com/issues/inertiatensor-does-not-reset-to-the-original-value-when-setting-rigidbody-constraints-from-freezeall-to-none))
    
*   Asset Bundles: UV1 data is lost during AssetBundle build when Optimize Mesh Data is on ([UUM-57201](https://issuetracker.unity3d.com/issues/uv1-data-is-lost-during-assetbundle-build-when-optimize-mesh-data-is-on))
    
*   Audio Authoring: Crash on AudioUtil\_CUSTOM\_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))
    
*   Audio Authoring: \[Error\] Game object with AudioListener and OnAudioFilterRead throws an error when drawing the inspector ([UUM-61145](https://issuetracker.unity3d.com/issues/error-game-object-with-audiolistener-and-onaudiofilterread-throws-an-error-when-drawing-the-inspector))
    
*   Audio Random Container: Memory leak when creating ARC prefab ([UUM-61023](https://issuetracker.unity3d.com/issues/memory-leak-when-creating-arc-prefab))
    
*   Audio Random Container: Undoing loses ARC reference on an audio source ([UUM-62119](https://issuetracker.unity3d.com/issues/undoing-loses-arc-reference-on-an-audio-source))
    
*   Culling: Crash on PrepareDrawShadowsCommandStep1 when selecting a camera while the Occlusion Culling window is open ([UUM-506](https://issuetracker.unity3d.com/issues/crash-on-preparedrawshadowscommandstep1-when-selecting-a-camera-while-the-occlusion-culling-window-is-open))
    
*   DirectX12: Crash on D3D12Fence::Wait when using Forward+ Rendering Path with Better Shaders asset ([UUM-57113](https://issuetracker.unity3d.com/issues/crash-on-d3d12fence-wait-when-using-forward-plus-rendering-path-with-better-shaders-asset))
    
*   HD RP: Prefab preview thumbnails are not being rendered when a Project uses HDRP ([UUM-60000](https://issuetracker.unity3d.com/issues/prefab-preview-thumbnails-are-not-being-rendered-when-a-project-uses-hdrp))
    
*   HD RP: \[AMD\] Crash on GfxDeviceD3D12Base::DrawBuffersCommon when Baking Light with Virtual Offset on Probe Volumes ([UUM-59522](https://issuetracker.unity3d.com/issues/amd-crash-on-gfxdeviced3d12base-drawbufferscommon-when-baking-light-with-virtual-offset-on-probe-volumes))
    
*   IAP: \[Android\] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))
    
*   IL2CPP: IL2CPP error is thrown and the build fails when building project for the WebGL platform ([UUM-62523](https://issuetracker.unity3d.com/issues/il2cpp-error-is-thrown-and-the-build-fails-when-building-project-for-the-webgl-platform))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Input: Crash on InputDeviceIOCTL when closing Unity editor ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))
    
*   Metal: \[iOS\] App crashes with out of memory exception in UnityGfxDeviceWorker when starting the app ([UUM-55488](https://issuetracker.unity3d.com/issues/ios-app-crashes-with-out-of-memory-exception-in-unitygfxdeviceworker-when-starting-the-app))
    
*   Mono: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))
    
*   Platform Audio: \[Linux\] No audio output when playing audio ([UUM-53143](https://issuetracker.unity3d.com/issues/linux-no-audio-output-when-playing-audio))
    
*   Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))
    
*   Scene Management: Crash on GameObject::QueryComponentByType when opening a project ([UUM-58461](https://issuetracker.unity3d.com/issues/crash-on-gameobject-querycomponentbytype-when-opening-a-project))
    
*   Scripting Buildtime: Unclearable nunit error when installing/uninstalling the Entities package on a new project ([UUM-58284](https://issuetracker.unity3d.com/issues/unclearable-nunit-error-when-installing-slash-uninstalling-the-entities-package-on-a-new-project))
    
*   UI Toolkit Controls: Editor crashes when multi-selecting GameObjects with more than one serialized \[Flags\] enum ([UUM-60654](https://issuetracker.unity3d.com/issues/editor-crashes-when-multi-selecting-gameoobjects-with-more-than-one-serialized-flags-enum))
    
*   Universal RP: Memory leak when Application.runInBackground is set to false and the Editor is unfocused ([UUM-63345](https://issuetracker.unity3d.com/issues/memory-leak-when-application-dot-runinbackground-is-set-to-false-and-the-editor-is-unfocused))
    
*   WebRequest: UnityWebRequest crashes if invoked when player is quitting ([UUM-63150](https://issuetracker.unity3d.com/issues/unitywebrequest-crashes-if-invoked-when-player-is-quitting))